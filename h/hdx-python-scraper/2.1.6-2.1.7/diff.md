# Comparing `tmp/hdx-python-scraper-2.1.6.tar.gz` & `tmp/hdx_python_scraper-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdx-python-scraper-2.1.6.tar", last modified: Wed Jun 21 04:21:18 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `hdx-python-scraper-2.1.6.tar` & `hdx_python_scraper-2.1.7.tar`

### file list

```diff
@@ -1,143 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 04:21:18.170715 hdx-python-scraper-2.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 04:21:18.126715 hdx-python-scraper-2.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 04:21:18.130715 hdx-python-scraper-2.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/.github/workflows/run-python-tests.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/.readthedocs.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-21 04:21:18.170715 hdx-python-scraper-2.1.6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1576 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 04:21:18.130715 hdx-python-scraper-2.1.6/doc/
--rwxr-xr-x   0 runner    (1001) docker     (123)    62576 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/doc/main.md
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       67 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1505 2023-06-21 04:21:18.170715 hdx-python-scraper-2.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 04:21:18.130715 hdx-python-scraper-2.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 04:21:18.126715 hdx-python-scraper-2.1.6/src/hdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 04:21:18.130715 hdx-python-scraper-2.1.6/src/hdx/scraper/
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/src/hdx/scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 04:21:17.000000 hdx-python-scraper-2.1.6/src/hdx/scraper/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14131 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/src/hdx/scraper/base_scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 04:21:18.130715 hdx-python-scraper-2.1.6/src/hdx/scraper/configurable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/src/hdx/scraper/configurable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14976 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/src/hdx/scraper/configurable/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/src/hdx/scraper/configurable/resource_downloader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14635 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/src/hdx/scraper/configurable/rowparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    20217 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/src/hdx/scraper/configurable/scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/src/hdx/scraper/configurable/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 04:21:18.130715 hdx-python-scraper-2.1.6/src/hdx/scraper/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/src/hdx/scraper/outputs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2566 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/src/hdx/scraper/outputs/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2197 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/src/hdx/scraper/outputs/excelfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3087 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/src/hdx/scraper/outputs/googlesheets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9499 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/src/hdx/scraper/outputs/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    46947 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/src/hdx/scraper/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 04:21:18.134715 hdx-python-scraper-2.1.6/src/hdx/scraper/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/src/hdx/scraper/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/src/hdx/scraper/utilities/fallbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    16403 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/src/hdx/scraper/utilities/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/src/hdx/scraper/utilities/region_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/src/hdx/scraper/utilities/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)    16738 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/src/hdx/scraper/utilities/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 04:21:18.134715 hdx-python-scraper-2.1.6/src/hdx_python_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-21 04:21:18.000000 hdx-python-scraper-2.1.6/src/hdx_python_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-06-21 04:21:18.000000 hdx-python-scraper-2.1.6/src/hdx_python_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 04:21:18.000000 hdx-python-scraper-2.1.6/src/hdx_python_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-21 04:21:18.000000 hdx-python-scraper-2.1.6/src/hdx_python_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-21 04:21:18.000000 hdx-python-scraper-2.1.6/src/hdx_python_scraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 04:21:16.000000 hdx-python-scraper-2.1.6/src/hdx_python_scraper.egg-info/zip-safe
--rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 04:21:18.130715 hdx-python-scraper-2.1.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 04:21:18.134715 hdx-python-scraper-2.1.6/tests/config/
--rwxr-xr-x   0 runner    (1001) docker     (123)    63512 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/config/project_configuration.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 04:21:18.166715 hdx-python-scraper-2.1.6/tests/fixtures/
--rwxr-xr-x   0 runner    (1001) docker     (123)      873 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/access_2pacx-1vrszjzuyvt9i-mkrq2hbxrul2lx2vihkthqm-lae8nyhqty70zqtcufs3pxbhzgat1l2bkoa4-daoap-pub-gid-574237756-single-true-output-csv.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/additional-json.json
--rw-r--r--   0 runner    (1001) docker     (123)    57147 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/affected_targeted_reached_affected_targeted_reached_eth_ethiopia_drought_affected_targeted_reached_by_cluster.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/affected_targeted_reached_affected_targeted_reached_ken_kenya_drought_affected_targeted_reached_by_cluster.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/affected_targeted_reached_affected_targeted_reached_som_somalia_drought_affected_targeted_reached_by_cluster.csv
--rw-r--r--   0 runner    (1001) docker     (123)   985584 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/altworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/cbpf-allocations-and-contributions.json
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/cbpf2-allocations-and-contributions.json
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/cerf-covid-19-allocations.json
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/cerf2-covid-19-allocations.json
--rw-r--r--   0 runner    (1001) docker     (123)  8415576 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/cerf2_global_download-full-pfmb-allocations.csv
--rw-r--r--   0 runner    (1001) docker     (123)  8415576 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/cerf_global_download-full-pfmb-allocations.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/covax_2pacx-1vtvzu79pptfaa2syevoqfyrrjy63djwitqu0ffbxiqczoun9k9timwmrvfgg1rbsnlmgyugzseiaye2-pub-gid-992438980-single-true-output-csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)   201089 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/covidtests_data-owid-covid-data.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/download-hno-2017-sahel-nutrition.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/download-hno-2017-sahel-people-in-need.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/education_closures_download-covid-impact-education.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33843 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/education_enrolment_download-countries-enrollment-data-uis-feb-22.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/ethiopia-drought-related-key-figures.json
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/ethiopia-pin-targeted-reached-by-location-and-cluster.json
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/fallbacks.json
--rwxr-xr-x   0 runner    (1001) docker     (123)   164046 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/gam_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx
--rwxr-xr-x   0 runner    (1001) docker     (123)   164046 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/gam_other_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    12411 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/global-school-closures-covid19.json
--rw-r--r--   0 runner    (1001) docker     (123)    78566 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/hdx_resource_downloader_xlsx_ukr_border_crossings_090622.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/idmc-internally-displaced-persons-idps.json
--rw-r--r--   0 runner    (1001) docker     (123)    51259 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/idps_download-displacement-data.csv
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/idps_override_population-widget-id-264111-geo-id-693-population-group-54074999.json
--rw-r--r--   0 runner    (1001) docker     (123)  1371019 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/idps_somalia_download-som-unhcr-prmn-displacement-dataset.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/ipc_somalia_download-som-food-insecurity-oct-dec2022-projection.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/kenya-drought-related-key-figures.json
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/kenya-pin-targeted-reached-by-location-and-cluster.json
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/key_figures_eth_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/key_figures_ken_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/key_figures_som_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)   985584 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/ourworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
--rw-r--r--   0 runner    (1001) docker     (123)   985584 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/ourworldindata_other_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/population.json
--rwxr-xr-x   0 runner    (1001) docker     (123)  1626112 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/population_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls
--rwxr-xr-x   0 runner    (1001) docker     (123)  1626112 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/population_other_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls
--rw-r--r--   0 runner    (1001) docker     (123)    19982 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/regions_download-tbl-regcov-2020-ocha.xlsx
--rwxr-xr-x   0 runner    (1001) docker     (123)      477 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/sadd-countries-to-include.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      641 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/sadd_covid-data-dataset-fullvars-extype-csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/sahel-humanitarian-needs-overview.json
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/somalia-acute-food-insecurity-country-data.json
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/somalia-drought-related-key-figures.json
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/somalia-internally-displaced-persons-idps.json
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/somalia-pin-targeted-reached-by-location-and-cluster.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     5328 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/test_output.xlsx
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/test_scraper_all.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       99 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/test_scraper_other.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/test_scraper_population.json
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/timeseries_casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14414 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/total-covid-19-tests-performed-by-country.json
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/ukraine-border-crossings.json
--rw-r--r--   0 runner    (1001) docker     (123)    16153 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/ukraine-who-does-what-where-3w.json
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/unocha-office-locations.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    21332 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/who_national2_who-covid-19-global-data.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    21332 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/who_national_who-covid-19-global-data.csv
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/whowhatwhere_afg_3w_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/fixtures/whowhatwhere_notags_3w_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 04:21:18.130715 hdx-python-scraper-2.1.6/tests/hdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 04:21:18.170715 hdx-python-scraper-2.1.6/tests/hdx/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/affected_targeted_reached.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4631 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/education_closures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/education_enrolment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7256 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/test_output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8566 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/test_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/test_regionlookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/test_runner_get_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    14568 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/test_scrapers_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16735 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/test_scrapers_appenddata.py
--rw-r--r--   0 runner    (1001) docker     (123)    34106 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/test_scrapers_custom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25503 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/test_scrapers_global.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/test_scrapers_multipleurls.py
--rw-r--r--   0 runner    (1001) docker     (123)    26538 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/test_scrapers_national.py
--rw-r--r--   0 runner    (1001) docker     (123)    15994 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/test_scrapers_regionaltoplevel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/test_scrapers_resource_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/test_scrapers_subnational.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/test_scrapers_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-21 04:20:56.000000 hdx-python-scraper-2.1.6/tests/hdx/scraper/unhcr_myanmar_idps.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     5635 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/.config/black.toml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/.config/coveragerc
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/.config/pytest.ini
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/documentation/.readthedocs.yaml
+-rwxr-xr-x   0        0        0    62577 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/documentation/main.md
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/documentation/pydoc-markdown.yaml
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/_version.py
+-rw-r--r--   0        0        0    14130 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/base_scraper.py
+-rw-r--r--   0        0        0    46946 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/__init__.py
+-rw-r--r--   0        0        0    14976 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/aggregator.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/resource_downloader.py
+-rwxr-xr-x   0        0        0    14635 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/rowparser.py
+-rw-r--r--   0        0        0    20217 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/scraper.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/timeseries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/outputs/__init__.py
+-rwxr-xr-x   0        0        0     2566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/outputs/base.py
+-rwxr-xr-x   0        0        0     2197 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/outputs/excelfile.py
+-rwxr-xr-x   0        0        0     3087 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/outputs/googlesheets.py
+-rwxr-xr-x   0        0        0     9498 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/outputs/json.py
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/__init__.py
+-rw-r--r--   0        0        0     6186 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/fallbacks.py
+-rw-r--r--   0        0        0    16403 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/reader.py
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/region_lookup.py
+-rw-r--r--   0        0        0    11204 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/sources.py
+-rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/writer.py
+-rwxr-xr-x   0        0        0    63512 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/config/project_configuration.yaml
+-rwxr-xr-x   0        0        0      873 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/access_2pacx-1vrszjzuyvt9i-mkrq2hbxrul2lx2vihkthqm-lae8nyhqty70zqtcufs3pxbhzgat1l2bkoa4-daoap-pub-gid-574237756-single-true-output-csv.csv
+-rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/additional-json.json
+-rw-r--r--   0        0        0    57147 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/affected_targeted_reached_affected_targeted_reached_eth_ethiopia_drought_affected_targeted_reached_by_cluster.csv
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/affected_targeted_reached_affected_targeted_reached_ken_kenya_drought_affected_targeted_reached_by_cluster.csv
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/affected_targeted_reached_affected_targeted_reached_som_somalia_drought_affected_targeted_reached_by_cluster.csv
+-rw-r--r--   0        0        0   985584 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/altworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv
+-rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/cbpf-allocations-and-contributions.json
+-rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/cbpf2-allocations-and-contributions.json
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/cerf-covid-19-allocations.json
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/cerf2-covid-19-allocations.json
+-rw-r--r--   0        0        0  8415576 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/cerf2_global_download-full-pfmb-allocations.csv
+-rw-r--r--   0        0        0  8415576 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/cerf_global_download-full-pfmb-allocations.csv
+-rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/covax_2pacx-1vtvzu79pptfaa2syevoqfyrrjy63djwitqu0ffbxiqczoun9k9timwmrvfgg1rbsnlmgyugzseiaye2-pub-gid-992438980-single-true-output-csv.csv
+-rw-r--r--   0        0        0   201089 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/covidtests_data-owid-covid-data.xlsx
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/download-hno-2017-sahel-nutrition.csv
+-rw-r--r--   0        0        0    10275 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/download-hno-2017-sahel-people-in-need.xlsx
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/education_closures_download-covid-impact-education.csv
+-rw-r--r--   0        0        0    33843 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/education_enrolment_download-countries-enrollment-data-uis-feb-22.xlsx
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/ethiopia-drought-related-key-figures.json
+-rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/ethiopia-pin-targeted-reached-by-location-and-cluster.json
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/fallbacks.json
+-rwxr-xr-x   0        0        0   164046 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/gam_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx
+-rwxr-xr-x   0        0        0   164046 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/gam_other_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx
+-rw-r--r--   0        0        0    12411 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/global-school-closures-covid19.json
+-rw-r--r--   0        0        0    78566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/hdx_resource_downloader_xlsx_ukr_border_crossings_090622.xlsx
+-rw-r--r--   0        0        0     7619 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/idmc-internally-displaced-persons-idps.json
+-rw-r--r--   0        0        0    51259 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/idps_download-displacement-data.csv
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/idps_override_population-widget-id-264111-geo-id-693-population-group-54074999.json
+-rw-r--r--   0        0        0  1371019 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/idps_somalia_download-som-unhcr-prmn-displacement-dataset.xlsx
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/ipc_somalia_download-som-food-insecurity-oct-dec2022-projection.csv
+-rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/kenya-drought-related-key-figures.json
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/kenya-pin-targeted-reached-by-location-and-cluster.json
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/key_figures_eth_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/key_figures_ken_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/key_figures_som_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv
+-rw-r--r--   0        0        0   985584 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/ourworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
+-rw-r--r--   0        0        0   985584 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/ourworldindata_other_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
+-rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/population.json
+-rwxr-xr-x   0        0        0  1626112 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/population_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls
+-rwxr-xr-x   0        0        0  1626112 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/population_other_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls
+-rw-r--r--   0        0        0    19982 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/regions_download-tbl-regcov-2020-ocha.xlsx
+-rwxr-xr-x   0        0        0      477 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/sadd-countries-to-include.csv
+-rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/sadd_covid-data-dataset-fullvars-extype-csv.csv
+-rw-r--r--   0        0        0    10068 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/sahel-humanitarian-needs-overview.json
+-rw-r--r--   0        0        0     7089 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/somalia-acute-food-insecurity-country-data.json
+-rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/somalia-drought-related-key-figures.json
+-rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/somalia-internally-displaced-persons-idps.json
+-rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/somalia-pin-targeted-reached-by-location-and-cluster.json
+-rwxr-xr-x   0        0        0     5328 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/test_output.xlsx
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/test_scraper_all.json
+-rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/test_scraper_other.json
+-rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/test_scraper_population.json
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/timeseries_casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv
+-rw-r--r--   0        0        0    14414 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/total-covid-19-tests-performed-by-country.json
+-rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/ukraine-border-crossings.json
+-rw-r--r--   0        0        0    16153 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/ukraine-who-does-what-where-3w.json
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/unocha-office-locations.json
+-rwxr-xr-x   0        0        0    21332 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/who_national2_who-covid-19-global-data.csv
+-rwxr-xr-x   0        0        0    21332 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/who_national_who-covid-19-global-data.csv
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/whowhatwhere_afg_3w_data.csv
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/whowhatwhere_notags_3w_data.csv
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/__init__.py
+-rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/affected_targeted_reached.py
+-rwxr-xr-x   0        0        0     4631 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/conftest.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/education_closures.py
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/education_enrolment.py
+-rwxr-xr-x   0        0        0     7256 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_output.py
+-rwxr-xr-x   0        0        0     8566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_readers.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_regionlookup.py
+-rw-r--r--   0        0        0     9283 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_runner_get_results.py
+-rw-r--r--   0        0        0    14566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_aggregation.py
+-rw-r--r--   0        0        0    16734 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_appenddata.py
+-rw-r--r--   0        0        0    34104 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_custom.py
+-rwxr-xr-x   0        0        0    25502 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_global.py
+-rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_multipleurls.py
+-rw-r--r--   0        0        0    26536 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_national.py
+-rw-r--r--   0        0        0    15992 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_regionaltoplevel.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_resource_downloaders.py
+-rw-r--r--   0        0        0    17601 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_subnational.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_timeseries.py
+-rw-r--r--   0        0        0     8096 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_sources.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_utils.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/unhcr_myanmar_idps.py
+-rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/.gitignore
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/LICENSE
+-rwxr-xr-x   0        0        0     1711 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/README.md
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/PKG-INFO
```

### Comparing `hdx-python-scraper-2.1.6/.github/workflows/publish.yml` & `hdx_python_scraper-2.1.7/.github/workflows/publish.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -6,25 +6,28 @@
 
 jobs:
   publish:
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v3
-    - name: Get history and tags for SCM versioning to work
+    - name: Get history and tags for versioning to work
       run: |
         git fetch --prune --unshallow
         git fetch --depth=1 origin +refs/tags/*:refs/tags/*
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install --upgrade tox-gh-actions
-    - name: Publish with tox and twine
+        pip install --upgrade hatch
+    - name: Build with hatch
+      run: |
+        hatch build
+    - name: Publish with hatch
       env:
-        TWINE_USERNAME: ${{ secrets.TWINE_USERNAME }}
-        TWINE_PASSWORD: ${{ secrets.TWINE_PASSWORD }}
+        HATCH_INDEX_USER: ${{secrets.HATCH_INDEX_USER}}
+        HATCH_INDEX_AUTH: ${{secrets.HATCH_INDEX_AUTH}}
       run: |
-        tox -e publish
+        hatch publish
```

### Comparing `hdx-python-scraper-2.1.6/.github/workflows/run-python-tests.yml` & `hdx_python_scraper-2.1.7/.github/workflows/run-python-tests.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -20,22 +20,29 @@
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install --upgrade tox-gh-actions
-    - name: Test with tox/pytest
+        pip install --upgrade hatch
+    - name: Test with hatch/pytest
       env:
         GSHEET_AUTH: ${{ secrets.GSHEET_AUTH }}
       run: |
-        tox
+        hatch run test:test
+    - name: Check styling
+      if: always()
+      run: |
+        hatch run lint:style
     - name: Publish Unit Test Results
       uses: EnricoMi/publish-unit-test-result-action@v2
       if: always()
       with:
         github_token: ${{ secrets.GITHUB_TOKEN }}
-        junit_files: .tox/*.xml
-    - name: Upload Coverage Results
-      uses: codecov/codecov-action@v3
-      if: success()
+        junit_files: test-results.xml
+    - name: Publish in Coveralls
+      uses: coverallsapp/github-action@v2
+      with:
+        github-token: ${{ secrets.GITHUB_TOKEN }}
+        flag-name: tests
+        format: lcov
```

### Comparing `hdx-python-scraper-2.1.6/.gitignore` & `hdx_python_scraper-2.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/LICENSE` & `hdx_python_scraper-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/PKG-INFO` & `hdx_python_scraper-2.1.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 Metadata-Version: 2.1
 Name: hdx-python-scraper
-Version: 2.1.6
+Version: 2.1.7
 Summary: HDX Python scraper utilities to assemble data from multiple sources
-Home-page: https://github.com/OCHA-DAP/hdx-python-scraper
-Author: Michael Rans
-Author-email: rans@email.com
+Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-scraper
+Author-email: Michael Rans <rans@email.com>
 License: MIT
-Keywords: HDX,scrapers,data assembly,data transformation,tabular data,library
-Platform: any
+License-File: LICENSE
+Keywords: HDX,data assembly,data transformation,scrapers,tabular data
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8
+Requires-Dist: gspread
+Requires-Dist: hdx-python-api>=6.0.4
+Requires-Dist: regex
+Provides-Extra: dev
+Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: pandas
-License-File: LICENSE
+Requires-Dist: pandas>=2.0.2; extra == 'pandas'
+Provides-Extra: test
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Description-Content-Type: text/markdown
 
-[![Build Status](https://github.com/OCHA-DAP/hdx-python-scraper/actions/workflows/run-python-tests.yml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-scraper/actions/workflows/run-python-tests.yml)
-[![Coverage Status](https://codecov.io/gh/OCHA-DAP/hdx-python-scraper/branch/main/graph/badge.svg?token=JpWZc5js4y)](https://codecov.io/gh/OCHA-DAP/hdx-python-scraper)
+[![Build Status](https://github.com/OCHA-DAP/hdx-python-scraper/actions/workflows/run-python-tests.yaml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-scraper/actions/workflows/run-python-tests.yaml)
+[![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-scraper/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-scraper?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Downloads](https://img.shields.io/pypi/dm/hdx-python-scraper.svg)](https://pypistats.org/packages/hdx-python-scraper)
 
 The HDX Python Scraper Library is designed to enable you to easily develop code that 
 assembles data from one or more tabular sources that can be csv, xls, xlsx or JSON. It 
 uses a YAML file that specifies for each source what needs to be read and allows some 
 transformations to be performed on the data. The output is written to JSON, Google sheets 
 and/or Excel and includes the addition of 
 [Humanitarian Exchange Language (HXL)](https://hxlstandard.org/) hashtags specified in
```

### Comparing `hdx-python-scraper-2.1.6/README.md` & `hdx_python_scraper-2.1.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-[![Build Status](https://github.com/OCHA-DAP/hdx-python-scraper/actions/workflows/run-python-tests.yml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-scraper/actions/workflows/run-python-tests.yml)
-[![Coverage Status](https://codecov.io/gh/OCHA-DAP/hdx-python-scraper/branch/main/graph/badge.svg?token=JpWZc5js4y)](https://codecov.io/gh/OCHA-DAP/hdx-python-scraper)
+[![Build Status](https://github.com/OCHA-DAP/hdx-python-scraper/actions/workflows/run-python-tests.yaml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-scraper/actions/workflows/run-python-tests.yaml)
+[![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-scraper/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-scraper?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Downloads](https://img.shields.io/pypi/dm/hdx-python-scraper.svg)](https://pypistats.org/packages/hdx-python-scraper)
 
 The HDX Python Scraper Library is designed to enable you to easily develop code that 
 assembles data from one or more tabular sources that can be csv, xls, xlsx or JSON. It 
 uses a YAML file that specifies for each source what needs to be read and allows some 
 transformations to be performed on the data. The output is written to JSON, Google sheets 
 and/or Excel and includes the addition of 
 [Humanitarian Exchange Language (HXL)](https://hxlstandard.org/) hashtags specified in
```

### Comparing `hdx-python-scraper-2.1.6/doc/main.md` & `hdx_python_scraper-2.1.7/documentation/main.md`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         runner.run(prioritise_scrapers=("population_national", "population_subnational"))
         results = runner.get_results()["national"]
         assert results["headers"] == [("header1", header2"...), ("#hxltag1", "#hxltag2",...)]
         assert results["values"] == [{"AFG": 38041754, "PSE": ...}, {"AFG": 123, "PSE": ...}, ...]
         assert results["sources"] == [("#population", "2020-10-01", "World Bank", "https://..."), ...]
         
 The framework is configured by passing in a configuration. Typically this will come from 
-a YAML file such as `config/project_configuration.yml`. To use the current date/time, 
+a YAML file such as `config/project_configuration.yaml`. To use the current date/time, 
 there is a now_utc() function from the dependency HDX Python Utilities. 
 
 ### Read Class
 
 The Read class inherits from Retrieve from the HDX Python Utilities library. The 
 Retrieve class inherits from BaseDownload which specifies a number of standard
 methods that all downloaders should have: `download_file`, `download_text`,
```

### Comparing `hdx-python-scraper-2.1.6/src/hdx/scraper/base_scraper.py` & `hdx_python_scraper-2.1.7/src/hdx/scraper/base_scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from typing import Dict, List, Optional, Set, Tuple
 
-from hdx.utilities.dictandlist import dict_of_lists_add
-from hdx.utilities.typehint import ListTuple
-
 from .utilities.reader import Read
 from .utilities.sources import Sources
+from hdx.utilities.dictandlist import dict_of_lists_add
+from hdx.utilities.typehint import ListTuple
 
 
 class BaseScraper(ABC):
     """Base scraper class for scrapers to inherit
 
     Args:
         name (str): Name of scraper
```

### Comparing `hdx-python-scraper-2.1.6/src/hdx/scraper/configurable/aggregator.py` & `hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/aggregator.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import logging
 import sys
 from copy import deepcopy
 from typing import Any, Dict, List, Optional, Tuple, Union
 
+from slugify import slugify
+
+from ..base_scraper import BaseScraper
+from ..utilities.reader import Read
 from hdx.utilities.dictandlist import dict_of_lists_add
 from hdx.utilities.text import (  # noqa: F401
     get_fraction_str,
     get_numeric_if_possible,
     number_format,
 )
 from hdx.utilities.typehint import ListTuple
-from slugify import slugify
-
-from ..base_scraper import BaseScraper
-from ..utilities.reader import Read
 
 logger = logging.getLogger(__name__)
 
 
 class Aggregator(BaseScraper):
     """Each aggregator is configured from dataset information that can come
     from a YAML file for example. When run, it works out headers and aggregated values.
```

### Comparing `hdx-python-scraper-2.1.6/src/hdx/scraper/configurable/resource_downloader.py` & `hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/resource_downloader.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/src/hdx/scraper/configurable/rowparser.py` & `hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/rowparser.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import logging
 from datetime import datetime
 from operator import itemgetter
 from typing import Dict, Generator, Iterator, List, Optional, Tuple
 
 import hxl
 from dateutil.relativedelta import relativedelta  # noqa: F401
+
+from ..utilities import match_template
 from hdx.location.adminlevel import AdminLevel
 from hdx.location.country import Country
 from hdx.utilities.dateparse import parse_date
 from hdx.utilities.dictandlist import dict_of_lists_add
 
-from ..utilities import match_template
-
 logger = logging.getLogger(__name__)
 
 
 class RowParser:
     """RowParser class for parsing each row.
 
     Args:
```

### Comparing `hdx-python-scraper-2.1.6/src/hdx/scraper/configurable/scraper.py` & `hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/scraper.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import copy
 import logging
 from datetime import datetime
 from typing import Any, Dict, Iterator, List, Optional, Tuple
 
 import regex
+
+from ..base_scraper import BaseScraper
+from ..utilities import get_rowval
+from ..utilities.sources import Sources
+from .rowparser import RowParser
 from hdx.location.adminlevel import AdminLevel
 from hdx.utilities.dateparse import (
     get_datetime_from_timestamp,
     now_utc,
     parse_date,
 )
 from hdx.utilities.dictandlist import dict_of_lists_add
@@ -15,19 +20,14 @@
 from hdx.utilities.errors_onexit import ErrorsOnExit
 from hdx.utilities.text import (  # noqa: F401
     get_fraction_str,
     get_numeric_if_possible,
     number_format,
 )
 
-from ..base_scraper import BaseScraper
-from ..utilities import get_rowval
-from ..utilities.sources import Sources
-from .rowparser import RowParser
-
 logger = logging.getLogger(__name__)
 
 
 class ConfigurableScraper(BaseScraper):
     """Each configurable scraper is configured from dataset information that can come
     from a YAML file for example. When run, it works out headers and values. It also
     overrides add_sources where sources are compiled and returned. If dealing with
```

### Comparing `hdx-python-scraper-2.1.6/src/hdx/scraper/configurable/timeseries.py` & `hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 from datetime import datetime
 from typing import Dict
 
-from hdx.utilities.dateparse import now_utc, parse_date
-
 from ..base_scraper import BaseScraper
 from ..outputs.base import BaseOutput
+from hdx.utilities.dateparse import now_utc, parse_date
 
 logger = logging.getLogger(__name__)
 
 
 class TimeSeries(BaseScraper):
     """Each time series scraper is configured from dataset information that can come
     from a YAML file for example. When run, it populates the given outputs with
```

### Comparing `hdx-python-scraper-2.1.6/src/hdx/scraper/outputs/base.py` & `hdx_python_scraper-2.1.7/src/hdx/scraper/outputs/base.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/src/hdx/scraper/outputs/excelfile.py` & `hdx_python_scraper-2.1.7/src/hdx/scraper/outputs/excelfile.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/src/hdx/scraper/outputs/googlesheets.py` & `hdx_python_scraper-2.1.7/src/hdx/scraper/outputs/googlesheets.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/src/hdx/scraper/outputs/json.py` & `hdx_python_scraper-2.1.7/src/hdx/scraper/outputs/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import logging
 from os.path import join
 from typing import Any, Dict, List, Optional, Union
 
+from .base import BaseOutput
 from hdx.utilities.dictandlist import dict_of_lists_add
 from hdx.utilities.saver import save_json
 
-from .base import BaseOutput
-
 try:
     from pandas import DataFrame
 except ImportError:
     DataFrame = None
 
 
 from ..utilities import match_template
```

### Comparing `hdx-python-scraper-2.1.6/src/hdx/scraper/runner.py` & `hdx_python_scraper-2.1.7/src/hdx/scraper/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import logging
 from datetime import datetime
 from traceback import format_exc
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
-from hdx.location.adminlevel import AdminLevel
-from hdx.utilities.dateparse import now_utc
-from hdx.utilities.errors_onexit import ErrorsOnExit
-from hdx.utilities.typehint import ListTuple
-
 from .base_scraper import BaseScraper
 from .configurable.aggregator import Aggregator
 from .configurable.resource_downloader import ResourceDownloader
 from .configurable.scraper import ConfigurableScraper
 from .configurable.timeseries import TimeSeries
 from .outputs.base import BaseOutput
 from .utilities import get_startend_dates_from_reference_period
 from .utilities.fallbacks import Fallbacks
 from .utilities.reader import Read
 from .utilities.sources import Sources
+from hdx.location.adminlevel import AdminLevel
+from hdx.utilities.dateparse import now_utc
+from hdx.utilities.errors_onexit import ErrorsOnExit
+from hdx.utilities.typehint import ListTuple
 
 logger = logging.getLogger(__name__)
 
 
 class Runner:
     """The Runner class is the means by which scrapers are set up and run.
```

### Comparing `hdx-python-scraper-2.1.6/src/hdx/scraper/utilities/__init__.py` & `hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/src/hdx/scraper/utilities/fallbacks.py` & `hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/fallbacks.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/src/hdx/scraper/utilities/reader.py` & `hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/reader.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import logging
 from datetime import datetime
 from os.path import join
 from typing import Any, Dict, Iterator, List, Optional, Tuple
 from urllib.parse import parse_qsl
 
 import hxl
+from hxl.input import InputOptions, munge_url
+from slugify import slugify
+
+from . import get_startend_dates_from_reference_period, match_template
+from .sources import Sources
 from hdx.data.dataset import Dataset
 from hdx.data.resource import Resource
 from hdx.utilities.downloader import Download
 from hdx.utilities.retriever import Retrieve
 from hdx.utilities.saver import save_json
 from hdx.utilities.typehint import ListTuple
-from hxl.input import InputOptions, munge_url
-from slugify import slugify
-
-from . import get_startend_dates_from_reference_period, match_template
-from .sources import Sources
 
 logger = logging.getLogger(__name__)
 
 
 class Read(Retrieve):
     """Read data from tabular source eg. csv, xls, xlsx
```

### Comparing `hdx-python-scraper-2.1.6/src/hdx/scraper/utilities/region_lookup.py` & `hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/region_lookup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 from typing import Dict
 
+from .reader import Read
 from hdx.utilities.dictandlist import dict_of_sets_add
 from hdx.utilities.typehint import ListTuple
 
-from .reader import Read
-
 logger = logging.getLogger(__name__)
 
 
 class RegionLookup:
     """Provide list of regions and mappings from country ISO3 code to region names."""
 
     iso3_to_region = {}
```

### Comparing `hdx-python-scraper-2.1.6/src/hdx/scraper/utilities/sources.py` & `hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/sources.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/src/hdx/scraper/utilities/writer.py` & `hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import logging
 from copy import deepcopy
 from typing import Dict, List, Optional, Tuple, Union
 
-from hdx.location.adminlevel import AdminLevel
-from hdx.location.country import Country
-from hdx.utilities.typehint import ListTuple
-
 from ..outputs.base import BaseOutput
 from ..runner import Runner
 from .sources import Sources
+from hdx.location.adminlevel import AdminLevel
+from hdx.location.country import Country
+from hdx.utilities.typehint import ListTuple
 
 try:
     from pandas import DataFrame
 except ImportError:
     DataFrame = None
 
 logger = logging.getLogger(__name__)
@@ -287,17 +286,18 @@
             lambda adm: adm,
             Country.get_country_name_from_iso3,
         ]
 
         if flag_countries:
             headers[0].append(flag_countries["header"])
             headers[1].append(flag_countries["hxltag"])
-            isfc_fn = (
-                lambda adm: "Y" if adm in flag_countries["countries"] else "N"
-            )
+
+            def isfc_fn(adm):
+                return "Y" if adm in flag_countries["countries"] else "N"
+
             fns.append(isfc_fn)
 
         if iso3_to_region:
             headers[0].append("region")
             headers[1].append("#region+name")
 
             def region_fn(adm):
```

### Comparing `hdx-python-scraper-2.1.6/tests/config/project_configuration.yml` & `hdx_python_scraper-2.1.7/tests/config/project_configuration.yaml`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/access_2pacx-1vrszjzuyvt9i-mkrq2hbxrul2lx2vihkthqm-lae8nyhqty70zqtcufs3pxbhzgat1l2bkoa4-daoap-pub-gid-574237756-single-true-output-csv.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/access_2pacx-1vrszjzuyvt9i-mkrq2hbxrul2lx2vihkthqm-lae8nyhqty70zqtcufs3pxbhzgat1l2bkoa4-daoap-pub-gid-574237756-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/affected_targeted_reached_affected_targeted_reached_eth_ethiopia_drought_affected_targeted_reached_by_cluster.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/affected_targeted_reached_affected_targeted_reached_eth_ethiopia_drought_affected_targeted_reached_by_cluster.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/affected_targeted_reached_affected_targeted_reached_ken_kenya_drought_affected_targeted_reached_by_cluster.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/affected_targeted_reached_affected_targeted_reached_ken_kenya_drought_affected_targeted_reached_by_cluster.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/affected_targeted_reached_affected_targeted_reached_som_somalia_drought_affected_targeted_reached_by_cluster.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/affected_targeted_reached_affected_targeted_reached_som_somalia_drought_affected_targeted_reached_by_cluster.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/altworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/altworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/cbpf-allocations-and-contributions.json` & `hdx_python_scraper-2.1.7/tests/fixtures/cbpf-allocations-and-contributions.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/cbpf2-allocations-and-contributions.json` & `hdx_python_scraper-2.1.7/tests/fixtures/cbpf2-allocations-and-contributions.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/cerf-covid-19-allocations.json` & `hdx_python_scraper-2.1.7/tests/fixtures/cerf-covid-19-allocations.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/cerf2-covid-19-allocations.json` & `hdx_python_scraper-2.1.7/tests/fixtures/cerf2-covid-19-allocations.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/cerf2_global_download-full-pfmb-allocations.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/cerf2_global_download-full-pfmb-allocations.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/cerf_global_download-full-pfmb-allocations.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/cerf_global_download-full-pfmb-allocations.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/covax_2pacx-1vtvzu79pptfaa2syevoqfyrrjy63djwitqu0ffbxiqczoun9k9timwmrvfgg1rbsnlmgyugzseiaye2-pub-gid-992438980-single-true-output-csv.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/covax_2pacx-1vtvzu79pptfaa2syevoqfyrrjy63djwitqu0ffbxiqczoun9k9timwmrvfgg1rbsnlmgyugzseiaye2-pub-gid-992438980-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/covidtests_data-owid-covid-data.xlsx` & `hdx_python_scraper-2.1.7/tests/fixtures/covidtests_data-owid-covid-data.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/download-hno-2017-sahel-nutrition.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/download-hno-2017-sahel-nutrition.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/download-hno-2017-sahel-people-in-need.xlsx` & `hdx_python_scraper-2.1.7/tests/fixtures/download-hno-2017-sahel-people-in-need.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/education_enrolment_download-countries-enrollment-data-uis-feb-22.xlsx` & `hdx_python_scraper-2.1.7/tests/fixtures/education_enrolment_download-countries-enrollment-data-uis-feb-22.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/ethiopia-drought-related-key-figures.json` & `hdx_python_scraper-2.1.7/tests/fixtures/ethiopia-drought-related-key-figures.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/ethiopia-pin-targeted-reached-by-location-and-cluster.json` & `hdx_python_scraper-2.1.7/tests/fixtures/ethiopia-pin-targeted-reached-by-location-and-cluster.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/fallbacks.json` & `hdx_python_scraper-2.1.7/tests/fixtures/fallbacks.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/gam_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx` & `hdx_python_scraper-2.1.7/tests/fixtures/gam_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/gam_other_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx` & `hdx_python_scraper-2.1.7/tests/fixtures/gam_other_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/global-school-closures-covid19.json` & `hdx_python_scraper-2.1.7/tests/fixtures/global-school-closures-covid19.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/hdx_resource_downloader_xlsx_ukr_border_crossings_090622.xlsx` & `hdx_python_scraper-2.1.7/tests/fixtures/hdx_resource_downloader_xlsx_ukr_border_crossings_090622.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/idmc-internally-displaced-persons-idps.json` & `hdx_python_scraper-2.1.7/tests/fixtures/idmc-internally-displaced-persons-idps.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/idps_download-displacement-data.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/idps_download-displacement-data.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/idps_override_population-widget-id-264111-geo-id-693-population-group-54074999.json` & `hdx_python_scraper-2.1.7/tests/fixtures/idps_override_population-widget-id-264111-geo-id-693-population-group-54074999.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/idps_somalia_download-som-unhcr-prmn-displacement-dataset.xlsx` & `hdx_python_scraper-2.1.7/tests/fixtures/idps_somalia_download-som-unhcr-prmn-displacement-dataset.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/ipc_somalia_download-som-food-insecurity-oct-dec2022-projection.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/ipc_somalia_download-som-food-insecurity-oct-dec2022-projection.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/kenya-drought-related-key-figures.json` & `hdx_python_scraper-2.1.7/tests/fixtures/kenya-drought-related-key-figures.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/kenya-pin-targeted-reached-by-location-and-cluster.json` & `hdx_python_scraper-2.1.7/tests/fixtures/kenya-pin-targeted-reached-by-location-and-cluster.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/key_figures_eth_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/key_figures_eth_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/key_figures_ken_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/key_figures_ken_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/key_figures_som_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/key_figures_som_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/ourworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/ourworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/ourworldindata_other_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/ourworldindata_other_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/population.json` & `hdx_python_scraper-2.1.7/tests/fixtures/population.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/population_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls` & `hdx_python_scraper-2.1.7/tests/fixtures/population_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/population_other_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls` & `hdx_python_scraper-2.1.7/tests/fixtures/population_other_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/regions_download-tbl-regcov-2020-ocha.xlsx` & `hdx_python_scraper-2.1.7/tests/fixtures/regions_download-tbl-regcov-2020-ocha.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/sadd_covid-data-dataset-fullvars-extype-csv.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/sadd_covid-data-dataset-fullvars-extype-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/sahel-humanitarian-needs-overview.json` & `hdx_python_scraper-2.1.7/tests/fixtures/sahel-humanitarian-needs-overview.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/somalia-acute-food-insecurity-country-data.json` & `hdx_python_scraper-2.1.7/tests/fixtures/somalia-acute-food-insecurity-country-data.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/somalia-drought-related-key-figures.json` & `hdx_python_scraper-2.1.7/tests/fixtures/somalia-drought-related-key-figures.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/somalia-internally-displaced-persons-idps.json` & `hdx_python_scraper-2.1.7/tests/fixtures/somalia-internally-displaced-persons-idps.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/somalia-pin-targeted-reached-by-location-and-cluster.json` & `hdx_python_scraper-2.1.7/tests/fixtures/somalia-pin-targeted-reached-by-location-and-cluster.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/test_output.xlsx` & `hdx_python_scraper-2.1.7/tests/fixtures/test_output.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/timeseries_casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/timeseries_casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/total-covid-19-tests-performed-by-country.json` & `hdx_python_scraper-2.1.7/tests/fixtures/total-covid-19-tests-performed-by-country.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/ukraine-border-crossings.json` & `hdx_python_scraper-2.1.7/tests/fixtures/ukraine-border-crossings.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/ukraine-who-does-what-where-3w.json` & `hdx_python_scraper-2.1.7/tests/fixtures/ukraine-who-does-what-where-3w.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/unocha-office-locations.json` & `hdx_python_scraper-2.1.7/tests/fixtures/unocha-office-locations.json`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/who_national2_who-covid-19-global-data.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/who_national2_who-covid-19-global-data.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/who_national_who-covid-19-global-data.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/who_national_who-covid-19-global-data.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/fixtures/whowhatwhere_afg_3w_data.csv` & `hdx_python_scraper-2.1.7/tests/fixtures/whowhatwhere_afg_3w_data.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/hdx/scraper/__init__.py` & `hdx_python_scraper-2.1.7/tests/hdx/scraper/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/hdx/scraper/affected_targeted_reached.py` & `hdx_python_scraper-2.1.7/tests/hdx/scraper/affected_targeted_reached.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import logging
 
+from hdx.scraper.base_scraper import BaseScraper
+from hdx.scraper.utilities.sources import Sources
 from hdx.utilities.dateparse import default_date
 from hdx.utilities.dictandlist import dict_of_lists_add
 from hdx.utilities.text import number_format
 
-from hdx.scraper.base_scraper import BaseScraper
-from hdx.scraper.utilities.sources import Sources
-
 logger = logging.getLogger(__name__)
 
 
 class AffectedTargetedReached(BaseScraper):
     def __init__(self, datasetinfo, today, adminone, admintwo):
         super().__init__(
             "affected_targeted_reached",
```

### Comparing `hdx-python-scraper-2.1.6/tests/hdx/scraper/conftest.py` & `hdx_python_scraper-2.1.7/tests/hdx/scraper/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 """Global fixtures"""
 from os.path import join
 
 import pytest
+
+from . import bool_assert
 from hdx.api.configuration import Configuration
 from hdx.api.locations import Locations
 from hdx.location.country import Country
-from hdx.utilities.dateparse import parse_date
-
 from hdx.scraper.base_scraper import BaseScraper
 from hdx.scraper.utilities import string_params_to_dict
 from hdx.scraper.utilities.fallbacks import Fallbacks
 from hdx.scraper.utilities.reader import Read
-
-from . import bool_assert
+from hdx.utilities.dateparse import parse_date
 
 
 @pytest.fixture(scope="session")
 def fixtures():
     return join("tests", "fixtures")
 
 
 @pytest.fixture(scope="session")
 def configuration(fixtures):
     Configuration._create(
         hdx_read_only=True,
         hdx_site="prod",
         user_agent="test",
         project_config_yaml=join(
-            "tests", "config", "project_configuration.yml"
+            "tests", "config", "project_configuration.yaml"
         ),
     )
     Locations.set_validlocations(
         [
             {"name": "afg", "title": "Afghanistan"},
             {"name": "phl", "title": "Philippines"},
             {"name": "pse", "title": "State of Palestine"},
```

### Comparing `hdx-python-scraper-2.1.6/tests/hdx/scraper/education_closures.py` & `hdx_python_scraper-2.1.7/tests/hdx/scraper/education_closures.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 from typing import Dict
 
-from hdx.utilities.dateparse import default_date, parse_date
-
 from hdx.scraper.base_scraper import BaseScraper
+from hdx.utilities.dateparse import default_date, parse_date
 
 logger = logging.getLogger(__name__)
 
 
 class EducationClosures(BaseScraper):
     def __init__(self, datasetinfo: Dict, today, countryiso3s, regionlookup):
         super().__init__(
```

### Comparing `hdx-python-scraper-2.1.6/tests/hdx/scraper/education_enrolment.py` & `hdx_python_scraper-2.1.7/tests/hdx/scraper/education_enrolment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 
-from hdx.utilities.text import get_fraction_str
-
 from hdx.scraper.base_scraper import BaseScraper
+from hdx.utilities.text import get_fraction_str
 
 logger = logging.getLogger(__name__)
 
 
 class EducationEnrolment(BaseScraper):
     def __init__(self, datasetinfo, closures, countryiso3s, regionlookup):
         super().__init__(
```

### Comparing `hdx-python-scraper-2.1.6/tests/hdx/scraper/test_output.py` & `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_output.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import filecmp
 from os import getenv
 from os.path import join
 
 import numpy as np
 import pandas
 import pytest
-from hdx.utilities.path import temp_dir
 
 from hdx.scraper.outputs.base import BaseOutput
 from hdx.scraper.outputs.excelfile import ExcelFile
 from hdx.scraper.outputs.googlesheets import GoogleSheets
 from hdx.scraper.outputs.json import JsonFile
+from hdx.utilities.path import temp_dir
 
 
 class TestOutput:
     @pytest.fixture(scope="class")
     def hxltags(self):
         return {
             "Country Code": "#country+code",
```

### Comparing `hdx-python-scraper-2.1.6/tests/hdx/scraper/test_readers.py` & `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_readers.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from datetime import datetime, timezone
 
 import pytest
+
 from hdx.data.dataset import Dataset
 from hdx.data.resource import Resource
+from hdx.scraper.utilities.reader import Read
 from hdx.utilities.dateparse import parse_date
 from hdx.utilities.downloader import Download
 from hdx.utilities.path import temp_dir
 
-from hdx.scraper.utilities.reader import Read
-
 
 class TestReaders:
     def test_clone(self):
         with Download(user_agent="test") as downloader:
             with Read(
                 downloader,
                 "fallback_dir",
```

### Comparing `hdx-python-scraper-2.1.6/tests/hdx/scraper/test_regionlookup.py` & `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_regionlookup.py`

 * *Files identical despite different names*

### Comparing `hdx-python-scraper-2.1.6/tests/hdx/scraper/test_runner_get_results.py` & `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_runner_get_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from hdx.utilities.dateparse import parse_date
-
+from .conftest import run_check_scrapers
 from hdx.scraper.base_scraper import BaseScraper
 from hdx.scraper.runner import Runner
-
-from .conftest import run_check_scrapers
+from hdx.utilities.dateparse import parse_date
 
 
 class TestRunnerGetResults:
     def test_get_results(self, configuration):
         BaseScraper.population_lookup = {}
         today = parse_date("2020-10-01")
```

### Comparing `hdx-python-scraper-2.1.6/tests/hdx/scraper/test_scrapers_aggregation.py` & `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_aggregation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from hdx.utilities.dateparse import parse_date
-
+from .conftest import run_check_scraper, run_check_scrapers
 from hdx.scraper.base_scraper import BaseScraper
 from hdx.scraper.runner import Runner
 from hdx.scraper.utilities.sources import Sources
-
-from .conftest import run_check_scraper, run_check_scrapers
+from hdx.utilities.dateparse import parse_date
 
 
 class TestScrapersAggregation:
     def test_get_aggregation_hxl(self, configuration):
         BaseScraper.population_lookup = {}
         today = parse_date("2020-10-01")
```

### Comparing `hdx-python-scraper-2.1.6/tests/hdx/scraper/test_scrapers_appenddata.py` & `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_appenddata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from copy import deepcopy
 
 import pytest
-from hdx.location.country import Country
-from hdx.utilities.dateparse import parse_date
 
+from .conftest import run_check_scrapers
+from hdx.location.country import Country
 from hdx.scraper.base_scraper import BaseScraper
 from hdx.scraper.outputs.json import JsonFile
 from hdx.scraper.runner import Runner
 from hdx.scraper.utilities.sources import Sources
 from hdx.scraper.utilities.writer import Writer
-
-from .conftest import run_check_scrapers
+from hdx.utilities.dateparse import parse_date
 
 
 # Test that scrapers can add to output from previous scrapers
 # Also test producing sources per admin unit eg. #targeted+total+eth
 class TestScrapersAppendData:
     @pytest.fixture
     def iso3s(self):
```

### Comparing `hdx-python-scraper-2.1.6/tests/hdx/scraper/test_scrapers_custom.py` & `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_custom.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from copy import deepcopy
 
-from hdx.location.adminlevel import AdminLevel
-from hdx.utilities.dateparse import parse_date
-
-from hdx.scraper.base_scraper import BaseScraper
-from hdx.scraper.runner import Runner
-
 from .affected_targeted_reached import AffectedTargetedReached
 from .conftest import check_scraper, check_scrapers
 from .education_closures import EducationClosures
 from .education_enrolment import EducationEnrolment
+from hdx.location.adminlevel import AdminLevel
+from hdx.scraper.base_scraper import BaseScraper
+from hdx.scraper.runner import Runner
+from hdx.utilities.dateparse import parse_date
 
 
 class TestScrapersCustom:
     def test_get_custom(self, configuration, fallbacks_json):
         BaseScraper.population_lookup = {}
         source_date = "Apr 30, 2022"
         today = parse_date("2020-10-01")
```

### Comparing `hdx-python-scraper-2.1.6/tests/hdx/scraper/test_scrapers_global.py` & `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_global.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import logging
 
 import pytest
-from hdx.utilities.dateparse import parse_date
 
+from .conftest import run_check_scraper
 from hdx.scraper.base_scraper import BaseScraper
 from hdx.scraper.runner import Runner
 from hdx.scraper.utilities.sources import Sources
-
-from .conftest import run_check_scraper
+from hdx.utilities.dateparse import parse_date
 
 
 class TestScraperGlobal:
     @pytest.fixture(scope="class")
     def cerf_headers(self):
         return (
             [
```

### Comparing `hdx-python-scraper-2.1.6/tests/hdx/scraper/test_scrapers_multipleurls.py` & `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_multipleurls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from hdx.utilities.dateparse import parse_date
-
+from .conftest import run_check_scraper
 from hdx.scraper.base_scraper import BaseScraper
 from hdx.scraper.runner import Runner
-
-from .conftest import run_check_scraper
+from hdx.utilities.dateparse import parse_date
 
 
 class TestScrapersMultipleURLs:
     def test_get_key_figures(self, configuration):
         BaseScraper.population_lookup = {}
         today = parse_date("2020-10-01")
         level = "national"
```

### Comparing `hdx-python-scraper-2.1.6/tests/hdx/scraper/test_scrapers_national.py` & `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_national.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-from hdx.utilities.dateparse import parse_date
-from hdx.utilities.errors_onexit import ErrorsOnExit
-
+from .conftest import run_check_scraper, run_check_scrapers
+from .unhcr_myanmar_idps import idps_post_run
 from hdx.scraper.base_scraper import BaseScraper
 from hdx.scraper.outputs.json import JsonFile
 from hdx.scraper.runner import Runner
 from hdx.scraper.utilities.reader import Read
 from hdx.scraper.utilities.writer import Writer
-
-from .conftest import run_check_scraper, run_check_scrapers
-from .unhcr_myanmar_idps import idps_post_run
+from hdx.utilities.dateparse import parse_date
+from hdx.utilities.errors_onexit import ErrorsOnExit
 
 
 class TestScrapersNational:
     def test_get_national_afg(self, configuration):
         BaseScraper.population_lookup = {}
         today = parse_date("2020-10-01")
         level = "national"
```

### Comparing `hdx-python-scraper-2.1.6/tests/hdx/scraper/test_scrapers_regionaltoplevel.py` & `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_regionaltoplevel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-from hdx.utilities.dateparse import parse_date
-
+from .conftest import run_check_scraper, run_check_scrapers
 from hdx.scraper.base_scraper import BaseScraper
 from hdx.scraper.outputs.json import JsonFile
 from hdx.scraper.runner import Runner
 from hdx.scraper.utilities.sources import Sources
 from hdx.scraper.utilities.writer import Writer
-
-from .conftest import run_check_scraper, run_check_scrapers
+from hdx.utilities.dateparse import parse_date
 
 
 class TestScrapersRegionalToplevel:
     access_national_headers = (
         [
             "% of visas pending or denied",
             "% of travel authorizations or movements denied",
```

### Comparing `hdx-python-scraper-2.1.6/tests/hdx/scraper/test_scrapers_resource_downloaders.py` & `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_resource_downloaders.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from os.path import exists, join
 
 import pytest
-from hdx.utilities.dateparse import parse_date
-from hdx.utilities.path import temp_dir
 
 from hdx.scraper.base_scraper import BaseScraper
 from hdx.scraper.runner import Runner
+from hdx.utilities.dateparse import parse_date
+from hdx.utilities.path import temp_dir
 
 
 class TestScrapersResourceDownloader:
     @pytest.fixture(scope="function")
     def output_file(self, fixtures):
         return join(fixtures, "test_output.xlsx")
```

### Comparing `hdx-python-scraper-2.1.6/tests/hdx/scraper/test_scrapers_subnational.py` & `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_subnational.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
+from .conftest import run_check_scraper
 from hdx.location.adminlevel import AdminLevel
-from hdx.utilities.dateparse import parse_date
-
 from hdx.scraper.base_scraper import BaseScraper
 from hdx.scraper.outputs.json import JsonFile
 from hdx.scraper.runner import Runner
 from hdx.scraper.utilities.writer import Writer
-
-from .conftest import run_check_scraper
+from hdx.utilities.dateparse import parse_date
 
 
 class TestScrapersSubnational:
     def test_get_subnational(self, configuration):
         BaseScraper.population_lookup = {}
         today = parse_date("2020-10-01")
         adminlevel = AdminLevel(configuration)
```

### Comparing `hdx-python-scraper-2.1.6/tests/hdx/scraper/test_scrapers_timeseries.py` & `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_timeseries.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from hdx.utilities.dateparse import parse_date
-
 from hdx.scraper.base_scraper import BaseScraper
 from hdx.scraper.outputs.json import JsonFile
 from hdx.scraper.runner import Runner
+from hdx.utilities.dateparse import parse_date
 
 
 class TestScrapersTimeSeries:
     def test_timeseries(self, configuration):
         BaseScraper.population_lookup = {}
         iso3s = ("AFG", "MMR")
         today = parse_date("2022-03-06")
```

### Comparing `hdx-python-scraper-2.1.6/tests/hdx/scraper/test_sources.py` & `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_sources.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
-from hdx.location.adminlevel import AdminLevel
-from hdx.utilities.dateparse import parse_date
 
+from hdx.location.adminlevel import AdminLevel
 from hdx.scraper.base_scraper import BaseScraper
 from hdx.scraper.configurable.scraper import ConfigurableScraper
 from hdx.scraper.utilities.sources import Sources
+from hdx.utilities.dateparse import parse_date
 
 
 class TestSources:
     @pytest.fixture(scope="class")
     def startdate(self):
         return parse_date("2021-09-23")
```

### Comparing `hdx-python-scraper-2.1.6/tests/hdx/scraper/unhcr_myanmar_idps.py` & `hdx_python_scraper-2.1.7/tests/hdx/scraper/unhcr_myanmar_idps.py`

 * *Files identical despite different names*

