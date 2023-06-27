# Comparing `tmp/Titan_Client-1.19.7.tar.gz` & `tmp/Titan_Client-1.19.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Titan Client-1.19.7.tar", last modified: Wed Jun  7 11:34:18 2023, max compression
+gzip compressed data, was "Titan Client-1.19.7.1.tar", last modified: Tue Jun 27 09:23:20 2023, max compression
```

## Comparing `Titan_Client-1.19.7.tar` & `Titan_Client-1.19.7.1.tar`

### file list

```diff
@@ -1,410 +1,410 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:34:18.302255 Titan Client-1.19.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-07 11:34:06.000000 Titan Client-1.19.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 11:34:06.000000 Titan Client-1.19.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-07 11:34:18.302255 Titan Client-1.19.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40576 2023-06-07 11:34:06.000000 Titan Client-1.19.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:34:18.206254 Titan Client-1.19.7/Titan_Client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-07 11:34:18.000000 Titan Client-1.19.7/Titan_Client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21824 2023-06-07 11:34:18.000000 Titan Client-1.19.7/Titan_Client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 11:34:18.000000 Titan Client-1.19.7/Titan_Client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-07 11:34:18.000000 Titan Client-1.19.7/Titan_Client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 11:34:18.000000 Titan Client-1.19.7/Titan_Client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 11:34:06.000000 Titan Client-1.19.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-07 11:34:18.302255 Titan Client-1.19.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-07 11:34:06.000000 Titan Client-1.19.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:34:18.206254 Titan Client-1.19.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-06-07 11:34:06.000000 Titan Client-1.19.7/test/test_api_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-07 11:34:06.000000 Titan Client-1.19.7/test/test_stix_mappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:34:18.206254 Titan Client-1.19.7/titan_client/
--rw-r--r--   0 runner    (1001) docker     (123)    42448 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:34:18.214254 Titan Client-1.19.7/titan_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29789 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api/actors_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23104 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api/alerts_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   185921 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api/credentials_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24251 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api/entities_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    41022 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api/events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    38360 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api/forums_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21583 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api/girs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    60498 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api/global_search_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    42887 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api/indicators_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24139 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api/iocs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22531 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api/malware_families_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    88638 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api/marketplaces_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27146 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api/messaging_services_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29583 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api/news_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24920 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api/pcap_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   110246 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api/reports_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19090 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api/tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33416 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api/vulnerabilities_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    82194 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api/watchers_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27806 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api/yara_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    40253 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29460 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17600 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:34:18.302255 Titan Client-1.19.7/titan_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    40882 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/actors_get412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    31424 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/alert_list_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17229 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/alert_list_schema_chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17793 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/alert_list_schema_highlights.py
--rw-r--r--   0 runner    (1001) docker     (123)    17913 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/alert_list_schema_highlights_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/alert_list_schema_highlights_inner_chunks_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    23973 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/alert_list_schema_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    18895 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/alert_list_schema_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/alert_subscription_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/alert_subscription_subscribe_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/alerts_get412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/breach_alerts_get412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    20683 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_accessed_url_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17847 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_accessed_url_schema_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17099 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_accessed_url_schema_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    18782 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_accessed_url_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    21156 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_accessed_url_schema_data_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    20827 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_accessed_url_stream_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    20483 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_accessed_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    21576 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_accessed_urls_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    20642 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_occurrence_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17827 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_occurrence_schema_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_occurrence_schema_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    20409 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_occurrence_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    21985 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_occurrence_schema_data_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    17661 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_occurrence_schema_data_credential_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    20328 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_occurrences_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    21399 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_occurrences_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    21061 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17663 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_schema_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    16985 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_schema_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17400 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_schema_data_credential_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)    17460 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_schema_data_credential_sets_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    19326 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_schema_data_password.py
--rw-r--r--   0 runner    (1001) docker     (123)    25719 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_schema_data_password_complexity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_schema_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    20798 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_set_accessed_url_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17899 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_set_accessed_url_schema_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_set_accessed_url_schema_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    18932 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_set_accessed_url_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17863 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_set_accessed_url_schema_data_credential_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    20960 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_set_accessed_url_stream_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    19193 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_set_accessed_url_stream_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    21197 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_set_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_set_schema_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17017 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_set_schema_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    24170 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_set_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17433 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_set_schema_data_external_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)    17493 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_set_schema_data_external_sources_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    17433 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_set_schema_data_internal_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)    17493 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_set_schema_data_internal_sources_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    17529 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_set_schema_data_victims.py
--rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_set_schema_data_victims_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    19565 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_set_schema_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_set_stream_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    24564 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_set_stream_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    20892 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_sets_accessed_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    22001 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_sets_accessed_urls_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_sets_get412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_sets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15869 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_sets_stream_get412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    20780 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credential_sets_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15833 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credentials_get412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    19390 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credentials_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15857 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credentials_stream_get412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    20421 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/credentials_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/cve_reports_get412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    19022 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/entities_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    21556 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/entities_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/entities_schema_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/entities_schema_links_actors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17580 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/entities_schema_links_actors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    24491 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/entities_schema_links_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    24671 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/entities_schema_links_reports_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    19997 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/event_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17583 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/event_schema_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    20713 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/event_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    32498 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/event_schema_data_event_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    18204 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    20083 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_controller_geo_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    19464 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_controller_geo_ip_isp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16616 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16656 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_controllers_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    18426 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_encryption_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    21139 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    17522 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_recipient_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_recipient_domains_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16712 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_triggers_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    18257 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/event_schema_data_threat.py
--rw-r--r--   0 runner    (1001) docker     (123)    19515 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/event_schema_data_threat_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16701 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/event_schema_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    19898 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/event_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    18908 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/events_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/events_stream_get412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    19538 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/full_breach_alert_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/full_breach_alert_schema_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/full_breach_alert_schema_all_of_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16751 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/full_breach_alert_schema_all_of_data_breach_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    20179 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/full_cve_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    18463 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/full_news_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    41733 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/full_report_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    19863 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/full_report_schema_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    19499 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/full_spot_report_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    22800 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/full_watcher_group_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17039 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/full_watcher_group_schema_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    17455 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/full_watcher_group_schema_all_of_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    18297 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/full_watcher_group_schema_all_of_links_forum.py
--rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/full_watcher_group_schema_all_of_links_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    17799 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/full_watcher_group_schema_all_of_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)    20464 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/full_watcher_group_schema_all_of_watchers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17315 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/gir_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    16542 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/gir_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    19483 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/gir_schema_data_gir.py
--rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/girs_get412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/girs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    19352 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/indicator_search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    19878 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/indicator_search_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17719 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/indicator_search_schema_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    26097 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/indicator_search_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16973 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/indicator_search_schema_data_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/indicator_search_schema_data_indicator_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    21604 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/indicator_search_schema_data_indicator_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    18597 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/indicator_search_schema_data_threat.py
--rw-r--r--   0 runner    (1001) docker     (123)    19699 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/indicator_search_schema_data_threat_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16771 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/indicator_search_schema_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    20280 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/indicator_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    17345 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/inline_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/inline_object1.py
--rw-r--r--   0 runner    (1001) docker     (123)    18643 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/instant_message_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/instant_message_schema_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    19490 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/instant_message_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17583 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/instant_message_schema_data_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20160 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/instant_message_schema_data_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    20642 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/instant_message_schema_data_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    21496 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/instant_message_schema_data_message_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)    21636 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/instant_message_schema_data_message_attachments_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    18537 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/instant_message_schema_data_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    23556 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/ioc_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    20173 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/ioc_schema_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    17468 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/ioc_schema_links_actors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17528 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/ioc_schema_links_actors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    24277 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/ioc_schema_links_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    24457 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/ioc_schema_links_reports_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    18782 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/iocs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    16607 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/malware.py
--rw-r--r--   0 runner    (1001) docker     (123)    15849 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/malware_families_get412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    18301 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/malware_family_search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    18785 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/malware_family_search_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17787 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/malware_family_search_schema_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/malware_pcaps_get412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    19787 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/malware_reports_search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    21472 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/malware_reports_search_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17799 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/malware_reports_search_schema_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/malware_reports_search_schema_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/malware_reports_search_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/malware_reports_search_schema_data_malware_report_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/malware_reports_search_schema_data_malware_report_data_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)    21365 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/malware_reports_search_schema_data_malware_report_data_attachments_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/malware_reports_search_schema_data_threat.py
--rw-r--r--   0 runner    (1001) docker     (123)    18948 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/malware_reports_search_schema_data_threat_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16020 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_product_availability_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    22379 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_product_credential_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    18356 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_product_credential_schema_victim.py
--rw-r--r--   0 runner    (1001) docker     (123)    22905 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_product_credit_card_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    21843 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_product_credit_card_schema_victim.py
--rw-r--r--   0 runner    (1001) docker     (123)    18478 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_product_marketplace_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    21254 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_product_other_product_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    20165 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_product_search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_product_search_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17835 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_product_search_schema_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    27624 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_product_search_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    20041 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_product_statistics_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    21135 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_product_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    16063 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_product_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    19368 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_resource_search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    19743 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_resource_search_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17835 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_resource_search_schema_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    22539 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_resource_search_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    20342 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_resource_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    19417 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    20543 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_search_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_search_schema_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    19847 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_search_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    18429 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_search_schema_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19198 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_vendor_search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    20731 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_vendor_search_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17803 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_vendor_search_schema_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    19487 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_vendor_search_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17215 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_vendor_search_schema_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    20160 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplace_vendor_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15893 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/marketplaces_products_stream_get412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/messaging_services_instant_messages_get412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    19788 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/messaging_services_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    18399 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/news_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17563 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/news_schema_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    20897 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/news_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    20447 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/news_schema_data_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)    20567 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/news_schema_data_attachments_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    17599 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/pcap_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    18013 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/pcap_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17931 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/pcap_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17443 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/pcap_schema_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17344 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/pcap_schema_data_malware_family.py
--rw-r--r--   0 runner    (1001) docker     (123)    17343 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/pcap_schema_data_pcap.py
--rw-r--r--   0 runner    (1001) docker     (123)    21293 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/post_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    18951 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/post_schema_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    17609 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/post_schema_links_author_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18340 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/post_schema_links_forum.py
--rw-r--r--   0 runner    (1001) docker     (123)    19481 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/post_schema_links_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    18821 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/posts_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    23470 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/private_message_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    20686 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/private_message_schema_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    17581 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/private_message_schema_links_author_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18500 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/private_message_schema_links_forum.py
--rw-r--r--   0 runner    (1001) docker     (123)    17629 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/private_message_schema_links_recipient_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16743 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/private_message_schema_links_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    19740 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/private_messages_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15817 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/reports_get412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    57979 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/search_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    20777 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_actor_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    28965 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_actor_schema_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    17916 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_actor_schema_links_contact_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_actor_schema_links_forums.py
--rw-r--r--   0 runner    (1001) docker     (123)    20473 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_actor_schema_links_forums_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_actor_schema_links_forums_inner_contact_info_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    18806 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_actor_schema_links_instant_message_servers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18886 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_actor_schema_links_instant_message_servers_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    19022 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_actors_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    19337 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_breach_alert_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    19569 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17755 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    26767 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_breach_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_breach_alert_confidence.py
--rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_breach_alert_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)    21480 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_breach_alert_sources_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    22080 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_breach_alert_victim.py
--rw-r--r--   0 runner    (1001) docker     (123)    18097 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_breach_alert_victim_industries.py
--rw-r--r--   0 runner    (1001) docker     (123)    18157 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_breach_alert_victim_industries_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    19485 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19624 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_entities_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_entities_inner_geo_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    17885 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_geo_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    20227 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_cve_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17631 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_cve_schema_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    16923 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_cve_schema_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_cve_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    38975 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_activity_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    17863 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_counter_measure_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    17923 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_counter_measure_links_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_cvss_score.py
--rw-r--r--   0 runner    (1001) docker     (123)    19925 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_exploit_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_interest_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    17719 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_patch_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    17779 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_patch_links_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    17739 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_poc_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    17799 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_poc_links_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    17711 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_titan_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    17771 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_titan_links_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    19202 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_cves_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    17650 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_news_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    37959 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_report_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17722 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_report_schema_actor_subject_of_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    17782 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_report_schema_actor_subject_of_report_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    16946 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_report_schema_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    17438 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_report_schema_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)    17498 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_report_schema_entities_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_report_schema_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)    18496 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_report_schema_locations_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    17931 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_report_schema_related_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_report_schema_related_reports_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    21844 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_report_schema_report_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)    21985 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_report_schema_report_attachments_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    19449 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_report_schema_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)    19549 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_report_schema_sources_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    17481 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_report_schema_victims.py
--rw-r--r--   0 runner    (1001) docker     (123)    17541 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_report_schema_victims_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_reports_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    19539 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_spot_report_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17739 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_spot_report_schema_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17814 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_spot_report_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17689 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_spot_report_schema_data_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)    17749 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_spot_report_schema_data_entities_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    17853 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_spot_report_schema_data_spot_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    27046 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_spot_report_schema_data_spot_report_spot_report_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    18971 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_spot_report_schema_data_spot_report_spot_report_data_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    19051 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_spot_report_schema_data_spot_report_spot_report_data_links_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    17871 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_spot_report_schema_data_spot_report_spot_report_data_victims.py
--rw-r--r--   0 runner    (1001) docker     (123)    17931 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_spot_report_schema_data_spot_report_spot_report_data_victims_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    19284 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_spot_reports_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    21678 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/simple_watcher_group_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    19470 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/situation_report_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    20621 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/situation_report_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17438 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/situation_report_schema_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17041 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/situation_report_schema_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    16830 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/situation_report_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    24241 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/situation_report_schema_data_situation_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    17848 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/situation_report_schema_data_situation_report_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)    17909 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/situation_report_schema_data_situation_report_entities_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/situation_report_schema_data_situation_report_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    16953 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/situation_report_schema_data_situation_report_link_malware_family.py
--rw-r--r--   0 runner    (1001) docker     (123)    16953 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/situation_report_schema_data_situation_report_link_malware_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    17724 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/situation_report_schema_data_situation_report_victims.py
--rw-r--r--   0 runner    (1001) docker     (123)    17785 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/situation_report_schema_data_situation_report_victims_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    18643 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    18653 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/tag_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    18142 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_group_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_groups_get412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    17478 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_groups_get_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_groups_group_uid_delete_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    18344 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_groups_group_uid_put_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_groups_group_uid_watchers_get412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_groups_group_uid_watchers_post412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_groups_post412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    17490 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_groups_post_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    28573 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_request_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    17419 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_request_body_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    17479 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_request_body_filters_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    17479 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_request_body_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)    17539 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_request_body_patterns_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    30068 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_request_body_post.py
--rw-r--r--   0 runner    (1001) docker     (123)    17180 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_request_body_post_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    30702 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_request_body_put.py
--rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_request_body_put_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    28296 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17561 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_schema_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    17621 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_schema_filters_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    18294 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_schema_forum.py
--rw-r--r--   0 runner    (1001) docker     (123)    17484 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_schema_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_schema_links_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_schema_links_inner_forum.py
--rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_schema_links_inner_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    17617 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_schema_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)    17677 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_schema_patterns_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    17825 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_schema_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    17495 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/watcher_schema_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/yara_search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    20158 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/yara_search_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17639 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/yara_search_schema_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    19921 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/yara_search_schema_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    18512 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/yara_search_schema_data_threat.py
--rw-r--r--   0 runner    (1001) docker     (123)    18796 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/yara_search_schema_data_threat_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17447 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/yara_search_schema_data_yara_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16727 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/models/yara_search_schema_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    25361 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:34:18.302255 Titan Client-1.19.7/titan_client/titan_stix/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/titan_stix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/titan_stix/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:34:18.302255 Titan Client-1.19.7/titan_client/titan_stix/mappers/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/titan_stix/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/titan_stix/mappers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/titan_stix/mappers/cves.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/titan_stix/mappers/indicators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/titan_stix/mappers/iocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/titan_stix/mappers/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/titan_stix/mappers/yara.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/titan_stix/observables.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/titan_stix/patterning.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-07 11:34:06.000000 Titan Client-1.19.7/titan_client/titan_stix/sdo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:20.022293 Titan Client-1.19.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-27 09:23:20.022293 Titan Client-1.19.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40578 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:19.934294 Titan Client-1.19.7.1/Titan_Client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-27 09:23:19.000000 Titan Client-1.19.7.1/Titan_Client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21824 2023-06-27 09:23:19.000000 Titan Client-1.19.7.1/Titan_Client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:23:19.000000 Titan Client-1.19.7.1/Titan_Client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-27 09:23:19.000000 Titan Client-1.19.7.1/Titan_Client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 09:23:19.000000 Titan Client-1.19.7.1/Titan_Client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-27 09:23:20.022293 Titan Client-1.19.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:19.934294 Titan Client-1.19.7.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/test/test_api_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/test/test_stix_mappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:19.938294 Titan Client-1.19.7.1/titan_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    42450 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:19.942294 Titan Client-1.19.7.1/titan_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29789 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api/actors_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23104 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api/alerts_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   185921 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api/credentials_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24251 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api/entities_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41022 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api/events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38360 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api/forums_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21583 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api/girs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60498 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api/global_search_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42659 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api/indicators_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24139 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api/iocs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22531 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api/malware_families_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88638 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api/marketplaces_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27146 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api/messaging_services_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29583 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api/news_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24920 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api/pcap_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110132 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api/reports_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19090 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33416 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api/vulnerabilities_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82194 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api/watchers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27692 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api/yara_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40255 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29462 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17600 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:20.018293 Titan Client-1.19.7.1/titan_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    40882 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/actors_get412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31424 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/alert_list_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17229 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/alert_list_schema_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17793 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/alert_list_schema_highlights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17913 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/alert_list_schema_highlights_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/alert_list_schema_highlights_inner_chunks_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23973 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/alert_list_schema_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18895 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/alert_list_schema_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/alert_subscription_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/alert_subscription_subscribe_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/alerts_get412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/breach_alerts_get412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20683 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_accessed_url_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17847 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_accessed_url_schema_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17099 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_accessed_url_schema_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18782 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_accessed_url_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21156 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_accessed_url_schema_data_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20827 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_accessed_url_stream_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20483 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_accessed_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21576 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_accessed_urls_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20642 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_occurrence_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17827 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_occurrence_schema_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_occurrence_schema_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20409 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_occurrence_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21985 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_occurrence_schema_data_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17661 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_occurrence_schema_data_credential_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20328 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_occurrences_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21399 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_occurrences_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21061 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17663 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_schema_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16985 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_schema_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17400 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_schema_data_credential_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17460 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_schema_data_credential_sets_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19326 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_schema_data_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25719 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_schema_data_password_complexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_schema_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20798 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_set_accessed_url_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17899 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_set_accessed_url_schema_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_set_accessed_url_schema_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18932 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_set_accessed_url_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17863 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_set_accessed_url_schema_data_credential_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20960 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_set_accessed_url_stream_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19193 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_set_accessed_url_stream_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21197 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_set_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_set_schema_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17017 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_set_schema_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24170 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_set_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17433 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_set_schema_data_external_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17493 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_set_schema_data_external_sources_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17433 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_set_schema_data_internal_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17493 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_set_schema_data_internal_sources_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17529 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_set_schema_data_victims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_set_schema_data_victims_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19565 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_set_schema_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_set_stream_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24564 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_set_stream_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20892 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_sets_accessed_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22001 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_sets_accessed_urls_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_sets_get412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_sets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15869 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_sets_stream_get412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20780 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credential_sets_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15833 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credentials_get412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19390 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credentials_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15857 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credentials_stream_get412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20421 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/credentials_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/cve_reports_get412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19022 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/entities_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21556 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/entities_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/entities_schema_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/entities_schema_links_actors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17580 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/entities_schema_links_actors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24491 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/entities_schema_links_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24671 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/entities_schema_links_reports_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19997 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/event_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17583 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/event_schema_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20713 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/event_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32498 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18204 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20083 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_controller_geo_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19464 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_controller_geo_ip_isp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16616 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16656 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_controllers_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18426 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_encryption_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21139 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17522 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_recipient_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_recipient_domains_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16712 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_triggers_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18257 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/event_schema_data_threat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19515 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/event_schema_data_threat_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16701 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/event_schema_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19898 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/event_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18908 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/events_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/events_stream_get412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19538 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/full_breach_alert_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/full_breach_alert_schema_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/full_breach_alert_schema_all_of_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16751 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/full_breach_alert_schema_all_of_data_breach_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20179 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/full_cve_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18463 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/full_news_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41733 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/full_report_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19863 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/full_report_schema_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19499 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/full_spot_report_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22800 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/full_watcher_group_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17039 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/full_watcher_group_schema_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17455 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/full_watcher_group_schema_all_of_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18297 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/full_watcher_group_schema_all_of_links_forum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/full_watcher_group_schema_all_of_links_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17799 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/full_watcher_group_schema_all_of_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20464 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/full_watcher_group_schema_all_of_watchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17315 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/gir_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16542 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/gir_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19483 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/gir_schema_data_gir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/girs_get412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/girs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19352 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/indicator_search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19878 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/indicator_search_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17719 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/indicator_search_schema_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26097 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/indicator_search_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16973 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/indicator_search_schema_data_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/indicator_search_schema_data_indicator_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21604 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/indicator_search_schema_data_indicator_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18597 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/indicator_search_schema_data_threat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19699 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/indicator_search_schema_data_threat_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16771 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/indicator_search_schema_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20280 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/indicator_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17345 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/inline_object1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18643 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/instant_message_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/instant_message_schema_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19490 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/instant_message_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17583 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/instant_message_schema_data_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20160 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/instant_message_schema_data_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20642 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/instant_message_schema_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21496 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/instant_message_schema_data_message_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21636 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/instant_message_schema_data_message_attachments_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18537 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/instant_message_schema_data_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23556 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/ioc_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20173 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/ioc_schema_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17468 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/ioc_schema_links_actors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17528 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/ioc_schema_links_actors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24277 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/ioc_schema_links_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24457 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/ioc_schema_links_reports_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18782 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/iocs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16607 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/malware.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15849 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/malware_families_get412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18301 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/malware_family_search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18785 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/malware_family_search_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17787 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/malware_family_search_schema_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/malware_pcaps_get412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19787 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/malware_reports_search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21472 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/malware_reports_search_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17799 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/malware_reports_search_schema_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/malware_reports_search_schema_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/malware_reports_search_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/malware_reports_search_schema_data_malware_report_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/malware_reports_search_schema_data_malware_report_data_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21365 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/malware_reports_search_schema_data_malware_report_data_attachments_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/malware_reports_search_schema_data_threat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18948 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/malware_reports_search_schema_data_threat_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16020 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_product_availability_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22379 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_product_credential_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18356 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_product_credential_schema_victim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22905 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_product_credit_card_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21843 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_product_credit_card_schema_victim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18478 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_product_marketplace_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21254 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_product_other_product_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20165 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_product_search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_product_search_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17835 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_product_search_schema_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27624 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_product_search_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20041 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_product_statistics_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21135 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_product_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16063 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_product_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19368 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_resource_search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19743 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_resource_search_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17835 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_resource_search_schema_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22539 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_resource_search_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20342 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_resource_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19417 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20543 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_search_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_search_schema_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19847 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_search_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18429 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_search_schema_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19198 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_vendor_search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20731 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_vendor_search_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17803 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_vendor_search_schema_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19487 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_vendor_search_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17215 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_vendor_search_schema_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20160 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplace_vendor_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15893 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/marketplaces_products_stream_get412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/messaging_services_instant_messages_get412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19788 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/messaging_services_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18399 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/news_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17563 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/news_schema_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20897 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/news_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20447 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/news_schema_data_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20567 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/news_schema_data_attachments_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17599 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/pcap_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18013 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/pcap_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17931 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/pcap_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17443 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/pcap_schema_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17344 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/pcap_schema_data_malware_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17343 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/pcap_schema_data_pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21293 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/post_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18951 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/post_schema_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17609 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/post_schema_links_author_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18340 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/post_schema_links_forum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19481 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/post_schema_links_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18821 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/posts_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23470 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/private_message_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20686 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/private_message_schema_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17581 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/private_message_schema_links_author_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18500 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/private_message_schema_links_forum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17629 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/private_message_schema_links_recipient_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16743 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/private_message_schema_links_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19740 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/private_messages_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15817 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/reports_get412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57979 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/search_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20777 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_actor_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28965 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_actor_schema_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17916 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_actor_schema_links_contact_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_actor_schema_links_forums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20473 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_actor_schema_links_forums_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_actor_schema_links_forums_inner_contact_info_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18806 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_actor_schema_links_instant_message_servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18886 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_actor_schema_links_instant_message_servers_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19022 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_actors_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19337 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19569 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17755 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26767 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_breach_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_breach_alert_confidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_breach_alert_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21480 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_breach_alert_sources_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22080 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_breach_alert_victim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18097 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_breach_alert_victim_industries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18157 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_breach_alert_victim_industries_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19485 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19624 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_entities_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_entities_inner_geo_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17885 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_geo_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20227 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_cve_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17631 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16923 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38975 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_activity_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17863 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_counter_measure_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17923 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_counter_measure_links_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_cvss_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19925 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_exploit_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_interest_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17719 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_patch_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17779 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_patch_links_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17739 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_poc_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17799 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_poc_links_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17711 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_titan_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17771 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_titan_links_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19202 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_cves_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17650 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_news_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37959 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_report_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17722 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_report_schema_actor_subject_of_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17782 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_report_schema_actor_subject_of_report_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16946 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_report_schema_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17438 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_report_schema_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17498 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_report_schema_entities_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_report_schema_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18496 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_report_schema_locations_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17931 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_report_schema_related_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_report_schema_related_reports_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21844 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_report_schema_report_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21985 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_report_schema_report_attachments_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19449 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_report_schema_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19549 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_report_schema_sources_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17481 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_report_schema_victims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17541 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_report_schema_victims_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_reports_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19539 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17739 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17814 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17689 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema_data_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17749 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema_data_entities_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17853 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema_data_spot_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27046 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema_data_spot_report_spot_report_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18971 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema_data_spot_report_spot_report_data_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19051 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema_data_spot_report_spot_report_data_links_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17871 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema_data_spot_report_spot_report_data_victims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17931 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema_data_spot_report_spot_report_data_victims_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19284 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_spot_reports_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21678 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/simple_watcher_group_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19470 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/situation_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20621 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/situation_report_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17438 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/situation_report_schema_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17041 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/situation_report_schema_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16830 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/situation_report_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24241 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/situation_report_schema_data_situation_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17848 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/situation_report_schema_data_situation_report_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17909 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/situation_report_schema_data_situation_report_entities_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/situation_report_schema_data_situation_report_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16953 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/situation_report_schema_data_situation_report_link_malware_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16953 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/situation_report_schema_data_situation_report_link_malware_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17724 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/situation_report_schema_data_situation_report_victims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17785 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/situation_report_schema_data_situation_report_victims_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18643 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18653 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/tag_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18142 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_groups_get412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17478 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_groups_get_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_groups_group_uid_delete_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18344 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_groups_group_uid_put_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_groups_group_uid_watchers_get412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_groups_group_uid_watchers_post412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_groups_post412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17490 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_groups_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28573 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17419 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_request_body_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17479 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_request_body_filters_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17479 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_request_body_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17539 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_request_body_patterns_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30068 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_request_body_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17180 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_request_body_post_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30702 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_request_body_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_request_body_put_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28296 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17561 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_schema_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17621 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_schema_filters_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18294 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_schema_forum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17484 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_schema_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_schema_links_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_schema_links_inner_forum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_schema_links_inner_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17617 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_schema_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17677 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_schema_patterns_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17825 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_schema_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17495 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/watcher_schema_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/yara_search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20158 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/yara_search_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17639 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/yara_search_schema_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19921 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/yara_search_schema_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18512 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/yara_search_schema_data_threat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18796 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/yara_search_schema_data_threat_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17447 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/yara_search_schema_data_yara_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16727 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/models/yara_search_schema_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25361 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:20.022293 Titan Client-1.19.7.1/titan_client/titan_stix/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/titan_stix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/titan_stix/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:23:20.022293 Titan Client-1.19.7.1/titan_client/titan_stix/mappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/titan_stix/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/titan_stix/mappers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/titan_stix/mappers/cves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/titan_stix/mappers/indicators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/titan_stix/mappers/iocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/titan_stix/mappers/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/titan_stix/mappers/yara.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/titan_stix/observables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/titan_stix/patterning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-27 09:23:07.000000 Titan Client-1.19.7.1/titan_client/titan_stix/sdo.py
```

### Comparing `Titan Client-1.19.7/LICENSE` & `Titan Client-1.19.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/README.md` & `Titan Client-1.19.7.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Titan Python Client
 
 Official low-level client for Intel 471's Titan API. It aims at providing common ground for all the endpoints in Python.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.19.7
-- Package version: 1.19.7
+- Package version: 1.19.7.1
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 
 ## Requirements.
 
 Python >= 3.6 
 
 ## Installation & Usage
```

### Comparing `Titan Client-1.19.7/Titan_Client.egg-info/SOURCES.txt` & `Titan Client-1.19.7.1/Titan_Client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/setup.py` & `Titan Client-1.19.7.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # coding: utf-8
 
 """
     Titan API v1
 
     Official low-level client for Intel 471's Titan API. It aims at providing common ground for all the endpoints in Python.
 
-    The version of the OpenAPI document: 1.19.7
+    The version of the OpenAPI document: 1.19.7.1
     Generated by: https://openapi-generator.tech
 """
 
 from pkg_resources import parse_requirements
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "Titan Client"
-VERSION = "1.19.7"
+VERSION = "1.19.7.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `Titan Client-1.19.7/test/test_api_responses.py` & `Titan Client-1.19.7.1/test/test_api_responses.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/test/test_stix_mappers.py` & `Titan Client-1.19.7.1/test/test_stix_mappers.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/__init__.py` & `Titan Client-1.19.7.1/titan_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 1.19.7
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.19.7"
+__version__ = "1.19.7.1"
 
 # import apis into sdk package
 from titan_client.api.actors_api import ActorsApi
 from titan_client.api.alerts_api import AlertsApi
 from titan_client.api.credentials_api import CredentialsApi
 from titan_client.api.entities_api import EntitiesApi
 from titan_client.api.events_api import EventsApi
```

### Comparing `Titan Client-1.19.7/titan_client/api/__init__.py` & `Titan Client-1.19.7.1/titan_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/api/actors_api.py` & `Titan Client-1.19.7.1/titan_client/api/actors_api.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/api/alerts_api.py` & `Titan Client-1.19.7.1/titan_client/api/alerts_api.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/api/credentials_api.py` & `Titan Client-1.19.7.1/titan_client/api/credentials_api.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/api/entities_api.py` & `Titan Client-1.19.7.1/titan_client/api/entities_api.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/api/events_api.py` & `Titan Client-1.19.7.1/titan_client/api/events_api.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/api/forums_api.py` & `Titan Client-1.19.7.1/titan_client/api/forums_api.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/api/girs_api.py` & `Titan Client-1.19.7.1/titan_client/api/girs_api.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/api/global_search_api.py` & `Titan Client-1.19.7.1/titan_client/api/global_search_api.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/api/indicators_api.py` & `Titan Client-1.19.7.1/titan_client/api/indicators_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         >>> thread = api.indicators_get(async_req=True)
         >>> result = thread.get()
 
         :param indicator: Free text indicator search (all fields included).
         :type indicator: str
         :param indicator_type: Search indicators by type (e.g. `file`, `ipv4`, `url`).
         :type indicator_type: str
-        :param threat_type: Search indicators by threat type (e.g. `malware`, `bulletproof_hosting`, `proxy_service`).
+        :param threat_type: Search indicators by threat type.
         :type threat_type: str
         :param threat_uid: Search indicators by threat UID.
         :type threat_uid: str
         :param malware_family: Search indicators by malware family (e.g. `gozi_isfb`, `smokeloader`, `trickbot`).
         :type malware_family: str
         :param malware_family_profile_uid: Search indicators by malware family profile UID. Useful for getting context for everything we have around specific malware family, for instance https://api.intel471.com/v1/search?malwareFamilyProfileUid=d073f7352b82c1b8eedda381590adced.
         :type malware_family_profile_uid: str
@@ -106,15 +106,15 @@
         >>> thread = api.indicators_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param indicator: Free text indicator search (all fields included).
         :type indicator: str
         :param indicator_type: Search indicators by type (e.g. `file`, `ipv4`, `url`).
         :type indicator_type: str
-        :param threat_type: Search indicators by threat type (e.g. `malware`, `bulletproof_hosting`, `proxy_service`).
+        :param threat_type: Search indicators by threat type.
         :type threat_type: str
         :param threat_uid: Search indicators by threat UID.
         :type threat_uid: str
         :param malware_family: Search indicators by malware family (e.g. `gozi_isfb`, `smokeloader`, `trickbot`).
         :type malware_family: str
         :param malware_family_profile_uid: Search indicators by malware family profile UID. Useful for getting context for everything we have around specific malware family, for instance https://api.intel471.com/v1/search?malwareFamilyProfileUid=d073f7352b82c1b8eedda381590adced.
         :type malware_family_profile_uid: str
@@ -294,15 +294,15 @@
         >>> thread = api.indicators_stream_get(async_req=True)
         >>> result = thread.get()
 
         :param indicator: Free text indicator search (all fields included).
         :type indicator: str
         :param indicator_type: Search indicators by type (e.g. `file`, `ipv4`, `url`).
         :type indicator_type: str
-        :param threat_type: Search indicators by threat type (e.g. `malware`, `bulletproof_hosting`, `proxy_service`).
+        :param threat_type: Search indicators by threat type.
         :type threat_type: str
         :param threat_uid: Search indicators by threat UID.
         :type threat_uid: str
         :param malware_family: Search indicators by malware family (e.g. `gozi_isfb`, `smokeloader`, `trickbot`).
         :type malware_family: str
         :param malware_family_profile_uid: Search indicators by malware family profile UID. Useful for getting context for everything we have around specific malware family, for instance https://api.intel471.com/v1/search?malwareFamilyProfileUid=d073f7352b82c1b8eedda381590adced.
         :type malware_family_profile_uid: str
@@ -352,15 +352,15 @@
         >>> thread = api.indicators_stream_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param indicator: Free text indicator search (all fields included).
         :type indicator: str
         :param indicator_type: Search indicators by type (e.g. `file`, `ipv4`, `url`).
         :type indicator_type: str
-        :param threat_type: Search indicators by threat type (e.g. `malware`, `bulletproof_hosting`, `proxy_service`).
+        :param threat_type: Search indicators by threat type.
         :type threat_type: str
         :param threat_uid: Search indicators by threat UID.
         :type threat_uid: str
         :param malware_family: Search indicators by malware family (e.g. `gozi_isfb`, `smokeloader`, `trickbot`).
         :type malware_family: str
         :param malware_family_profile_uid: Search indicators by malware family profile UID. Useful for getting context for everything we have around specific malware family, for instance https://api.intel471.com/v1/search?malwareFamilyProfileUid=d073f7352b82c1b8eedda381590adced.
         :type malware_family_profile_uid: str
```

### Comparing `Titan Client-1.19.7/titan_client/api/iocs_api.py` & `Titan Client-1.19.7.1/titan_client/api/iocs_api.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/api/malware_families_api.py` & `Titan Client-1.19.7.1/titan_client/api/malware_families_api.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/api/marketplaces_api.py` & `Titan Client-1.19.7.1/titan_client/api/marketplaces_api.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/api/messaging_services_api.py` & `Titan Client-1.19.7.1/titan_client/api/messaging_services_api.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/api/news_api.py` & `Titan Client-1.19.7.1/titan_client/api/news_api.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/api/pcap_api.py` & `Titan Client-1.19.7.1/titan_client/api/pcap_api.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/api/reports_api.py` & `Titan Client-1.19.7.1/titan_client/api/reports_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,15 +409,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.malware_reports_get(async_req=True)
         >>> result = thread.get()
 
         :param malware_report: Free text Malware reports search (all fields included). At least one of `malwareReport`, `threatType`, `reportTitle`, `malwareFamily`, 'malwareFamilyProfileUid` is required.
         :type malware_report: str
-        :param threat_type: Search Malware reports by threat type (e.g. `malware`, `bulletproof_hosting`, `proxy_service`)
+        :param threat_type: Search Malware reports by threat type
         :type threat_type: str
         :param report_title: Search Malware reports by threat UID
         :type report_title: str
         :param malware_family: Search Malware reports by malware family (e.g. `gozi_isfb`, `smokeloader`, `trickbot`).
         :type malware_family: str
         :param malware_family_profile_uid: Search Malware reports by malware family profile UID. Useful for getting context for everything we have around specific malware family, for instance https://api.intel471.com/v1/search?malwareFamilyProfileUid=20eb1f82621001883ea0c2085aff5729.
         :type malware_family_profile_uid: str
@@ -465,15 +465,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.malware_reports_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param malware_report: Free text Malware reports search (all fields included). At least one of `malwareReport`, `threatType`, `reportTitle`, `malwareFamily`, 'malwareFamilyProfileUid` is required.
         :type malware_report: str
-        :param threat_type: Search Malware reports by threat type (e.g. `malware`, `bulletproof_hosting`, `proxy_service`)
+        :param threat_type: Search Malware reports by threat type
         :type threat_type: str
         :param report_title: Search Malware reports by threat UID
         :type report_title: str
         :param malware_family: Search Malware reports by malware family (e.g. `gozi_isfb`, `smokeloader`, `trickbot`).
         :type malware_family: str
         :param malware_family_profile_uid: Search Malware reports by malware family profile UID. Useful for getting context for everything we have around specific malware family, for instance https://api.intel471.com/v1/search?malwareFamilyProfileUid=20eb1f82621001883ea0c2085aff5729.
         :type malware_family_profile_uid: str
```

### Comparing `Titan Client-1.19.7/titan_client/api/tags_api.py` & `Titan Client-1.19.7.1/titan_client/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/api/vulnerabilities_api.py` & `Titan Client-1.19.7.1/titan_client/api/vulnerabilities_api.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/api/watchers_api.py` & `Titan Client-1.19.7.1/titan_client/api/watchers_api.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/api/yara_api.py` & `Titan Client-1.19.7.1/titan_client/api/yara_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.yara_get(async_req=True)
         >>> result = thread.get()
 
         :param yara: Free text YARA search (all fields included). At least one of `yara`, `threatType`, `threatUid`, `malwareFamily`, `malwareFamilyProfileUid` or `confidence` is required.
         :type yara: str
-        :param threat_type: Search `YARA` by threat type (e.g. `malware`, `bulletproof_hosting`, `proxy_service`)
+        :param threat_type: Search `YARA` by threat type
         :type threat_type: str
         :param threat_uid: Search YARA by threat UID
         :type threat_uid: str
         :param malware_family: Search YARA by malware family (e.g. `gozi_isfb`, `smokeloader`, `trickbot`)
         :type malware_family: str
         :param malware_family_profile_uid: Search YARA by malware family profile UID. Useful for getting context for everything we have around specific malware family, for instance https://api.intel471.com/v1/search?malwareFamilyProfileUid=d073f7352b82c1b8eedda381590adced
         :type malware_family_profile_uid: str
@@ -102,15 +102,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.yara_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param yara: Free text YARA search (all fields included). At least one of `yara`, `threatType`, `threatUid`, `malwareFamily`, `malwareFamilyProfileUid` or `confidence` is required.
         :type yara: str
-        :param threat_type: Search `YARA` by threat type (e.g. `malware`, `bulletproof_hosting`, `proxy_service`)
+        :param threat_type: Search `YARA` by threat type
         :type threat_type: str
         :param threat_uid: Search YARA by threat UID
         :type threat_uid: str
         :param malware_family: Search YARA by malware family (e.g. `gozi_isfb`, `smokeloader`, `trickbot`)
         :type malware_family: str
         :param malware_family_profile_uid: Search YARA by malware family profile UID. Useful for getting context for everything we have around specific malware family, for instance https://api.intel471.com/v1/search?malwareFamilyProfileUid=d073f7352b82c1b8eedda381590adced
         :type malware_family_profile_uid: str
```

### Comparing `Titan Client-1.19.7/titan_client/api_client.py` & `Titan Client-1.19.7.1/titan_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.19.7/python'
+        self.user_agent = 'OpenAPI-Generator/1.19.7.1/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `Titan Client-1.19.7/titan_client/configuration.py` & `Titan Client-1.19.7.1/titan_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.19.7\n"\
-               "SDK Package Version: 1.19.7".\
+               "SDK Package Version: 1.19.7.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `Titan Client-1.19.7/titan_client/exceptions.py` & `Titan Client-1.19.7.1/titan_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/__init__.py` & `Titan Client-1.19.7.1/titan_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/actors_get412_response.py` & `Titan Client-1.19.7.1/titan_client/models/actors_get412_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/alert_list_schema.py` & `Titan Client-1.19.7.1/titan_client/models/alert_list_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/alert_list_schema_chunks.py` & `Titan Client-1.19.7.1/titan_client/models/alert_list_schema_chunks.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/alert_list_schema_highlights.py` & `Titan Client-1.19.7.1/titan_client/models/alert_list_schema_highlights.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/alert_list_schema_highlights_inner.py` & `Titan Client-1.19.7.1/titan_client/models/alert_list_schema_highlights_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/alert_list_schema_highlights_inner_chunks_inner.py` & `Titan Client-1.19.7.1/titan_client/models/alert_list_schema_highlights_inner_chunks_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/alert_list_schema_report.py` & `Titan Client-1.19.7.1/titan_client/models/alert_list_schema_report.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/alert_list_schema_response.py` & `Titan Client-1.19.7.1/titan_client/models/alert_list_schema_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/alert_subscription_schema.py` & `Titan Client-1.19.7.1/titan_client/models/alert_subscription_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/alert_subscription_subscribe_response.py` & `Titan Client-1.19.7.1/titan_client/models/alert_subscription_subscribe_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/alerts_get412_response.py` & `Titan Client-1.19.7.1/titan_client/models/alerts_get412_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/breach_alerts_get412_response.py` & `Titan Client-1.19.7.1/titan_client/models/breach_alerts_get412_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_accessed_url_schema.py` & `Titan Client-1.19.7.1/titan_client/models/credential_accessed_url_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_accessed_url_schema_activity.py` & `Titan Client-1.19.7.1/titan_client/models/credential_accessed_url_schema_activity.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_accessed_url_schema_classification.py` & `Titan Client-1.19.7.1/titan_client/models/credential_accessed_url_schema_classification.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_accessed_url_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/credential_accessed_url_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_accessed_url_schema_data_credential.py` & `Titan Client-1.19.7.1/titan_client/models/credential_accessed_url_schema_data_credential.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_accessed_url_stream_schema.py` & `Titan Client-1.19.7.1/titan_client/models/credential_accessed_url_stream_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_accessed_urls_response.py` & `Titan Client-1.19.7.1/titan_client/models/credential_accessed_urls_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_accessed_urls_stream_response.py` & `Titan Client-1.19.7.1/titan_client/models/credential_accessed_urls_stream_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_occurrence_schema.py` & `Titan Client-1.19.7.1/titan_client/models/credential_occurrence_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_occurrence_schema_activity.py` & `Titan Client-1.19.7.1/titan_client/models/credential_occurrence_schema_activity.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_occurrence_schema_classification.py` & `Titan Client-1.19.7.1/titan_client/models/credential_occurrence_schema_classification.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_occurrence_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/credential_occurrence_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_occurrence_schema_data_credential.py` & `Titan Client-1.19.7.1/titan_client/models/credential_occurrence_schema_data_credential.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_occurrence_schema_data_credential_set.py` & `Titan Client-1.19.7.1/titan_client/models/credential_occurrence_schema_data_credential_set.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_occurrences_response.py` & `Titan Client-1.19.7.1/titan_client/models/credential_occurrences_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_occurrences_stream_response.py` & `Titan Client-1.19.7.1/titan_client/models/credential_occurrences_stream_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_schema.py` & `Titan Client-1.19.7.1/titan_client/models/credential_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_schema_activity.py` & `Titan Client-1.19.7.1/titan_client/models/credential_schema_activity.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_schema_classification.py` & `Titan Client-1.19.7.1/titan_client/models/credential_schema_classification.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/credential_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_schema_data_credential_sets.py` & `Titan Client-1.19.7.1/titan_client/models/credential_schema_data_credential_sets.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_schema_data_credential_sets_inner.py` & `Titan Client-1.19.7.1/titan_client/models/credential_schema_data_credential_sets_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_schema_data_password.py` & `Titan Client-1.19.7.1/titan_client/models/credential_schema_data_password.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_schema_data_password_complexity.py` & `Titan Client-1.19.7.1/titan_client/models/credential_schema_data_password_complexity.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_schema_statistics.py` & `Titan Client-1.19.7.1/titan_client/models/credential_schema_statistics.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_set_accessed_url_schema.py` & `Titan Client-1.19.7.1/titan_client/models/credential_set_accessed_url_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_set_accessed_url_schema_activity.py` & `Titan Client-1.19.7.1/titan_client/models/credential_set_accessed_url_schema_activity.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_set_accessed_url_schema_classification.py` & `Titan Client-1.19.7.1/titan_client/models/credential_set_accessed_url_schema_classification.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_set_accessed_url_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/credential_set_accessed_url_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_set_accessed_url_schema_data_credential_set.py` & `Titan Client-1.19.7.1/titan_client/models/credential_set_accessed_url_schema_data_credential_set.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_set_accessed_url_stream_schema.py` & `Titan Client-1.19.7.1/titan_client/models/credential_set_accessed_url_stream_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_set_accessed_url_stream_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/credential_set_accessed_url_stream_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_set_schema.py` & `Titan Client-1.19.7.1/titan_client/models/credential_set_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_set_schema_activity.py` & `Titan Client-1.19.7.1/titan_client/models/credential_set_schema_activity.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_set_schema_classification.py` & `Titan Client-1.19.7.1/titan_client/models/credential_set_schema_classification.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_set_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/credential_set_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_set_schema_data_external_sources.py` & `Titan Client-1.19.7.1/titan_client/models/credential_set_schema_data_external_sources.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_set_schema_data_external_sources_inner.py` & `Titan Client-1.19.7.1/titan_client/models/credential_set_schema_data_external_sources_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_set_schema_data_internal_sources.py` & `Titan Client-1.19.7.1/titan_client/models/credential_set_schema_data_internal_sources.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_set_schema_data_internal_sources_inner.py` & `Titan Client-1.19.7.1/titan_client/models/credential_set_schema_data_internal_sources_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_set_schema_data_victims.py` & `Titan Client-1.19.7.1/titan_client/models/credential_set_schema_data_victims.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_set_schema_data_victims_inner.py` & `Titan Client-1.19.7.1/titan_client/models/credential_set_schema_data_victims_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_set_schema_statistics.py` & `Titan Client-1.19.7.1/titan_client/models/credential_set_schema_statistics.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_set_stream_schema.py` & `Titan Client-1.19.7.1/titan_client/models/credential_set_stream_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_set_stream_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/credential_set_stream_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_sets_accessed_urls_response.py` & `Titan Client-1.19.7.1/titan_client/models/credential_sets_accessed_urls_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_sets_accessed_urls_stream_response.py` & `Titan Client-1.19.7.1/titan_client/models/credential_sets_accessed_urls_stream_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_sets_get412_response.py` & `Titan Client-1.19.7.1/titan_client/models/credential_sets_get412_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_sets_response.py` & `Titan Client-1.19.7.1/titan_client/models/credential_sets_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_sets_stream_get412_response.py` & `Titan Client-1.19.7.1/titan_client/models/credential_sets_stream_get412_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credential_sets_stream_response.py` & `Titan Client-1.19.7.1/titan_client/models/credential_sets_stream_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credentials_get412_response.py` & `Titan Client-1.19.7.1/titan_client/models/credentials_get412_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credentials_response.py` & `Titan Client-1.19.7.1/titan_client/models/credentials_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credentials_stream_get412_response.py` & `Titan Client-1.19.7.1/titan_client/models/credentials_stream_get412_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/credentials_stream_response.py` & `Titan Client-1.19.7.1/titan_client/models/credentials_stream_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/cve_reports_get412_response.py` & `Titan Client-1.19.7.1/titan_client/models/cve_reports_get412_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/entities_response.py` & `Titan Client-1.19.7.1/titan_client/models/entities_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/entities_schema.py` & `Titan Client-1.19.7.1/titan_client/models/entities_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/entities_schema_links.py` & `Titan Client-1.19.7.1/titan_client/models/entities_schema_links.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/entities_schema_links_actors.py` & `Titan Client-1.19.7.1/titan_client/models/entities_schema_links_actors.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/entities_schema_links_actors_inner.py` & `Titan Client-1.19.7.1/titan_client/models/entities_schema_links_actors_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/entities_schema_links_reports.py` & `Titan Client-1.19.7.1/titan_client/models/entities_schema_links_reports.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/entities_schema_links_reports_inner.py` & `Titan Client-1.19.7.1/titan_client/models/entities_schema_links_reports_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/event_schema.py` & `Titan Client-1.19.7.1/titan_client/models/event_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/event_schema_activity.py` & `Titan Client-1.19.7.1/titan_client/models/event_schema_activity.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/event_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/event_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/event_schema_data_event_data.py` & `Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_controller.py` & `Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_controller.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_controller_geo_ip.py` & `Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_controller_geo_ip.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_controller_geo_ip_isp.py` & `Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_controller_geo_ip_isp.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_controllers.py` & `Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_controllers.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_controllers_inner.py` & `Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_controllers_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_encryption.py` & `Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_encryption.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_encryption_inner.py` & `Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_encryption_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_file.py` & `Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_file.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_location.py` & `Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_location.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_recipient_domains.py` & `Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_recipient_domains.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_recipient_domains_inner.py` & `Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_recipient_domains_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_triggers.py` & `Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_triggers.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/event_schema_data_event_data_triggers_inner.py` & `Titan Client-1.19.7.1/titan_client/models/event_schema_data_event_data_triggers_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/event_schema_data_threat.py` & `Titan Client-1.19.7.1/titan_client/models/event_schema_data_threat.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/event_schema_data_threat_data.py` & `Titan Client-1.19.7.1/titan_client/models/event_schema_data_threat_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/event_schema_meta.py` & `Titan Client-1.19.7.1/titan_client/models/event_schema_meta.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/event_stream_response.py` & `Titan Client-1.19.7.1/titan_client/models/event_stream_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/events_response.py` & `Titan Client-1.19.7.1/titan_client/models/events_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/events_stream_get412_response.py` & `Titan Client-1.19.7.1/titan_client/models/events_stream_get412_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/full_breach_alert_schema.py` & `Titan Client-1.19.7.1/titan_client/models/full_breach_alert_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/full_breach_alert_schema_all_of.py` & `Titan Client-1.19.7.1/titan_client/models/full_breach_alert_schema_all_of.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/full_breach_alert_schema_all_of_data.py` & `Titan Client-1.19.7.1/titan_client/models/full_breach_alert_schema_all_of_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/full_breach_alert_schema_all_of_data_breach_alert.py` & `Titan Client-1.19.7.1/titan_client/models/full_breach_alert_schema_all_of_data_breach_alert.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/full_cve_schema.py` & `Titan Client-1.19.7.1/titan_client/models/full_cve_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/full_news_schema.py` & `Titan Client-1.19.7.1/titan_client/models/full_news_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/full_report_schema.py` & `Titan Client-1.19.7.1/titan_client/models/full_report_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/full_report_schema_all_of.py` & `Titan Client-1.19.7.1/titan_client/models/full_report_schema_all_of.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/full_spot_report_schema.py` & `Titan Client-1.19.7.1/titan_client/models/full_spot_report_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/full_watcher_group_schema.py` & `Titan Client-1.19.7.1/titan_client/models/full_watcher_group_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/full_watcher_group_schema_all_of.py` & `Titan Client-1.19.7.1/titan_client/models/full_watcher_group_schema_all_of.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/full_watcher_group_schema_all_of_links.py` & `Titan Client-1.19.7.1/titan_client/models/full_watcher_group_schema_all_of_links.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/full_watcher_group_schema_all_of_links_forum.py` & `Titan Client-1.19.7.1/titan_client/models/full_watcher_group_schema_all_of_links_forum.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/full_watcher_group_schema_all_of_links_thread.py` & `Titan Client-1.19.7.1/titan_client/models/full_watcher_group_schema_all_of_links_thread.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/full_watcher_group_schema_all_of_patterns.py` & `Titan Client-1.19.7.1/titan_client/models/full_watcher_group_schema_all_of_patterns.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/full_watcher_group_schema_all_of_watchers.py` & `Titan Client-1.19.7.1/titan_client/models/full_watcher_group_schema_all_of_watchers.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/gir_schema.py` & `Titan Client-1.19.7.1/titan_client/models/gir_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/gir_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/gir_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/gir_schema_data_gir.py` & `Titan Client-1.19.7.1/titan_client/models/gir_schema_data_gir.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/girs_get412_response.py` & `Titan Client-1.19.7.1/titan_client/models/girs_get412_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/girs_response.py` & `Titan Client-1.19.7.1/titan_client/models/girs_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/indicator_search_response.py` & `Titan Client-1.19.7.1/titan_client/models/indicator_search_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/indicator_search_schema.py` & `Titan Client-1.19.7.1/titan_client/models/indicator_search_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/indicator_search_schema_activity.py` & `Titan Client-1.19.7.1/titan_client/models/indicator_search_schema_activity.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/indicator_search_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/indicator_search_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/indicator_search_schema_data_context.py` & `Titan Client-1.19.7.1/titan_client/models/indicator_search_schema_data_context.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/indicator_search_schema_data_indicator_data.py` & `Titan Client-1.19.7.1/titan_client/models/indicator_search_schema_data_indicator_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/indicator_search_schema_data_indicator_data_file.py` & `Titan Client-1.19.7.1/titan_client/models/indicator_search_schema_data_indicator_data_file.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/indicator_search_schema_data_threat.py` & `Titan Client-1.19.7.1/titan_client/models/indicator_search_schema_data_threat.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/indicator_search_schema_data_threat_data.py` & `Titan Client-1.19.7.1/titan_client/models/indicator_search_schema_data_threat_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/indicator_search_schema_meta.py` & `Titan Client-1.19.7.1/titan_client/models/indicator_search_schema_meta.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/indicator_stream_response.py` & `Titan Client-1.19.7.1/titan_client/models/indicator_stream_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/inline_object.py` & `Titan Client-1.19.7.1/titan_client/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/inline_object1.py` & `Titan Client-1.19.7.1/titan_client/models/inline_object1.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/instant_message_schema.py` & `Titan Client-1.19.7.1/titan_client/models/instant_message_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/instant_message_schema_activity.py` & `Titan Client-1.19.7.1/titan_client/models/instant_message_schema_activity.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/instant_message_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/instant_message_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/instant_message_schema_data_actor.py` & `Titan Client-1.19.7.1/titan_client/models/instant_message_schema_data_actor.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/instant_message_schema_data_channel.py` & `Titan Client-1.19.7.1/titan_client/models/instant_message_schema_data_channel.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/instant_message_schema_data_message.py` & `Titan Client-1.19.7.1/titan_client/models/instant_message_schema_data_message.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/instant_message_schema_data_message_attachments.py` & `Titan Client-1.19.7.1/titan_client/models/instant_message_schema_data_message_attachments.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/instant_message_schema_data_message_attachments_inner.py` & `Titan Client-1.19.7.1/titan_client/models/instant_message_schema_data_message_attachments_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/instant_message_schema_data_server.py` & `Titan Client-1.19.7.1/titan_client/models/instant_message_schema_data_server.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/ioc_schema.py` & `Titan Client-1.19.7.1/titan_client/models/ioc_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/ioc_schema_links.py` & `Titan Client-1.19.7.1/titan_client/models/ioc_schema_links.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/ioc_schema_links_actors.py` & `Titan Client-1.19.7.1/titan_client/models/ioc_schema_links_actors.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/ioc_schema_links_actors_inner.py` & `Titan Client-1.19.7.1/titan_client/models/ioc_schema_links_actors_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/ioc_schema_links_reports.py` & `Titan Client-1.19.7.1/titan_client/models/ioc_schema_links_reports.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/ioc_schema_links_reports_inner.py` & `Titan Client-1.19.7.1/titan_client/models/ioc_schema_links_reports_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/iocs_response.py` & `Titan Client-1.19.7.1/titan_client/models/iocs_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/malware.py` & `Titan Client-1.19.7.1/titan_client/models/malware.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/malware_families_get412_response.py` & `Titan Client-1.19.7.1/titan_client/models/malware_families_get412_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/malware_family_search_response.py` & `Titan Client-1.19.7.1/titan_client/models/malware_family_search_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/malware_family_search_schema.py` & `Titan Client-1.19.7.1/titan_client/models/malware_family_search_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/malware_family_search_schema_activity.py` & `Titan Client-1.19.7.1/titan_client/models/malware_family_search_schema_activity.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/malware_pcaps_get412_response.py` & `Titan Client-1.19.7.1/titan_client/models/malware_pcaps_get412_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/malware_reports_search_response.py` & `Titan Client-1.19.7.1/titan_client/models/malware_reports_search_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/malware_reports_search_schema.py` & `Titan Client-1.19.7.1/titan_client/models/malware_reports_search_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/malware_reports_search_schema_activity.py` & `Titan Client-1.19.7.1/titan_client/models/malware_reports_search_schema_activity.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/malware_reports_search_schema_classification.py` & `Titan Client-1.19.7.1/titan_client/models/malware_reports_search_schema_classification.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/malware_reports_search_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/malware_reports_search_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/malware_reports_search_schema_data_malware_report_data.py` & `Titan Client-1.19.7.1/titan_client/models/malware_reports_search_schema_data_malware_report_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/malware_reports_search_schema_data_malware_report_data_attachments.py` & `Titan Client-1.19.7.1/titan_client/models/malware_reports_search_schema_data_malware_report_data_attachments.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/malware_reports_search_schema_data_malware_report_data_attachments_inner.py` & `Titan Client-1.19.7.1/titan_client/models/malware_reports_search_schema_data_malware_report_data_attachments_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/malware_reports_search_schema_data_threat.py` & `Titan Client-1.19.7.1/titan_client/models/malware_reports_search_schema_data_threat.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/malware_reports_search_schema_data_threat_data.py` & `Titan Client-1.19.7.1/titan_client/models/malware_reports_search_schema_data_threat_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_product_availability_schema.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_product_availability_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_product_credential_schema.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_product_credential_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_product_credential_schema_victim.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_product_credential_schema_victim.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_product_credit_card_schema.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_product_credit_card_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_product_credit_card_schema_victim.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_product_credit_card_schema_victim.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_product_marketplace_schema.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_product_marketplace_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_product_other_product_schema.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_product_other_product_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_product_search_response.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_product_search_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_product_search_schema.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_product_search_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_product_search_schema_activity.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_product_search_schema_activity.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_product_search_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_product_search_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_product_statistics_schema.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_product_statistics_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_product_stream_response.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_product_stream_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_product_type_schema.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_product_type_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_resource_search_response.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_resource_search_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_resource_search_schema.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_resource_search_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_resource_search_schema_activity.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_resource_search_schema_activity.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_resource_search_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_resource_search_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_resource_stream_response.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_resource_stream_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_search_response.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_search_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_search_schema.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_search_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_search_schema_activity.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_search_schema_activity.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_search_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_search_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_search_schema_statistics.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_search_schema_statistics.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_vendor_search_response.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_vendor_search_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_vendor_search_schema.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_vendor_search_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_vendor_search_schema_activity.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_vendor_search_schema_activity.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_vendor_search_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_vendor_search_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_vendor_search_schema_statistics.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_vendor_search_schema_statistics.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplace_vendor_stream_response.py` & `Titan Client-1.19.7.1/titan_client/models/marketplace_vendor_stream_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/marketplaces_products_stream_get412_response.py` & `Titan Client-1.19.7.1/titan_client/models/marketplaces_products_stream_get412_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/messaging_services_instant_messages_get412_response.py` & `Titan Client-1.19.7.1/titan_client/models/messaging_services_instant_messages_get412_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/messaging_services_response.py` & `Titan Client-1.19.7.1/titan_client/models/messaging_services_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/news_schema.py` & `Titan Client-1.19.7.1/titan_client/models/news_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/news_schema_activity.py` & `Titan Client-1.19.7.1/titan_client/models/news_schema_activity.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/news_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/news_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/news_schema_data_attachments.py` & `Titan Client-1.19.7.1/titan_client/models/news_schema_data_attachments.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/news_schema_data_attachments_inner.py` & `Titan Client-1.19.7.1/titan_client/models/news_schema_data_attachments_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/pcap_response.py` & `Titan Client-1.19.7.1/titan_client/models/pcap_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/pcap_schema.py` & `Titan Client-1.19.7.1/titan_client/models/pcap_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/pcap_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/pcap_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/pcap_schema_data_file.py` & `Titan Client-1.19.7.1/titan_client/models/pcap_schema_data_file.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/pcap_schema_data_malware_family.py` & `Titan Client-1.19.7.1/titan_client/models/pcap_schema_data_malware_family.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/pcap_schema_data_pcap.py` & `Titan Client-1.19.7.1/titan_client/models/pcap_schema_data_pcap.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/post_schema.py` & `Titan Client-1.19.7.1/titan_client/models/post_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/post_schema_links.py` & `Titan Client-1.19.7.1/titan_client/models/post_schema_links.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/post_schema_links_author_actor.py` & `Titan Client-1.19.7.1/titan_client/models/post_schema_links_author_actor.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/post_schema_links_forum.py` & `Titan Client-1.19.7.1/titan_client/models/post_schema_links_forum.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/post_schema_links_thread.py` & `Titan Client-1.19.7.1/titan_client/models/post_schema_links_thread.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/posts_response.py` & `Titan Client-1.19.7.1/titan_client/models/posts_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/private_message_schema.py` & `Titan Client-1.19.7.1/titan_client/models/private_message_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/private_message_schema_links.py` & `Titan Client-1.19.7.1/titan_client/models/private_message_schema_links.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/private_message_schema_links_author_actor.py` & `Titan Client-1.19.7.1/titan_client/models/private_message_schema_links_author_actor.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/private_message_schema_links_forum.py` & `Titan Client-1.19.7.1/titan_client/models/private_message_schema_links_forum.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/private_message_schema_links_recipient_actor.py` & `Titan Client-1.19.7.1/titan_client/models/private_message_schema_links_recipient_actor.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/private_message_schema_links_thread.py` & `Titan Client-1.19.7.1/titan_client/models/private_message_schema_links_thread.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/private_messages_response.py` & `Titan Client-1.19.7.1/titan_client/models/private_messages_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/reports_get412_response.py` & `Titan Client-1.19.7.1/titan_client/models/reports_get412_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/search_schema.py` & `Titan Client-1.19.7.1/titan_client/models/search_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_actor_schema.py` & `Titan Client-1.19.7.1/titan_client/models/simple_actor_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_actor_schema_links.py` & `Titan Client-1.19.7.1/titan_client/models/simple_actor_schema_links.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_actor_schema_links_contact_info.py` & `Titan Client-1.19.7.1/titan_client/models/simple_actor_schema_links_contact_info.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_actor_schema_links_forums.py` & `Titan Client-1.19.7.1/titan_client/models/simple_actor_schema_links_forums.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_actor_schema_links_forums_inner.py` & `Titan Client-1.19.7.1/titan_client/models/simple_actor_schema_links_forums_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_actor_schema_links_forums_inner_contact_info_inner.py` & `Titan Client-1.19.7.1/titan_client/models/simple_actor_schema_links_forums_inner_contact_info_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_actor_schema_links_instant_message_servers.py` & `Titan Client-1.19.7.1/titan_client/models/simple_actor_schema_links_instant_message_servers.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_actor_schema_links_instant_message_servers_inner.py` & `Titan Client-1.19.7.1/titan_client/models/simple_actor_schema_links_instant_message_servers_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_actors_response.py` & `Titan Client-1.19.7.1/titan_client/models/simple_actors_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_breach_alert_response.py` & `Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema.py` & `Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_activity.py` & `Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_activity.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_breach_alert.py` & `Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_breach_alert.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_breach_alert_confidence.py` & `Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_breach_alert_confidence.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_breach_alert_sources.py` & `Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_breach_alert_sources.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_breach_alert_sources_inner.py` & `Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_breach_alert_sources_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_breach_alert_victim.py` & `Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_breach_alert_victim.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_breach_alert_victim_industries.py` & `Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_breach_alert_victim_industries.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_breach_alert_victim_industries_inner.py` & `Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_breach_alert_victim_industries_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_entities.py` & `Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_entities.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_entities_inner.py` & `Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_entities_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_entities_inner_geo_info.py` & `Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_entities_inner_geo_info.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_breach_alert_schema_data_geo_info.py` & `Titan Client-1.19.7.1/titan_client/models/simple_breach_alert_schema_data_geo_info.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_cve_schema.py` & `Titan Client-1.19.7.1/titan_client/models/simple_cve_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_cve_schema_activity.py` & `Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_activity.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_cve_schema_classification.py` & `Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_classification.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_cve_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report.py` & `Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_activity_location.py` & `Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_activity_location.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_counter_measure_links.py` & `Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_counter_measure_links.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_counter_measure_links_inner.py` & `Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_counter_measure_links_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_cvss_score.py` & `Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_cvss_score.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_exploit_status.py` & `Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_exploit_status.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_interest_level.py` & `Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_interest_level.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_patch_links.py` & `Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_patch_links.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_patch_links_inner.py` & `Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_patch_links_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_poc_links.py` & `Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_poc_links.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_poc_links_inner.py` & `Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_poc_links_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_titan_links.py` & `Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_titan_links.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_cve_schema_data_cve_report_titan_links_inner.py` & `Titan Client-1.19.7.1/titan_client/models/simple_cve_schema_data_cve_report_titan_links_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_cves_response.py` & `Titan Client-1.19.7.1/titan_client/models/simple_cves_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_news_response.py` & `Titan Client-1.19.7.1/titan_client/models/simple_news_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_report_schema.py` & `Titan Client-1.19.7.1/titan_client/models/simple_report_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_report_schema_actor_subject_of_report.py` & `Titan Client-1.19.7.1/titan_client/models/simple_report_schema_actor_subject_of_report.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_report_schema_actor_subject_of_report_inner.py` & `Titan Client-1.19.7.1/titan_client/models/simple_report_schema_actor_subject_of_report_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_report_schema_classification.py` & `Titan Client-1.19.7.1/titan_client/models/simple_report_schema_classification.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_report_schema_entities.py` & `Titan Client-1.19.7.1/titan_client/models/simple_report_schema_entities.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_report_schema_entities_inner.py` & `Titan Client-1.19.7.1/titan_client/models/simple_report_schema_entities_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_report_schema_locations.py` & `Titan Client-1.19.7.1/titan_client/models/simple_report_schema_locations.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_report_schema_locations_inner.py` & `Titan Client-1.19.7.1/titan_client/models/simple_report_schema_locations_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_report_schema_related_reports.py` & `Titan Client-1.19.7.1/titan_client/models/simple_report_schema_related_reports.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_report_schema_related_reports_inner.py` & `Titan Client-1.19.7.1/titan_client/models/simple_report_schema_related_reports_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_report_schema_report_attachments.py` & `Titan Client-1.19.7.1/titan_client/models/simple_report_schema_report_attachments.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_report_schema_report_attachments_inner.py` & `Titan Client-1.19.7.1/titan_client/models/simple_report_schema_report_attachments_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_report_schema_sources.py` & `Titan Client-1.19.7.1/titan_client/models/simple_report_schema_sources.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_report_schema_sources_inner.py` & `Titan Client-1.19.7.1/titan_client/models/simple_report_schema_sources_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_report_schema_victims.py` & `Titan Client-1.19.7.1/titan_client/models/simple_report_schema_victims.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_report_schema_victims_inner.py` & `Titan Client-1.19.7.1/titan_client/models/simple_report_schema_victims_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_reports_response.py` & `Titan Client-1.19.7.1/titan_client/models/simple_reports_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_spot_report_schema.py` & `Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_spot_report_schema_activity.py` & `Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema_activity.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_spot_report_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_spot_report_schema_data_entities.py` & `Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema_data_entities.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_spot_report_schema_data_entities_inner.py` & `Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema_data_entities_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_spot_report_schema_data_spot_report.py` & `Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema_data_spot_report.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_spot_report_schema_data_spot_report_spot_report_data.py` & `Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema_data_spot_report_spot_report_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_spot_report_schema_data_spot_report_spot_report_data_links.py` & `Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema_data_spot_report_spot_report_data_links.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_spot_report_schema_data_spot_report_spot_report_data_links_inner.py` & `Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema_data_spot_report_spot_report_data_links_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_spot_report_schema_data_spot_report_spot_report_data_victims.py` & `Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema_data_spot_report_spot_report_data_victims.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_spot_report_schema_data_spot_report_spot_report_data_victims_inner.py` & `Titan Client-1.19.7.1/titan_client/models/simple_spot_report_schema_data_spot_report_spot_report_data_victims_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_spot_reports_response.py` & `Titan Client-1.19.7.1/titan_client/models/simple_spot_reports_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/simple_watcher_group_schema.py` & `Titan Client-1.19.7.1/titan_client/models/simple_watcher_group_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/situation_report_response.py` & `Titan Client-1.19.7.1/titan_client/models/situation_report_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/situation_report_schema.py` & `Titan Client-1.19.7.1/titan_client/models/situation_report_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/situation_report_schema_activity.py` & `Titan Client-1.19.7.1/titan_client/models/situation_report_schema_activity.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/situation_report_schema_classification.py` & `Titan Client-1.19.7.1/titan_client/models/situation_report_schema_classification.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/situation_report_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/situation_report_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/situation_report_schema_data_situation_report.py` & `Titan Client-1.19.7.1/titan_client/models/situation_report_schema_data_situation_report.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/situation_report_schema_data_situation_report_entities.py` & `Titan Client-1.19.7.1/titan_client/models/situation_report_schema_data_situation_report_entities.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/situation_report_schema_data_situation_report_entities_inner.py` & `Titan Client-1.19.7.1/titan_client/models/situation_report_schema_data_situation_report_entities_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/situation_report_schema_data_situation_report_link.py` & `Titan Client-1.19.7.1/titan_client/models/situation_report_schema_data_situation_report_link.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/situation_report_schema_data_situation_report_link_malware_family.py` & `Titan Client-1.19.7.1/titan_client/models/situation_report_schema_data_situation_report_link_malware_family.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/situation_report_schema_data_situation_report_link_malware_report.py` & `Titan Client-1.19.7.1/titan_client/models/situation_report_schema_data_situation_report_link_malware_report.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/situation_report_schema_data_situation_report_victims.py` & `Titan Client-1.19.7.1/titan_client/models/situation_report_schema_data_situation_report_victims.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/situation_report_schema_data_situation_report_victims_inner.py` & `Titan Client-1.19.7.1/titan_client/models/situation_report_schema_data_situation_report_victims_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/tag_response.py` & `Titan Client-1.19.7.1/titan_client/models/tag_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/tag_schema.py` & `Titan Client-1.19.7.1/titan_client/models/tag_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_group_response.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_group_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_groups_get412_response.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_groups_get412_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_groups_get_request.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_groups_get_request.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_groups_group_uid_delete_request.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_groups_group_uid_delete_request.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_groups_group_uid_put_request.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_groups_group_uid_put_request.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,26 @@
     Titan API v1
 
     # Introduction The Intel 471 API is organized around the principles of REST. Our API lets you gather results from our platform using anything that can send a HTTP request, including cURL and modern internet browsers. Access to this API requires an API token which is managed from your account settings.  Intel 471 reserves the right to add fields to our API however we will provide backwards compatibility and older version support so that it will be possible to choose exact versions that provide a response with an older structure.  # Authentication Authentication to the API occurs by providing your email address as the login and API key as a password in the authorization header via HTTP Basic Auth. Your API key can be found in the [API](https://portal.intel471.com/api) section on the portal. It carries many privileges so please do not expose it on public web resources.  # Accessing the API  Following examples demonstrate different methods to get the reports from `/reports` endpoint.  ## Internet browser  Just open URL: https://api.intel471.com/v1/reports  Browser will ask you for credentials, provide your email as login and API key as password.  ## cURL command line utility  Execute following command in your terminal:  ``` curl -u <YOU EMAIL>:<YOUR API KEY> https://api.intel471.com/v1/reports ```  ## Python client  We provide a [Python client](https://github.com/intel471/titan-client-python) for Intel 471's Titan API, which aims at providing common ground for all the endpoints. Please note that all the call parameters and response body fields' names are normalized to camel_case, so for example when you search reports by document type using Python client use `document_type` instead of `documentType`.  Install the client using pip (python >= 3.6 required):  ``` pip install titan-client ```  Run following script  ```python import titan_client  configuration = titan_client.Configuration(     username=\"<YOU EMAIL>\",     password=\"<YOUR API KEY>\")  with titan_client.ApiClient(configuration) as api_client:     api_instance = titan_client.ReportsApi(api_client)     api_response = api_instance.reports_get() print(api_response) ```  # Use cases  Below we present several commonly used scenarios in both raw HTTP request format and as a script using Python client. Examples are simplified so that they do not contain the authentication part and for Python client they do not contain configuration and API client object creation portion. For full example please refer to **Accessing the API** section of this document.   ## Paging  One page of the results can carry up to 100 records and you can display up to 11 pages for one query (max offset is 1000) in non-stream API endpoints. Use `count` parameter to set the number of items per page. Use `offset` parameter to shift the window by given number of results.       **HTTP**   ``` # Get 20 reports, sorted by the default field GET https://api.intel471.com/v1/reports?count=20  # Get next 20 reports GET https://api.intel471.com/v1/reports?count=20&offset=20  # Get 40 reports in one go to save API calls GET https://api.intel471.com/v1/reports?count=40 ```  **Python**  ``` response = titan_client.ReportsApi(api_client).reports_get(count=20, offset=20) ```  ## Paging beyond the max allowed offset  Paging described in the previous use case is generally sufficient for most needs. If there are more than 1100 objects  to be obtained for a given time period and set of filter criteria, then it is possible to move the filter timestamps  along and then restart the offset sequencing. There is a very small number of situations where this may cause issues,  where there is multiple objects with the same timestamp adjacent to the last object in the response.  For the higher volume or fast changing data (such as malware indicators, malware events, creds) there are stream API endpoints  available where cursors may be used in order to acquire data easily and to avoid the need to shift timestamp ranges.  ``` # Get first 11 pages, 100 objects each  GET https://api.intel471.com/v1/reports?sort=latest&count=100 GET https://api.intel471.com/v1/reports?sort=latest&count=100&offset=100 ... GET https://api.intel471.com/v1/reports?sort=latest&count=100&offset=1000 ... > {\"reports\": [{..., \"created\": 1661867086000}, {..., \"created\": 1661864268000}]} ```  Then the `created` time value from the last response will be used as an upper limit in the next series of calls:  ```   GET https://api.intel471.com/v1/reports?sort=latest&until=1661864268000&count=100 GET https://api.intel471.com/v1/reports?sort=latest&until=1661864268000&offset=100 ... GET https://api.intel471.com/v1/reports?sort=latest&until=1661864268000&offset=1000 ```  And so on, until the results are available or until the desired number of objects has been fetched.  ## Paging /alerts endpoint  Alerts endpoint differs from all the other non-stream API endpoints in that the `offset` parameter needs to be set  to the uid of the most recent acquired alert instead of an integer indicating the shift.  **HTTP**   ``` GET https://api.intel471.com/v1/alerts?count=100 > {\"alerts\": [{..., \"uid\": \"abc123\"}, {..., \"uid\": \"abc234\"}]}  GET https://api.intel471.com/v1/alerts?count=100&offset=abc234 > {\"alerts\": [{..., \"uid\": \"abc345\"}, {..., \"uid\": \"abc456\"}]} ```  **Python**  ``` response = titan_client.AlertsApi(api_client).alerts_get(count=100, offset=\"abc456\") ```  ## Stream endpoints paging  Stream endpoints provide the same data as their regular counterparts but they differ in a way of paging.  When working with a stream endpoint, the response always contains `cursorNext` field, which should be provided to the next subsequent  call to fetch potential next page of the results. All the subsequent calls should have the same set of query parameters as the first one,  except the cursor value. Keep calling the endpoint with a new cursor value until it stops yielding results. When new data appear after that, another call will fetch it.  **HTTP**   ``` GET https://api.intel471.com/v1/indicators/stream?lastUpdatedFrom=1655809200000 > {\"indicators\": [...], \"cursorNext\": \"MTY1NT1\"}  GET https://api.intel471.com/v1/indicators/stream?lastUpdatedFrom=1655809200000&cursor=MTY1NT1 > {\"indicators\": [...], \"cursorNext\": \"MTY1NT2\"}  GET https://api.intel471.com/v1/indicators/stream?lastUpdatedFrom=1655809200000&cursor=MTY1NT2 > {\"cursorNext\": \"MTY1NT3\"} ```  **Python**  ``` response = titan_client.IndicatorsApi(api_client).indicators_stream_get(last_updated_from=1656809200000) print(response.cursor_next, response.indicators) # MTY1NT1, [...]  response = titan_client.IndicatorsApi(api_client).indicators_stream_get(last_updated_from=1656809200000, cursor=\"MTY1NT1\")) print(response.cursor_next, response.indicators) # MTY1NT2, [...]  response = titan_client.IndicatorsApi(api_client).indicators_stream_get(last_updated_from=1656809200000, cursor=\"MTY1NT2\")) print(response.cursor_next, response.indicators) # MTY1NT3, None ```  ## Querying using logical operators  ### Array parameters  Any query parameter can be singular or array, if multiple parameters with the same name were provided. All parameters with the same name are internally combined into a query with `AND` operator.  So following query:  ``` GET https://api.intel471.com/v1/reports?report=sources&report=abba ```  Means \"find me reports with `source` AND `abba` in their body\".  This approach is not supported in the Python client. Instead use query string method discussed below.   ### Query string parameters  Query parameters accept Elastic's query string syntax, which allows for even better flexibility.  For example above query can be rephrased as:  **HTTP**   ``` GET https://api.intel471.com/v1/reports?report=sources OR abba ```  **Python**  ``` response = titan_client.ReportsApi(api_client).reports_get(report=\"sources OR abba\") ```  More advanced combination would include both `OR` and `AND` operators and a negation:  **HTTP**  ``` GET https://api.intel471.com/v1/reports?report=(sources OR abba) AND -creaba ```  **Python**  ``` response = titan_client.ReportsApi(api_client).reports_get(report=\"(sources OR abba) AND -creaba\") ```  Means \"find me reports with `source` or `abba` in their body which at the same time do not contain `creaba`\".  The query string \"mini-language\" reference and examples can be found on  [Elastic's query string syntax](https://www.elastic.co/guide/en/elasticsearch/reference/7.5/query-dsl-query-string-query.html#query-dsl-query-string-query) page.  ## Get CVEs using multiple filtering criteria  Get all CVE reports for Chrome product where the risk is high and the patch is not available yet.  **HTTP**   ``` GET https://api.intel471.com/v1/cve/reports?productName=Chrome&riskLevel=high&patchStatus=unavailable ```  **Python**  ``` response = titan_client.VulnerabilitiesApi(api_client).cve_reports_get(     product_name=\"Chrome\",     risk_level=\"high\",     patch_status=\"unavailable\" ) ```  ## List watcher groups   **HTTP**   ``` GET https://api.intel471.com/v1/watcherGroups ```  **Python**  ``` response = titan_client.WatchersApi(api_client).watcher_groups_get() ```  ## Create watcher group   To create a watcher group you need to pass a body along with the request.  **HTTP**   ``` POST https://api.intel471.com/v1/watcherGroups {   \"name\": \"my_group_name\",   \"description\": \"My description\" } ```  **Python**  ``` response = titan_client.WatchersApi(api_client).watcher_groups_post(   {\"name\": \"my_group_name\", \"description\": \"My description\"} ) ```  ## Create free text search watcher  **HTTP**   ``` POST https://api.intel471.com/v1/watcherGroups/<GROUP UID>/watchers {   \"type\": \"search\",   \"freeTextPattern\": \"text to search\",   \"notificationChannel\": \"website\" } ```  **Python**  ``` response = titan_client.WatchersApi(api_client).watcher_groups_group_uid_watchers_post(   group_uid=\"<GROUP UID>\",   watcher_request_body_post={     \"type\": \"search\",     \"freeTextPattern\": \"text to search\",     \"notificationChannel\": \"website\"   } ) ```  ## Create specific search watcher  **HTTP**   ``` POST https://api.intel471.com/v1/watcherGroups/<GROUP UID>/watchers {   \"type\": \"search\",   \"patterns\": [     {\"types\": \"Actor\" , \"pattern\": \"swisman\"}   ],   \"notificationChannel\": \"website\" } ```  **Python**  ``` response = titan_client.WatchersApi(api_client).watcher_groups_group_uid_watchers_post(   group_uid=\"<GROUP UID>\",   watcher_request_body_post={     \"type\": \"search\",     \"patterns\": [       {\"types\": \"Actor\" , \"pattern\": \"swisman\"}     ],     \"notificationChannel\": \"website\"   } ) ```  # API integration best practice with your application CORS requests to the API are not allowed due to security concerns, so please avoid AJAX calls directly from the browser. Instead consider setting up a server side proxy in your application to handle API requests.  Please consider not storing information provided by the API locally as we are constantly improving our data set and want you to have the most updated information.  # Versioning support We consistently improve our API and occasionally introduce the changes based on the customer feedback. The current API version is provided in this documentation's header. We provide API backwards compatibility whenever possible.  All requests are prefixed with the major version number, for example `/v1`:  ``` https://api.intel471.com/v1/reports ```  Different major versions are not compatible and imply significant response structure changes. Minor versions differences might include extra fields in response or provide new request parameter support. To stick to the specific version, just add `v` parameter to the request, for example: `?v=1.19.2`. If you specify a non existing version, it will be brought down to the nearest existing one.  Omitting the version parameter in the request will call the latest version of the API.  We consistently phase out the outdated versions of the API, keeping only several most recent versions. Specific version is getting disabled only when we do not record any requests using it, so it's guaranteed that calls to the outdated ones will work, though we recommend switching to the latest one as soon as possible.  We recommend to always add the version parameter to the request to be safe on API updates in your integrations.   Python client always adds the version parameter in the underlying request. API version matches the Python client's package version.   # noqa: E501
 
     The version of the OpenAPI document: 1.19.7
     Generated by: https://openapi-generator.tech
 """
-from titan_client.titan_stix import STIXMapperSettings
+
 
 try:
     from inspect import getfullargspec
 except ImportError:
     from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
 import six
 
 from titan_client.configuration import Configuration
+from titan_client.titan_stix import STIXMapperSettings
 from titan_client.titan_stix.mappers.common import StixMapper
 
 
 class WatcherGroupsGroupUidPutRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -167,15 +168,14 @@
 
         return result
 
     def to_stix(self, settings: STIXMapperSettings = None):
         stix_mapper = StixMapper(settings)
         return stix_mapper.map(self.to_dict(serialize=True))
 
-
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
```

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_groups_group_uid_watchers_get412_response.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_groups_group_uid_watchers_get412_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_groups_group_uid_watchers_post412_response.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_groups_group_uid_watchers_post412_response.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,25 +4,26 @@
     Titan API v1
 
     # Introduction The Intel 471 API is organized around the principles of REST. Our API lets you gather results from our platform using anything that can send a HTTP request, including cURL and modern internet browsers. Access to this API requires an API token which is managed from your account settings.  Intel 471 reserves the right to add fields to our API however we will provide backwards compatibility and older version support so that it will be possible to choose exact versions that provide a response with an older structure.  # Authentication Authentication to the API occurs by providing your email address as the login and API key as a password in the authorization header via HTTP Basic Auth. Your API key can be found in the [API](https://portal.intel471.com/api) section on the portal. It carries many privileges so please do not expose it on public web resources.  # Accessing the API  Following examples demonstrate different methods to get the reports from `/reports` endpoint.  ## Internet browser  Just open URL: https://api.intel471.com/v1/reports  Browser will ask you for credentials, provide your email as login and API key as password.  ## cURL command line utility  Execute following command in your terminal:  ``` curl -u <YOU EMAIL>:<YOUR API KEY> https://api.intel471.com/v1/reports ```  ## Python client  We provide a [Python client](https://github.com/intel471/titan-client-python) for Intel 471's Titan API, which aims at providing common ground for all the endpoints. Please note that all the call parameters and response body fields' names are normalized to camel_case, so for example when you search reports by document type using Python client use `document_type` instead of `documentType`.  Install the client using pip (python >= 3.6 required):  ``` pip install titan-client ```  Run following script  ```python import titan_client  configuration = titan_client.Configuration(     username=\"<YOU EMAIL>\",     password=\"<YOUR API KEY>\")  with titan_client.ApiClient(configuration) as api_client:     api_instance = titan_client.ReportsApi(api_client)     api_response = api_instance.reports_get() print(api_response) ```  # Use cases  Below we present several commonly used scenarios in both raw HTTP request format and as a script using Python client. Examples are simplified so that they do not contain the authentication part and for Python client they do not contain configuration and API client object creation portion. For full example please refer to **Accessing the API** section of this document.   ## Paging  One page of the results can carry up to 100 records and you can display up to 11 pages for one query (max offset is 1000) in non-stream API endpoints. Use `count` parameter to set the number of items per page. Use `offset` parameter to shift the window by given number of results.       **HTTP**   ``` # Get 20 reports, sorted by the default field GET https://api.intel471.com/v1/reports?count=20  # Get next 20 reports GET https://api.intel471.com/v1/reports?count=20&offset=20  # Get 40 reports in one go to save API calls GET https://api.intel471.com/v1/reports?count=40 ```  **Python**  ``` response = titan_client.ReportsApi(api_client).reports_get(count=20, offset=20) ```  ## Paging beyond the max allowed offset  Paging described in the previous use case is generally sufficient for most needs. If there are more than 1100 objects  to be obtained for a given time period and set of filter criteria, then it is possible to move the filter timestamps  along and then restart the offset sequencing. There is a very small number of situations where this may cause issues,  where there is multiple objects with the same timestamp adjacent to the last object in the response.  For the higher volume or fast changing data (such as malware indicators, malware events, creds) there are stream API endpoints  available where cursors may be used in order to acquire data easily and to avoid the need to shift timestamp ranges.  ``` # Get first 11 pages, 100 objects each  GET https://api.intel471.com/v1/reports?sort=latest&count=100 GET https://api.intel471.com/v1/reports?sort=latest&count=100&offset=100 ... GET https://api.intel471.com/v1/reports?sort=latest&count=100&offset=1000 ... > {\"reports\": [{..., \"created\": 1661867086000}, {..., \"created\": 1661864268000}]} ```  Then the `created` time value from the last response will be used as an upper limit in the next series of calls:  ```   GET https://api.intel471.com/v1/reports?sort=latest&until=1661864268000&count=100 GET https://api.intel471.com/v1/reports?sort=latest&until=1661864268000&offset=100 ... GET https://api.intel471.com/v1/reports?sort=latest&until=1661864268000&offset=1000 ```  And so on, until the results are available or until the desired number of objects has been fetched.  ## Paging /alerts endpoint  Alerts endpoint differs from all the other non-stream API endpoints in that the `offset` parameter needs to be set  to the uid of the most recent acquired alert instead of an integer indicating the shift.  **HTTP**   ``` GET https://api.intel471.com/v1/alerts?count=100 > {\"alerts\": [{..., \"uid\": \"abc123\"}, {..., \"uid\": \"abc234\"}]}  GET https://api.intel471.com/v1/alerts?count=100&offset=abc234 > {\"alerts\": [{..., \"uid\": \"abc345\"}, {..., \"uid\": \"abc456\"}]} ```  **Python**  ``` response = titan_client.AlertsApi(api_client).alerts_get(count=100, offset=\"abc456\") ```  ## Stream endpoints paging  Stream endpoints provide the same data as their regular counterparts but they differ in a way of paging.  When working with a stream endpoint, the response always contains `cursorNext` field, which should be provided to the next subsequent  call to fetch potential next page of the results. All the subsequent calls should have the same set of query parameters as the first one,  except the cursor value. Keep calling the endpoint with a new cursor value until it stops yielding results. When new data appear after that, another call will fetch it.  **HTTP**   ``` GET https://api.intel471.com/v1/indicators/stream?lastUpdatedFrom=1655809200000 > {\"indicators\": [...], \"cursorNext\": \"MTY1NT1\"}  GET https://api.intel471.com/v1/indicators/stream?lastUpdatedFrom=1655809200000&cursor=MTY1NT1 > {\"indicators\": [...], \"cursorNext\": \"MTY1NT2\"}  GET https://api.intel471.com/v1/indicators/stream?lastUpdatedFrom=1655809200000&cursor=MTY1NT2 > {\"cursorNext\": \"MTY1NT3\"} ```  **Python**  ``` response = titan_client.IndicatorsApi(api_client).indicators_stream_get(last_updated_from=1656809200000) print(response.cursor_next, response.indicators) # MTY1NT1, [...]  response = titan_client.IndicatorsApi(api_client).indicators_stream_get(last_updated_from=1656809200000, cursor=\"MTY1NT1\")) print(response.cursor_next, response.indicators) # MTY1NT2, [...]  response = titan_client.IndicatorsApi(api_client).indicators_stream_get(last_updated_from=1656809200000, cursor=\"MTY1NT2\")) print(response.cursor_next, response.indicators) # MTY1NT3, None ```  ## Querying using logical operators  ### Array parameters  Any query parameter can be singular or array, if multiple parameters with the same name were provided. All parameters with the same name are internally combined into a query with `AND` operator.  So following query:  ``` GET https://api.intel471.com/v1/reports?report=sources&report=abba ```  Means \"find me reports with `source` AND `abba` in their body\".  This approach is not supported in the Python client. Instead use query string method discussed below.   ### Query string parameters  Query parameters accept Elastic's query string syntax, which allows for even better flexibility.  For example above query can be rephrased as:  **HTTP**   ``` GET https://api.intel471.com/v1/reports?report=sources OR abba ```  **Python**  ``` response = titan_client.ReportsApi(api_client).reports_get(report=\"sources OR abba\") ```  More advanced combination would include both `OR` and `AND` operators and a negation:  **HTTP**  ``` GET https://api.intel471.com/v1/reports?report=(sources OR abba) AND -creaba ```  **Python**  ``` response = titan_client.ReportsApi(api_client).reports_get(report=\"(sources OR abba) AND -creaba\") ```  Means \"find me reports with `source` or `abba` in their body which at the same time do not contain `creaba`\".  The query string \"mini-language\" reference and examples can be found on  [Elastic's query string syntax](https://www.elastic.co/guide/en/elasticsearch/reference/7.5/query-dsl-query-string-query.html#query-dsl-query-string-query) page.  ## Get CVEs using multiple filtering criteria  Get all CVE reports for Chrome product where the risk is high and the patch is not available yet.  **HTTP**   ``` GET https://api.intel471.com/v1/cve/reports?productName=Chrome&riskLevel=high&patchStatus=unavailable ```  **Python**  ``` response = titan_client.VulnerabilitiesApi(api_client).cve_reports_get(     product_name=\"Chrome\",     risk_level=\"high\",     patch_status=\"unavailable\" ) ```  ## List watcher groups   **HTTP**   ``` GET https://api.intel471.com/v1/watcherGroups ```  **Python**  ``` response = titan_client.WatchersApi(api_client).watcher_groups_get() ```  ## Create watcher group   To create a watcher group you need to pass a body along with the request.  **HTTP**   ``` POST https://api.intel471.com/v1/watcherGroups {   \"name\": \"my_group_name\",   \"description\": \"My description\" } ```  **Python**  ``` response = titan_client.WatchersApi(api_client).watcher_groups_post(   {\"name\": \"my_group_name\", \"description\": \"My description\"} ) ```  ## Create free text search watcher  **HTTP**   ``` POST https://api.intel471.com/v1/watcherGroups/<GROUP UID>/watchers {   \"type\": \"search\",   \"freeTextPattern\": \"text to search\",   \"notificationChannel\": \"website\" } ```  **Python**  ``` response = titan_client.WatchersApi(api_client).watcher_groups_group_uid_watchers_post(   group_uid=\"<GROUP UID>\",   watcher_request_body_post={     \"type\": \"search\",     \"freeTextPattern\": \"text to search\",     \"notificationChannel\": \"website\"   } ) ```  ## Create specific search watcher  **HTTP**   ``` POST https://api.intel471.com/v1/watcherGroups/<GROUP UID>/watchers {   \"type\": \"search\",   \"patterns\": [     {\"types\": \"Actor\" , \"pattern\": \"swisman\"}   ],   \"notificationChannel\": \"website\" } ```  **Python**  ``` response = titan_client.WatchersApi(api_client).watcher_groups_group_uid_watchers_post(   group_uid=\"<GROUP UID>\",   watcher_request_body_post={     \"type\": \"search\",     \"patterns\": [       {\"types\": \"Actor\" , \"pattern\": \"swisman\"}     ],     \"notificationChannel\": \"website\"   } ) ```  # API integration best practice with your application CORS requests to the API are not allowed due to security concerns, so please avoid AJAX calls directly from the browser. Instead consider setting up a server side proxy in your application to handle API requests.  Please consider not storing information provided by the API locally as we are constantly improving our data set and want you to have the most updated information.  # Versioning support We consistently improve our API and occasionally introduce the changes based on the customer feedback. The current API version is provided in this documentation's header. We provide API backwards compatibility whenever possible.  All requests are prefixed with the major version number, for example `/v1`:  ``` https://api.intel471.com/v1/reports ```  Different major versions are not compatible and imply significant response structure changes. Minor versions differences might include extra fields in response or provide new request parameter support. To stick to the specific version, just add `v` parameter to the request, for example: `?v=1.19.2`. If you specify a non existing version, it will be brought down to the nearest existing one.  Omitting the version parameter in the request will call the latest version of the API.  We consistently phase out the outdated versions of the API, keeping only several most recent versions. Specific version is getting disabled only when we do not record any requests using it, so it's guaranteed that calls to the outdated ones will work, though we recommend switching to the latest one as soon as possible.  We recommend to always add the version parameter to the request to be safe on API updates in your integrations.   Python client always adds the version parameter in the underlying request. API version matches the Python client's package version.   # noqa: E501
 
     The version of the OpenAPI document: 1.19.7
     Generated by: https://openapi-generator.tech
 """
-from titan_client.titan_stix import STIXMapperSettings
+
 
 try:
     from inspect import getfullargspec
 except ImportError:
     from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
 import six
 
 from titan_client.configuration import Configuration
+from titan_client.titan_stix import STIXMapperSettings
 from titan_client.titan_stix.mappers.common import StixMapper
 
 
 class WatcherGroupsGroupUidWatchersPost412Response(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -81,15 +82,14 @@
 
         return result
 
     def to_stix(self, settings: STIXMapperSettings = None):
         stix_mapper = StixMapper(settings)
         return stix_mapper.map(self.to_dict(serialize=True))
 
-
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
```

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_groups_post412_response.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_groups_post412_response.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,25 +4,26 @@
     Titan API v1
 
     # Introduction The Intel 471 API is organized around the principles of REST. Our API lets you gather results from our platform using anything that can send a HTTP request, including cURL and modern internet browsers. Access to this API requires an API token which is managed from your account settings.  Intel 471 reserves the right to add fields to our API however we will provide backwards compatibility and older version support so that it will be possible to choose exact versions that provide a response with an older structure.  # Authentication Authentication to the API occurs by providing your email address as the login and API key as a password in the authorization header via HTTP Basic Auth. Your API key can be found in the [API](https://portal.intel471.com/api) section on the portal. It carries many privileges so please do not expose it on public web resources.  # Accessing the API  Following examples demonstrate different methods to get the reports from `/reports` endpoint.  ## Internet browser  Just open URL: https://api.intel471.com/v1/reports  Browser will ask you for credentials, provide your email as login and API key as password.  ## cURL command line utility  Execute following command in your terminal:  ``` curl -u <YOU EMAIL>:<YOUR API KEY> https://api.intel471.com/v1/reports ```  ## Python client  We provide a [Python client](https://github.com/intel471/titan-client-python) for Intel 471's Titan API, which aims at providing common ground for all the endpoints. Please note that all the call parameters and response body fields' names are normalized to camel_case, so for example when you search reports by document type using Python client use `document_type` instead of `documentType`.  Install the client using pip (python >= 3.6 required):  ``` pip install titan-client ```  Run following script  ```python import titan_client  configuration = titan_client.Configuration(     username=\"<YOU EMAIL>\",     password=\"<YOUR API KEY>\")  with titan_client.ApiClient(configuration) as api_client:     api_instance = titan_client.ReportsApi(api_client)     api_response = api_instance.reports_get() print(api_response) ```  # Use cases  Below we present several commonly used scenarios in both raw HTTP request format and as a script using Python client. Examples are simplified so that they do not contain the authentication part and for Python client they do not contain configuration and API client object creation portion. For full example please refer to **Accessing the API** section of this document.   ## Paging  One page of the results can carry up to 100 records and you can display up to 11 pages for one query (max offset is 1000) in non-stream API endpoints. Use `count` parameter to set the number of items per page. Use `offset` parameter to shift the window by given number of results.       **HTTP**   ``` # Get 20 reports, sorted by the default field GET https://api.intel471.com/v1/reports?count=20  # Get next 20 reports GET https://api.intel471.com/v1/reports?count=20&offset=20  # Get 40 reports in one go to save API calls GET https://api.intel471.com/v1/reports?count=40 ```  **Python**  ``` response = titan_client.ReportsApi(api_client).reports_get(count=20, offset=20) ```  ## Paging beyond the max allowed offset  Paging described in the previous use case is generally sufficient for most needs. If there are more than 1100 objects  to be obtained for a given time period and set of filter criteria, then it is possible to move the filter timestamps  along and then restart the offset sequencing. There is a very small number of situations where this may cause issues,  where there is multiple objects with the same timestamp adjacent to the last object in the response.  For the higher volume or fast changing data (such as malware indicators, malware events, creds) there are stream API endpoints  available where cursors may be used in order to acquire data easily and to avoid the need to shift timestamp ranges.  ``` # Get first 11 pages, 100 objects each  GET https://api.intel471.com/v1/reports?sort=latest&count=100 GET https://api.intel471.com/v1/reports?sort=latest&count=100&offset=100 ... GET https://api.intel471.com/v1/reports?sort=latest&count=100&offset=1000 ... > {\"reports\": [{..., \"created\": 1661867086000}, {..., \"created\": 1661864268000}]} ```  Then the `created` time value from the last response will be used as an upper limit in the next series of calls:  ```   GET https://api.intel471.com/v1/reports?sort=latest&until=1661864268000&count=100 GET https://api.intel471.com/v1/reports?sort=latest&until=1661864268000&offset=100 ... GET https://api.intel471.com/v1/reports?sort=latest&until=1661864268000&offset=1000 ```  And so on, until the results are available or until the desired number of objects has been fetched.  ## Paging /alerts endpoint  Alerts endpoint differs from all the other non-stream API endpoints in that the `offset` parameter needs to be set  to the uid of the most recent acquired alert instead of an integer indicating the shift.  **HTTP**   ``` GET https://api.intel471.com/v1/alerts?count=100 > {\"alerts\": [{..., \"uid\": \"abc123\"}, {..., \"uid\": \"abc234\"}]}  GET https://api.intel471.com/v1/alerts?count=100&offset=abc234 > {\"alerts\": [{..., \"uid\": \"abc345\"}, {..., \"uid\": \"abc456\"}]} ```  **Python**  ``` response = titan_client.AlertsApi(api_client).alerts_get(count=100, offset=\"abc456\") ```  ## Stream endpoints paging  Stream endpoints provide the same data as their regular counterparts but they differ in a way of paging.  When working with a stream endpoint, the response always contains `cursorNext` field, which should be provided to the next subsequent  call to fetch potential next page of the results. All the subsequent calls should have the same set of query parameters as the first one,  except the cursor value. Keep calling the endpoint with a new cursor value until it stops yielding results. When new data appear after that, another call will fetch it.  **HTTP**   ``` GET https://api.intel471.com/v1/indicators/stream?lastUpdatedFrom=1655809200000 > {\"indicators\": [...], \"cursorNext\": \"MTY1NT1\"}  GET https://api.intel471.com/v1/indicators/stream?lastUpdatedFrom=1655809200000&cursor=MTY1NT1 > {\"indicators\": [...], \"cursorNext\": \"MTY1NT2\"}  GET https://api.intel471.com/v1/indicators/stream?lastUpdatedFrom=1655809200000&cursor=MTY1NT2 > {\"cursorNext\": \"MTY1NT3\"} ```  **Python**  ``` response = titan_client.IndicatorsApi(api_client).indicators_stream_get(last_updated_from=1656809200000) print(response.cursor_next, response.indicators) # MTY1NT1, [...]  response = titan_client.IndicatorsApi(api_client).indicators_stream_get(last_updated_from=1656809200000, cursor=\"MTY1NT1\")) print(response.cursor_next, response.indicators) # MTY1NT2, [...]  response = titan_client.IndicatorsApi(api_client).indicators_stream_get(last_updated_from=1656809200000, cursor=\"MTY1NT2\")) print(response.cursor_next, response.indicators) # MTY1NT3, None ```  ## Querying using logical operators  ### Array parameters  Any query parameter can be singular or array, if multiple parameters with the same name were provided. All parameters with the same name are internally combined into a query with `AND` operator.  So following query:  ``` GET https://api.intel471.com/v1/reports?report=sources&report=abba ```  Means \"find me reports with `source` AND `abba` in their body\".  This approach is not supported in the Python client. Instead use query string method discussed below.   ### Query string parameters  Query parameters accept Elastic's query string syntax, which allows for even better flexibility.  For example above query can be rephrased as:  **HTTP**   ``` GET https://api.intel471.com/v1/reports?report=sources OR abba ```  **Python**  ``` response = titan_client.ReportsApi(api_client).reports_get(report=\"sources OR abba\") ```  More advanced combination would include both `OR` and `AND` operators and a negation:  **HTTP**  ``` GET https://api.intel471.com/v1/reports?report=(sources OR abba) AND -creaba ```  **Python**  ``` response = titan_client.ReportsApi(api_client).reports_get(report=\"(sources OR abba) AND -creaba\") ```  Means \"find me reports with `source` or `abba` in their body which at the same time do not contain `creaba`\".  The query string \"mini-language\" reference and examples can be found on  [Elastic's query string syntax](https://www.elastic.co/guide/en/elasticsearch/reference/7.5/query-dsl-query-string-query.html#query-dsl-query-string-query) page.  ## Get CVEs using multiple filtering criteria  Get all CVE reports for Chrome product where the risk is high and the patch is not available yet.  **HTTP**   ``` GET https://api.intel471.com/v1/cve/reports?productName=Chrome&riskLevel=high&patchStatus=unavailable ```  **Python**  ``` response = titan_client.VulnerabilitiesApi(api_client).cve_reports_get(     product_name=\"Chrome\",     risk_level=\"high\",     patch_status=\"unavailable\" ) ```  ## List watcher groups   **HTTP**   ``` GET https://api.intel471.com/v1/watcherGroups ```  **Python**  ``` response = titan_client.WatchersApi(api_client).watcher_groups_get() ```  ## Create watcher group   To create a watcher group you need to pass a body along with the request.  **HTTP**   ``` POST https://api.intel471.com/v1/watcherGroups {   \"name\": \"my_group_name\",   \"description\": \"My description\" } ```  **Python**  ``` response = titan_client.WatchersApi(api_client).watcher_groups_post(   {\"name\": \"my_group_name\", \"description\": \"My description\"} ) ```  ## Create free text search watcher  **HTTP**   ``` POST https://api.intel471.com/v1/watcherGroups/<GROUP UID>/watchers {   \"type\": \"search\",   \"freeTextPattern\": \"text to search\",   \"notificationChannel\": \"website\" } ```  **Python**  ``` response = titan_client.WatchersApi(api_client).watcher_groups_group_uid_watchers_post(   group_uid=\"<GROUP UID>\",   watcher_request_body_post={     \"type\": \"search\",     \"freeTextPattern\": \"text to search\",     \"notificationChannel\": \"website\"   } ) ```  ## Create specific search watcher  **HTTP**   ``` POST https://api.intel471.com/v1/watcherGroups/<GROUP UID>/watchers {   \"type\": \"search\",   \"patterns\": [     {\"types\": \"Actor\" , \"pattern\": \"swisman\"}   ],   \"notificationChannel\": \"website\" } ```  **Python**  ``` response = titan_client.WatchersApi(api_client).watcher_groups_group_uid_watchers_post(   group_uid=\"<GROUP UID>\",   watcher_request_body_post={     \"type\": \"search\",     \"patterns\": [       {\"types\": \"Actor\" , \"pattern\": \"swisman\"}     ],     \"notificationChannel\": \"website\"   } ) ```  # API integration best practice with your application CORS requests to the API are not allowed due to security concerns, so please avoid AJAX calls directly from the browser. Instead consider setting up a server side proxy in your application to handle API requests.  Please consider not storing information provided by the API locally as we are constantly improving our data set and want you to have the most updated information.  # Versioning support We consistently improve our API and occasionally introduce the changes based on the customer feedback. The current API version is provided in this documentation's header. We provide API backwards compatibility whenever possible.  All requests are prefixed with the major version number, for example `/v1`:  ``` https://api.intel471.com/v1/reports ```  Different major versions are not compatible and imply significant response structure changes. Minor versions differences might include extra fields in response or provide new request parameter support. To stick to the specific version, just add `v` parameter to the request, for example: `?v=1.19.2`. If you specify a non existing version, it will be brought down to the nearest existing one.  Omitting the version parameter in the request will call the latest version of the API.  We consistently phase out the outdated versions of the API, keeping only several most recent versions. Specific version is getting disabled only when we do not record any requests using it, so it's guaranteed that calls to the outdated ones will work, though we recommend switching to the latest one as soon as possible.  We recommend to always add the version parameter to the request to be safe on API updates in your integrations.   Python client always adds the version parameter in the underlying request. API version matches the Python client's package version.   # noqa: E501
 
     The version of the OpenAPI document: 1.19.7
     Generated by: https://openapi-generator.tech
 """
-from titan_client.titan_stix import STIXMapperSettings
+
 
 try:
     from inspect import getfullargspec
 except ImportError:
     from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
 import six
 
 from titan_client.configuration import Configuration
+from titan_client.titan_stix import STIXMapperSettings
 from titan_client.titan_stix.mappers.common import StixMapper
 
 
 class WatcherGroupsPost412Response(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -81,15 +82,14 @@
 
         return result
 
     def to_stix(self, settings: STIXMapperSettings = None):
         stix_mapper = StixMapper(settings)
         return stix_mapper.map(self.to_dict(serialize=True))
 
-
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
```

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_groups_post_request.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_groups_post_request.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,25 +4,26 @@
     Titan API v1
 
     # Introduction The Intel 471 API is organized around the principles of REST. Our API lets you gather results from our platform using anything that can send a HTTP request, including cURL and modern internet browsers. Access to this API requires an API token which is managed from your account settings.  Intel 471 reserves the right to add fields to our API however we will provide backwards compatibility and older version support so that it will be possible to choose exact versions that provide a response with an older structure.  # Authentication Authentication to the API occurs by providing your email address as the login and API key as a password in the authorization header via HTTP Basic Auth. Your API key can be found in the [API](https://portal.intel471.com/api) section on the portal. It carries many privileges so please do not expose it on public web resources.  # Accessing the API  Following examples demonstrate different methods to get the reports from `/reports` endpoint.  ## Internet browser  Just open URL: https://api.intel471.com/v1/reports  Browser will ask you for credentials, provide your email as login and API key as password.  ## cURL command line utility  Execute following command in your terminal:  ``` curl -u <YOU EMAIL>:<YOUR API KEY> https://api.intel471.com/v1/reports ```  ## Python client  We provide a [Python client](https://github.com/intel471/titan-client-python) for Intel 471's Titan API, which aims at providing common ground for all the endpoints. Please note that all the call parameters and response body fields' names are normalized to camel_case, so for example when you search reports by document type using Python client use `document_type` instead of `documentType`.  Install the client using pip (python >= 3.6 required):  ``` pip install titan-client ```  Run following script  ```python import titan_client  configuration = titan_client.Configuration(     username=\"<YOU EMAIL>\",     password=\"<YOUR API KEY>\")  with titan_client.ApiClient(configuration) as api_client:     api_instance = titan_client.ReportsApi(api_client)     api_response = api_instance.reports_get() print(api_response) ```  # Use cases  Below we present several commonly used scenarios in both raw HTTP request format and as a script using Python client. Examples are simplified so that they do not contain the authentication part and for Python client they do not contain configuration and API client object creation portion. For full example please refer to **Accessing the API** section of this document.   ## Paging  One page of the results can carry up to 100 records and you can display up to 11 pages for one query (max offset is 1000) in non-stream API endpoints. Use `count` parameter to set the number of items per page. Use `offset` parameter to shift the window by given number of results.       **HTTP**   ``` # Get 20 reports, sorted by the default field GET https://api.intel471.com/v1/reports?count=20  # Get next 20 reports GET https://api.intel471.com/v1/reports?count=20&offset=20  # Get 40 reports in one go to save API calls GET https://api.intel471.com/v1/reports?count=40 ```  **Python**  ``` response = titan_client.ReportsApi(api_client).reports_get(count=20, offset=20) ```  ## Paging beyond the max allowed offset  Paging described in the previous use case is generally sufficient for most needs. If there are more than 1100 objects  to be obtained for a given time period and set of filter criteria, then it is possible to move the filter timestamps  along and then restart the offset sequencing. There is a very small number of situations where this may cause issues,  where there is multiple objects with the same timestamp adjacent to the last object in the response.  For the higher volume or fast changing data (such as malware indicators, malware events, creds) there are stream API endpoints  available where cursors may be used in order to acquire data easily and to avoid the need to shift timestamp ranges.  ``` # Get first 11 pages, 100 objects each  GET https://api.intel471.com/v1/reports?sort=latest&count=100 GET https://api.intel471.com/v1/reports?sort=latest&count=100&offset=100 ... GET https://api.intel471.com/v1/reports?sort=latest&count=100&offset=1000 ... > {\"reports\": [{..., \"created\": 1661867086000}, {..., \"created\": 1661864268000}]} ```  Then the `created` time value from the last response will be used as an upper limit in the next series of calls:  ```   GET https://api.intel471.com/v1/reports?sort=latest&until=1661864268000&count=100 GET https://api.intel471.com/v1/reports?sort=latest&until=1661864268000&offset=100 ... GET https://api.intel471.com/v1/reports?sort=latest&until=1661864268000&offset=1000 ```  And so on, until the results are available or until the desired number of objects has been fetched.  ## Paging /alerts endpoint  Alerts endpoint differs from all the other non-stream API endpoints in that the `offset` parameter needs to be set  to the uid of the most recent acquired alert instead of an integer indicating the shift.  **HTTP**   ``` GET https://api.intel471.com/v1/alerts?count=100 > {\"alerts\": [{..., \"uid\": \"abc123\"}, {..., \"uid\": \"abc234\"}]}  GET https://api.intel471.com/v1/alerts?count=100&offset=abc234 > {\"alerts\": [{..., \"uid\": \"abc345\"}, {..., \"uid\": \"abc456\"}]} ```  **Python**  ``` response = titan_client.AlertsApi(api_client).alerts_get(count=100, offset=\"abc456\") ```  ## Stream endpoints paging  Stream endpoints provide the same data as their regular counterparts but they differ in a way of paging.  When working with a stream endpoint, the response always contains `cursorNext` field, which should be provided to the next subsequent  call to fetch potential next page of the results. All the subsequent calls should have the same set of query parameters as the first one,  except the cursor value. Keep calling the endpoint with a new cursor value until it stops yielding results. When new data appear after that, another call will fetch it.  **HTTP**   ``` GET https://api.intel471.com/v1/indicators/stream?lastUpdatedFrom=1655809200000 > {\"indicators\": [...], \"cursorNext\": \"MTY1NT1\"}  GET https://api.intel471.com/v1/indicators/stream?lastUpdatedFrom=1655809200000&cursor=MTY1NT1 > {\"indicators\": [...], \"cursorNext\": \"MTY1NT2\"}  GET https://api.intel471.com/v1/indicators/stream?lastUpdatedFrom=1655809200000&cursor=MTY1NT2 > {\"cursorNext\": \"MTY1NT3\"} ```  **Python**  ``` response = titan_client.IndicatorsApi(api_client).indicators_stream_get(last_updated_from=1656809200000) print(response.cursor_next, response.indicators) # MTY1NT1, [...]  response = titan_client.IndicatorsApi(api_client).indicators_stream_get(last_updated_from=1656809200000, cursor=\"MTY1NT1\")) print(response.cursor_next, response.indicators) # MTY1NT2, [...]  response = titan_client.IndicatorsApi(api_client).indicators_stream_get(last_updated_from=1656809200000, cursor=\"MTY1NT2\")) print(response.cursor_next, response.indicators) # MTY1NT3, None ```  ## Querying using logical operators  ### Array parameters  Any query parameter can be singular or array, if multiple parameters with the same name were provided. All parameters with the same name are internally combined into a query with `AND` operator.  So following query:  ``` GET https://api.intel471.com/v1/reports?report=sources&report=abba ```  Means \"find me reports with `source` AND `abba` in their body\".  This approach is not supported in the Python client. Instead use query string method discussed below.   ### Query string parameters  Query parameters accept Elastic's query string syntax, which allows for even better flexibility.  For example above query can be rephrased as:  **HTTP**   ``` GET https://api.intel471.com/v1/reports?report=sources OR abba ```  **Python**  ``` response = titan_client.ReportsApi(api_client).reports_get(report=\"sources OR abba\") ```  More advanced combination would include both `OR` and `AND` operators and a negation:  **HTTP**  ``` GET https://api.intel471.com/v1/reports?report=(sources OR abba) AND -creaba ```  **Python**  ``` response = titan_client.ReportsApi(api_client).reports_get(report=\"(sources OR abba) AND -creaba\") ```  Means \"find me reports with `source` or `abba` in their body which at the same time do not contain `creaba`\".  The query string \"mini-language\" reference and examples can be found on  [Elastic's query string syntax](https://www.elastic.co/guide/en/elasticsearch/reference/7.5/query-dsl-query-string-query.html#query-dsl-query-string-query) page.  ## Get CVEs using multiple filtering criteria  Get all CVE reports for Chrome product where the risk is high and the patch is not available yet.  **HTTP**   ``` GET https://api.intel471.com/v1/cve/reports?productName=Chrome&riskLevel=high&patchStatus=unavailable ```  **Python**  ``` response = titan_client.VulnerabilitiesApi(api_client).cve_reports_get(     product_name=\"Chrome\",     risk_level=\"high\",     patch_status=\"unavailable\" ) ```  ## List watcher groups   **HTTP**   ``` GET https://api.intel471.com/v1/watcherGroups ```  **Python**  ``` response = titan_client.WatchersApi(api_client).watcher_groups_get() ```  ## Create watcher group   To create a watcher group you need to pass a body along with the request.  **HTTP**   ``` POST https://api.intel471.com/v1/watcherGroups {   \"name\": \"my_group_name\",   \"description\": \"My description\" } ```  **Python**  ``` response = titan_client.WatchersApi(api_client).watcher_groups_post(   {\"name\": \"my_group_name\", \"description\": \"My description\"} ) ```  ## Create free text search watcher  **HTTP**   ``` POST https://api.intel471.com/v1/watcherGroups/<GROUP UID>/watchers {   \"type\": \"search\",   \"freeTextPattern\": \"text to search\",   \"notificationChannel\": \"website\" } ```  **Python**  ``` response = titan_client.WatchersApi(api_client).watcher_groups_group_uid_watchers_post(   group_uid=\"<GROUP UID>\",   watcher_request_body_post={     \"type\": \"search\",     \"freeTextPattern\": \"text to search\",     \"notificationChannel\": \"website\"   } ) ```  ## Create specific search watcher  **HTTP**   ``` POST https://api.intel471.com/v1/watcherGroups/<GROUP UID>/watchers {   \"type\": \"search\",   \"patterns\": [     {\"types\": \"Actor\" , \"pattern\": \"swisman\"}   ],   \"notificationChannel\": \"website\" } ```  **Python**  ``` response = titan_client.WatchersApi(api_client).watcher_groups_group_uid_watchers_post(   group_uid=\"<GROUP UID>\",   watcher_request_body_post={     \"type\": \"search\",     \"patterns\": [       {\"types\": \"Actor\" , \"pattern\": \"swisman\"}     ],     \"notificationChannel\": \"website\"   } ) ```  # API integration best practice with your application CORS requests to the API are not allowed due to security concerns, so please avoid AJAX calls directly from the browser. Instead consider setting up a server side proxy in your application to handle API requests.  Please consider not storing information provided by the API locally as we are constantly improving our data set and want you to have the most updated information.  # Versioning support We consistently improve our API and occasionally introduce the changes based on the customer feedback. The current API version is provided in this documentation's header. We provide API backwards compatibility whenever possible.  All requests are prefixed with the major version number, for example `/v1`:  ``` https://api.intel471.com/v1/reports ```  Different major versions are not compatible and imply significant response structure changes. Minor versions differences might include extra fields in response or provide new request parameter support. To stick to the specific version, just add `v` parameter to the request, for example: `?v=1.19.2`. If you specify a non existing version, it will be brought down to the nearest existing one.  Omitting the version parameter in the request will call the latest version of the API.  We consistently phase out the outdated versions of the API, keeping only several most recent versions. Specific version is getting disabled only when we do not record any requests using it, so it's guaranteed that calls to the outdated ones will work, though we recommend switching to the latest one as soon as possible.  We recommend to always add the version parameter to the request to be safe on API updates in your integrations.   Python client always adds the version parameter in the underlying request. API version matches the Python client's package version.   # noqa: E501
 
     The version of the OpenAPI document: 1.19.7
     Generated by: https://openapi-generator.tech
 """
-from titan_client.titan_stix import STIXMapperSettings
+
 
 try:
     from inspect import getfullargspec
 except ImportError:
     from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
 import six
 
 from titan_client.configuration import Configuration
+from titan_client.titan_stix import STIXMapperSettings
 from titan_client.titan_stix.mappers.common import StixMapper
 
 
 class WatcherGroupsPostRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -139,15 +140,14 @@
 
         return result
 
     def to_stix(self, settings: STIXMapperSettings = None):
         stix_mapper = StixMapper(settings)
         return stix_mapper.map(self.to_dict(serialize=True))
 
-
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
```

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_request_body.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_request_body.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_request_body_filters.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_request_body_filters.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_request_body_filters_inner.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_request_body_filters_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_request_body_patterns.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_request_body_patterns.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_request_body_patterns_inner.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_request_body_patterns_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_request_body_post.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_request_body_post.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_request_body_post_all_of.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_request_body_post_all_of.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_request_body_put.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_request_body_put.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_request_body_put_all_of.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_request_body_put_all_of.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_schema.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_schema_filters.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_schema_filters.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_schema_filters_inner.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_schema_filters_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_schema_forum.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_schema_forum.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_schema_links.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_schema_links.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_schema_links_inner.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_schema_links_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_schema_links_inner_forum.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_schema_links_inner_forum.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_schema_links_inner_thread.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_schema_links_inner_thread.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_schema_patterns.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_schema_patterns.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_schema_patterns_inner.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_schema_patterns_inner.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_schema_response.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_schema_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/watcher_schema_thread.py` & `Titan Client-1.19.7.1/titan_client/models/watcher_schema_thread.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/yara_search_response.py` & `Titan Client-1.19.7.1/titan_client/models/yara_search_response.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/yara_search_schema.py` & `Titan Client-1.19.7.1/titan_client/models/yara_search_schema.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/yara_search_schema_activity.py` & `Titan Client-1.19.7.1/titan_client/models/yara_search_schema_activity.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/yara_search_schema_data.py` & `Titan Client-1.19.7.1/titan_client/models/yara_search_schema_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/yara_search_schema_data_threat.py` & `Titan Client-1.19.7.1/titan_client/models/yara_search_schema_data_threat.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/yara_search_schema_data_threat_data.py` & `Titan Client-1.19.7.1/titan_client/models/yara_search_schema_data_threat_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/yara_search_schema_data_yara_data.py` & `Titan Client-1.19.7.1/titan_client/models/yara_search_schema_data_yara_data.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/models/yara_search_schema_meta.py` & `Titan Client-1.19.7.1/titan_client/models/yara_search_schema_meta.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/rest.py` & `Titan Client-1.19.7.1/titan_client/rest.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/titan_stix/__init__.py` & `Titan Client-1.19.7.1/titan_client/titan_stix/__init__.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/titan_stix/mappers/common.py` & `Titan Client-1.19.7.1/titan_client/titan_stix/mappers/common.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/titan_stix/mappers/cves.py` & `Titan Client-1.19.7.1/titan_client/titan_stix/mappers/cves.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/titan_stix/mappers/indicators.py` & `Titan Client-1.19.7.1/titan_client/titan_stix/mappers/indicators.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/titan_stix/mappers/iocs.py` & `Titan Client-1.19.7.1/titan_client/titan_stix/mappers/iocs.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/titan_stix/mappers/reports.py` & `Titan Client-1.19.7.1/titan_client/titan_stix/mappers/reports.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/titan_stix/mappers/yara.py` & `Titan Client-1.19.7.1/titan_client/titan_stix/mappers/yara.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/titan_stix/observables.py` & `Titan Client-1.19.7.1/titan_client/titan_stix/observables.py`

 * *Files identical despite different names*

### Comparing `Titan Client-1.19.7/titan_client/titan_stix/patterning.py` & `Titan Client-1.19.7.1/titan_client/titan_stix/patterning.py`

 * *Files identical despite different names*

