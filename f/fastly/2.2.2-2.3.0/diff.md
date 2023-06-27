# Comparing `tmp/fastly-2.2.2.tar.gz` & `tmp/fastly-2.3.0.tar.gz`

## Comparing `fastly-2.2.2.tar` & `fastly-2.3.0.tar`

### file list

```diff
@@ -1,1449 +1,1449 @@
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 fastly-2.2.2/.gitlab-ci.yml
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 fastly-2.2.2/CHANGELOG.md
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 fastly-2.2.2/MANIFEST.in
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 fastly-2.2.2/SECURITY.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fastly-2.2.2/requirements.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fastly-2.2.2/setup.cfg
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 fastly-2.2.2/setup.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastly-2.2.2/sig.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 fastly-2.2.2/test-requirements.txt
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 fastly-2.2.2/tox.ini
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 fastly-2.2.2/.github/ISSUE_TEMPLATE/bug_report.md
--rwxr-xr-x   0        0        0      619 2020-02-02 00:00:00.000000 fastly-2.2.2/.github/scripts/pack.sh
--rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 fastly-2.2.2/.github/scripts/prepare.sh
--rwxr-xr-x   0        0        0      812 2020-02-02 00:00:00.000000 fastly-2.2.2/.github/scripts/publish_env.sh
--rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 fastly-2.2.2/.github/scripts/release_body.sh
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 fastly-2.2.2/.github/workflows/ci-release.yaml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Acl.md
--rw-r--r--   0        0        0    15695 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/AclApi.md
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/AclEntry.md
--rw-r--r--   0        0        0    20447 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/AclEntryApi.md
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/AclEntryResponse.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/AclEntryResponseAllOf.md
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/AclResponse.md
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/AclResponseAllOf.md
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ApexRedirect.md
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ApexRedirectAllOf.md
--rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ApexRedirectApi.md
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/AwsRegion.md
--rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Backend.md
--rw-r--r--   0        0        0    38268 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BackendApi.md
--rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BackendResponse.md
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BackendResponseAllOf.md
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Billing.md
--rw-r--r--   0        0        0    13259 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BillingAddressApi.md
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BillingAddressAttributes.md
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BillingAddressRequest.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BillingAddressRequestData.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BillingAddressResponse.md
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BillingAddressResponseData.md
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BillingAddressVerificationErrorResponse.md
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BillingAddressVerificationErrorResponseErrors.md
--rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BillingApi.md
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BillingEstimateResponse.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BillingEstimateResponseAllOf.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BillingEstimateResponseAllOfLine.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BillingEstimateResponseAllOfLines.md
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BillingResponse.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BillingResponseAllOf.md
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BillingResponseLineItem.md
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BillingResponseLineItemAllOf.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BillingStatus.md
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BillingTotal.md
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BillingTotalExtras.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BulkUpdateAclEntriesRequest.md
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BulkUpdateAclEntry.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BulkUpdateAclEntryAllOf.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BulkUpdateConfigStoreItem.md
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BulkUpdateConfigStoreItemAllOf.md
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BulkUpdateConfigStoreListRequest.md
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BulkUpdateDictionaryItem.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BulkUpdateDictionaryListRequest.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BulkWafActiveRule.md
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/BulkWafActiveRules.md
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/CacheSetting.md
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/CacheSettingResponse.md
--rw-r--r--   0        0        0    18846 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/CacheSettingsApi.md
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Condition.md
--rw-r--r--   0        0        0    17741 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ConditionApi.md
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ConditionResponse.md
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ConditionsResponse.md
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ConfigStore.md
--rw-r--r--   0        0        0    18464 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ConfigStoreApi.md
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ConfigStoreInfoResponse.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ConfigStoreItem.md
--rw-r--r--   0        0        0    23504 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ConfigStoreItemApi.md
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ConfigStoreItemResponse.md
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ConfigStoreItemResponseAllOf.md
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ConfigStoreResponse.md
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ConfigStoreResponseAllOf.md
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Contact.md
--rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ContactApi.md
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ContactResponse.md
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ContactResponseAllOf.md
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Content.md
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ContentApi.md
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Customer.md
--rw-r--r--   0        0        0    18926 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/CustomerApi.md
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/CustomerResponse.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/CustomerResponseAllOf.md
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Dictionary.md
--rw-r--r--   0        0        0    17237 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DictionaryApi.md
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DictionaryInfoApi.md
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DictionaryInfoResponse.md
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DictionaryItem.md
--rw-r--r--   0        0        0    26138 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DictionaryItemApi.md
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DictionaryItemResponse.md
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DictionaryItemResponseAllOf.md
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DictionaryResponse.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DictionaryResponseAllOf.md
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DiffApi.md
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DiffResponse.md
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Director.md
--rw-r--r--   0        0        0    15015 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DirectorApi.md
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DirectorBackend.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DirectorBackendAllOf.md
--rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DirectorBackendApi.md
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DirectorResponse.md
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Domain.md
--rw-r--r--   0        0        0    21769 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DomainApi.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DomainCheckItem.md
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DomainCheckResponse.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DomainCheckResponseList.md
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DomainOwnershipsApi.md
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DomainResponse.md
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/DomainsResponse.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/EnabledProductResponse.md
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/EnabledProductResponseLinks.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/EnabledProductResponseProduct.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/EnabledProductResponseService.md
--rw-r--r--   0        0        0     8351 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/EnabledProductsApi.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Event.md
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/EventAttributes.md
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/EventResponse.md
--rw-r--r--   0        0        0     7243 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/EventsApi.md
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/EventsResponse.md
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/EventsResponseAllOf.md
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/GenericTokenError.md
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Gzip.md
--rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/GzipApi.md
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/GzipResponse.md
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Header.md
--rw-r--r--   0        0        0    20925 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HeaderApi.md
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HeaderResponse.md
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Healthcheck.md
--rw-r--r--   0        0        0    20120 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HealthcheckApi.md
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HealthcheckResponse.md
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Historical.md
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalAggregateResponse.md
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalAggregateResponseAllOf.md
--rw-r--r--   0        0        0    39081 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalApi.md
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalFieldAggregateResponse.md
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalFieldAggregateResponseAllOf.md
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalFieldResponse.md
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalFieldResponseDataField.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalFieldResults.md
--rw-r--r--   0        0        0    27260 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalFieldResultsAttributes.md
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalFieldResultsAttributesAllOf.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalMeta.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalRegionsResponse.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalRegionsResponseAllOf.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalResponse.md
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalResponseDataField.md
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalResults.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalService.md
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalServices.md
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalUsageAggregateResponse.md
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalUsageMonthResponse.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalUsageMonthResponseAllOf.md
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalUsageMonthResponseData.md
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalUsageResults.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalUsageServiceResponse.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HistoricalUsageServiceResponseAllOf.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Http3.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Http3AllOf.md
--rw-r--r--   0        0        0     9629 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Http3Api.md
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HttpResponseFormat.md
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/HttpStreamFormat.md
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/IamPermission.md
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/IamPermissionsApi.md
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/IamRole.md
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/IamRoleAllOf.md
--rw-r--r--   0        0        0     9918 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/IamRolesApi.md
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/IamServiceGroup.md
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/IamServiceGroupAllOf.md
--rw-r--r--   0        0        0    11406 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/IamServiceGroupsApi.md
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/IamUserGroup.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/IamUserGroupAllOf.md
--rw-r--r--   0        0        0    17911 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/IamUserGroupsApi.md
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/IncludedWithWafActiveRule.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/IncludedWithWafActiveRuleItem.md
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/IncludedWithWafExclusion.md
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/IncludedWithWafExclusionItem.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/IncludedWithWafFirewall.md
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/IncludedWithWafFirewallVersion.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/IncludedWithWafFirewallVersionItem.md
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/IncludedWithWafRule.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/IncludedWithWafRuleItem.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/IncludedWithWafRuleRevision.md
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/InlineObject.md
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/InlineObject1.md
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/InlineResponse200.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/InlineResponse2001.md
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/InlineResponse2002.md
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/InlineResponse2002Meta.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/InlineResponse2003.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/InlineResponse2003Meta.md
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Invitation.md
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/InvitationData.md
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/InvitationDataAttributes.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/InvitationResponse.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/InvitationResponseAllOf.md
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/InvitationResponseData.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/InvitationResponseDataAllOf.md
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/InvitationsApi.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/InvitationsResponse.md
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/InvitationsResponseAllOf.md
--rw-r--r--   0        0        0     9883 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/KvStoreApi.md
--rw-r--r--   0        0        0    12230 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/KvStoreItemApi.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingAddressAndPort.md
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingAzureblob.md
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingAzureblobAllOf.md
--rw-r--r--   0        0        0    29125 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingAzureblobApi.md
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingAzureblobResponse.md
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingBigquery.md
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingBigqueryAllOf.md
--rw-r--r--   0        0        0    24678 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingBigqueryApi.md
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingBigqueryResponse.md
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingCloudfiles.md
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingCloudfilesAllOf.md
--rw-r--r--   0        0        0    27524 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingCloudfilesApi.md
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingCloudfilesResponse.md
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingCommon.md
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingDatadog.md
--rw-r--r--   0        0        0     3883 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingDatadogAllOf.md
--rw-r--r--   0        0        0    38955 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingDatadogApi.md
--rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingDatadogResponse.md
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingDigitalocean.md
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingDigitaloceanAllOf.md
--rw-r--r--   0        0        0    28174 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingDigitaloceanApi.md
--rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingDigitaloceanResponse.md
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingElasticsearch.md
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingElasticsearchAllOf.md
--rw-r--r--   0        0        0    30259 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingElasticsearchApi.md
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingElasticsearchResponse.md
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingFormatVersion.md
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingFtp.md
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingFtpAllOf.md
--rw-r--r--   0        0        0    27244 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingFtpApi.md
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingFtpResponse.md
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingGcs.md
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingGcsAllOf.md
--rw-r--r--   0        0        0    28487 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingGcsApi.md
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingGcsCommon.md
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingGcsResponse.md
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingGenericCommon.md
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingGooglePubsub.md
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingGooglePubsubAllOf.md
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingGooglePubsubResponse.md
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingHeroku.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingHerokuAllOf.md
--rw-r--r--   0        0        0    21127 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingHerokuApi.md
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingHerokuResponse.md
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingHoneycomb.md
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingHoneycombAllOf.md
--rw-r--r--   0        0        0    20986 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingHoneycombApi.md
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingHoneycombResponse.md
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingHttps.md
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingHttpsAllOf.md
--rw-r--r--   0        0        0    29036 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingHttpsApi.md
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingHttpsResponse.md
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingKafka.md
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingKafkaAllOf.md
--rw-r--r--   0        0        0    18733 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingKafkaApi.md
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingKafkaResponse.md
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingKinesis.md
--rw-r--r--   0        0        0    17289 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingKinesisApi.md
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingKinesisResponse.md
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingLogentries.md
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingLogentriesAllOf.md
--rw-r--r--   0        0        0    22258 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingLogentriesApi.md
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingLogentriesResponse.md
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingLoggly.md
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingLogglyAllOf.md
--rw-r--r--   0        0        0    20871 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingLogglyApi.md
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingLogglyResponse.md
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingLogshuttle.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingLogshuttleAllOf.md
--rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingLogshuttleApi.md
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingLogshuttleResponse.md
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingMessageType.md
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingNewrelic.md
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingNewrelicAllOf.md
--rw-r--r--   0        0        0    25794 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingNewrelicApi.md
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingNewrelicResponse.md
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingOpenstack.md
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingOpenstackAllOf.md
--rw-r--r--   0        0        0    27216 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingOpenstackApi.md
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingOpenstackResponse.md
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingPapertrail.md
--rw-r--r--   0        0        0    21189 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingPapertrailApi.md
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingPapertrailResponse.md
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingPlacement.md
--rw-r--r--   0        0        0    24358 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingPubsubApi.md
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingRequestCapsCommon.md
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingS3.md
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingS3AllOf.md
--rw-r--r--   0        0        0    31697 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingS3Api.md
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingS3Response.md
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingScalyr.md
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingScalyrAllOf.md
--rw-r--r--   0        0        0    21715 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingScalyrApi.md
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingScalyrResponse.md
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingSftp.md
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingSftpAllOf.md
--rw-r--r--   0        0        0    28475 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingSftpApi.md
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingSftpResponse.md
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingSplunk.md
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingSplunkAllOf.md
--rw-r--r--   0        0        0    26444 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingSplunkApi.md
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingSplunkResponse.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingSumologic.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingSumologicAllOf.md
--rw-r--r--   0        0        0    21088 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingSumologicApi.md
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingSumologicResponse.md
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingSyslog.md
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingSyslogAllOf.md
--rw-r--r--   0        0        0    26805 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingSyslogApi.md
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingSyslogResponse.md
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingTlsCommon.md
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/LoggingUseTls.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/MutualAuthentication.md
--rw-r--r--   0        0        0    17143 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/MutualAuthenticationApi.md
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/MutualAuthenticationData.md
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/MutualAuthenticationDataAttributes.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/MutualAuthenticationResponse.md
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/MutualAuthenticationResponseAttributes.md
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/MutualAuthenticationResponseAttributesAllOf.md
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/MutualAuthenticationResponseData.md
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/MutualAuthenticationResponseDataAllOf.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/MutualAuthenticationsResponse.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/MutualAuthenticationsResponseAllOf.md
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/NumberVersion.md
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Package.md
--rw-r--r--   0        0        0     6678 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PackageApi.md
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PackageMetadata.md
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PackageResponse.md
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PackageResponseAllOf.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Pagination.md
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PaginationLinks.md
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PaginationMeta.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Permission.md
--rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Pool.md
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PoolAllOf.md
--rw-r--r--   0        0        0    29387 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PoolApi.md
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PoolResponse.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PoolResponseAllOf.md
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Pop.md
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PopApi.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PopCoordinates.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PublicIpList.md
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PublicIpListApi.md
--rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PublishApi.md
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PublishItem.md
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PublishItemFormats.md
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PublishRequest.md
--rw-r--r--   0        0        0    10418 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PurgeApi.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PurgeKeys.md
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PurgeKeysResponse.md
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/PurgeResponse.md
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RateLimiter.md
--rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RateLimiterApi.md
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RateLimiterResponse.md
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RateLimiterResponse1.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RateLimiterResponseAllOf.md
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Realtime.md
--rw-r--r--   0        0        0     8759 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RealtimeApi.md
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RealtimeEntry.md
--rw-r--r--   0        0        0    27336 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RealtimeMeasurements.md
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipCommonName.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipCustomer.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipCustomerCustomer.md
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMemberCustomer.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMemberMutualAuthentication.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMemberService.md
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMemberServiceInvitation.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMemberTlsActivation.md
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMemberTlsBulkCertificate.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMemberTlsCertificate.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMemberTlsConfiguration.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMemberTlsDnsRecord.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMemberTlsDomain.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMemberTlsPrivateKey.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMemberTlsSubscription.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMemberWafActiveRule.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMemberWafFirewall.md
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMemberWafFirewallVersion.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMemberWafRule.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMemberWafRuleRevision.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMemberWafTag.md
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMutualAuthentication.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMutualAuthenticationMutualAuthentication.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMutualAuthentications.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipMutualAuthenticationsMutualAuthentications.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipService.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipServiceInvitations.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipServiceInvitationsCreate.md
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipServiceInvitationsCreateServiceInvitations.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipServiceInvitationsServiceInvitations.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipServices.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipServicesServices.md
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsActivation.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsActivationTlsActivation.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsActivations.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsBulkCertificate.md
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsBulkCertificateTlsBulkCertificate.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsBulkCertificates.md
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsCertificate.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsCertificateTlsCertificate.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsCertificates.md
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsCertificatesTlsCertificates.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsConfiguration.md
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsConfigurationForTlsSubscription.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsConfigurationTlsConfiguration.md
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsConfigurations.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsConfigurationsTlsConfigurations.md
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsDnsRecord.md
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsDnsRecordDnsRecord.md
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsDnsRecords.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsDomain.md
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsDomainTlsDomain.md
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsDomains.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsDomainsTlsDomains.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsPrivateKey.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsPrivateKeyTlsPrivateKey.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsPrivateKeys.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsPrivateKeysTlsPrivateKeys.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsSubscription.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsSubscriptionTlsSubscription.md
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipTlsSubscriptions.md
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipUser.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipUserUser.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipWafActiveRules.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipWafActiveRulesWafActiveRules.md
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipWafFirewall.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipWafFirewallVersion.md
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipWafFirewallVersionWafFirewallVersion.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipWafFirewallVersions.md
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipWafFirewallWafFirewall.md
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipWafRule.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipWafRuleRevision.md
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipWafRuleRevisionWafRuleRevisions.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipWafRuleRevisions.md
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipWafRuleWafRule.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipWafRules.md
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipWafTags.md
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipWafTagsWafTags.md
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipsForInvitation.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipsForMutualAuthentication.md
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipsForStar.md
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipsForTlsActivation.md
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipsForTlsBulkCertificate.md
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipsForTlsConfiguration.md
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipsForTlsDomain.md
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipsForTlsPrivateKey.md
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipsForTlsSubscription.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipsForWafActiveRule.md
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipsForWafExclusion.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipsForWafFirewallVersion.md
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RelationshipsForWafRule.md
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RequestSettings.md
--rw-r--r--   0        0        0    15635 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RequestSettingsApi.md
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RequestSettingsResponse.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Resource.md
--rw-r--r--   0        0        0    15552 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ResourceApi.md
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ResourceResponse.md
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ResourceResponseAllOf.md
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ResponseObject.md
--rw-r--r--   0        0        0     8900 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ResponseObjectApi.md
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ResponseObjectResponse.md
--rw-r--r--   0        0        0    27224 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Results.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/RoleUser.md
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/SchemasContactResponse.md
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/SchemasSnippetResponse.md
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/SchemasUserResponse.md
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/SchemasVclResponse.md
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/SchemasVersion.md
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/SchemasVersionResponse.md
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/SchemasWafFirewallVersion.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/SchemasWafFirewallVersionData.md
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Server.md
--rw-r--r--   0        0        0    19968 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServerApi.md
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServerResponse.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServerResponseAllOf.md
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Service.md
--rw-r--r--   0        0        0    22475 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceApi.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceAuthorization.md
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceAuthorizationData.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceAuthorizationDataAttributes.md
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceAuthorizationDataRelationships.md
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceAuthorizationDataRelationshipsUser.md
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceAuthorizationDataRelationshipsUserData.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceAuthorizationResponse.md
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceAuthorizationResponseData.md
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceAuthorizationResponseDataAllOf.md
--rw-r--r--   0        0        0    16177 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceAuthorizationsApi.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceAuthorizationsResponse.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceAuthorizationsResponseAllOf.md
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceCreate.md
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceCreateAllOf.md
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceDetail.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceDetailAllOf.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceIdAndVersion.md
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceInvitation.md
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceInvitationData.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceInvitationDataAttributes.md
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceInvitationDataRelationships.md
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceInvitationResponse.md
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceInvitationResponseAllOf.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceInvitationResponseAllOfData.md
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceListResponse.md
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceListResponseAllOf.md
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceResponse.md
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceResponseAllOf.md
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceVersionDetail.md
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ServiceVersionDetailOrNull.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Settings.md
--rw-r--r--   0        0        0     7419 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/SettingsApi.md
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/SettingsResponse.md
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Snippet.md
--rw-r--r--   0        0        0    19437 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/SnippetApi.md
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/SnippetResponse.md
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/SnippetResponseAllOf.md
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Star.md
--rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/StarApi.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/StarData.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/StarResponse.md
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/StarResponseAllOf.md
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Stats.md
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/StatsApi.md
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Store.md
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/StoreResponse.md
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Timestamps.md
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TimestampsNoDelete.md
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsActivation.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsActivationData.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsActivationResponse.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsActivationResponseData.md
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsActivationResponseDataAllOf.md
--rw-r--r--   0        0        0    16586 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsActivationsApi.md
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsActivationsResponse.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsActivationsResponseAllOf.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsBulkCertificate.md
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsBulkCertificateData.md
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsBulkCertificateDataAttributes.md
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsBulkCertificateResponse.md
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsBulkCertificateResponseAttributes.md
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsBulkCertificateResponseAttributesAllOf.md
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsBulkCertificateResponseData.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsBulkCertificateResponseDataAllOf.md
--rw-r--r--   0        0        0    16217 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsBulkCertificatesApi.md
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsBulkCertificatesResponse.md
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsBulkCertificatesResponseAllOf.md
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsCertificate.md
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsCertificateData.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsCertificateDataAttributes.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsCertificateResponse.md
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsCertificateResponseAttributes.md
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsCertificateResponseAttributesAllOf.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsCertificateResponseData.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsCertificateResponseDataAllOf.md
--rw-r--r--   0        0        0    17205 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsCertificatesApi.md
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsCertificatesResponse.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsCertificatesResponseAllOf.md
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsCommon.md
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsConfiguration.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsConfigurationData.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsConfigurationDataAttributes.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsConfigurationResponse.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsConfigurationResponseAttributes.md
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsConfigurationResponseAttributesAllOf.md
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsConfigurationResponseData.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsConfigurationResponseDataAllOf.md
--rw-r--r--   0        0        0    10339 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsConfigurationsApi.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsConfigurationsResponse.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsConfigurationsResponseAllOf.md
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsDnsRecord.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsDomainData.md
--rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsDomainsApi.md
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsDomainsResponse.md
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsDomainsResponseAllOf.md
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsPrivateKey.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsPrivateKeyData.md
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsPrivateKeyDataAttributes.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsPrivateKeyResponse.md
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsPrivateKeyResponseAttributes.md
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsPrivateKeyResponseAttributesAllOf.md
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsPrivateKeyResponseData.md
--rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsPrivateKeysApi.md
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsPrivateKeysResponse.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsPrivateKeysResponseAllOf.md
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsSubscription.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsSubscriptionData.md
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsSubscriptionDataAttributes.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsSubscriptionResponse.md
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsSubscriptionResponseAttributes.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsSubscriptionResponseAttributesAllOf.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsSubscriptionResponseData.md
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsSubscriptionResponseDataAllOf.md
--rw-r--r--   0        0        0    26148 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsSubscriptionsApi.md
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsSubscriptionsResponse.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TlsSubscriptionsResponseAllOf.md
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Token.md
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TokenCreatedResponse.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TokenCreatedResponseAllOf.md
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TokenResponse.md
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TokenResponseAllOf.md
--rw-r--r--   0        0        0    14773 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TokensApi.md
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeBillingAddress.md
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeContact.md
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeCustomer.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeEvent.md
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeInvitation.md
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeMutualAuthentication.md
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeResource.md
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeService.md
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeServiceAuthorization.md
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeServiceInvitation.md
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeStar.md
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeTlsActivation.md
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeTlsBulkCertificate.md
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeTlsCertificate.md
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeTlsConfiguration.md
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeTlsDnsRecord.md
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeTlsDomain.md
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeTlsPrivateKey.md
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeTlsSubscription.md
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeUser.md
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeWafActiveRule.md
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeWafExclusion.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeWafFirewall.md
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeWafFirewallVersion.md
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeWafRule.md
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeWafRuleRevision.md
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/TypeWafTag.md
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/UpdateBillingAddressRequest.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/UpdateBillingAddressRequestData.md
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/User.md
--rw-r--r--   0        0        0    20765 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/UserApi.md
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/UserResponse.md
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/UserResponseAllOf.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ValidatorResult.md
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/ValidatorResultMessages.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Vcl.md
--rw-r--r--   0        0        0    32742 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/VclApi.md
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/VclDiff.md
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/VclDiffApi.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/VclResponse.md
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/Version.md
--rw-r--r--   0        0        0    26131 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/VersionApi.md
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/VersionCreateResponse.md
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/VersionDetail.md
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/VersionDetailSettings.md
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/VersionResponse.md
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/VersionResponseAllOf.md
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafActiveRule.md
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafActiveRuleCreationResponse.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafActiveRuleData.md
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafActiveRuleDataAttributes.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafActiveRuleResponse.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafActiveRuleResponseData.md
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafActiveRuleResponseDataAllOf.md
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafActiveRuleResponseDataAttributes.md
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafActiveRuleResponseDataAttributesAllOf.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafActiveRuleResponseDataRelationships.md
--rw-r--r--   0        0        0    27789 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafActiveRulesApi.md
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafActiveRulesResponse.md
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafActiveRulesResponseAllOf.md
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafExclusion.md
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafExclusionData.md
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafExclusionDataAttributes.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafExclusionResponse.md
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafExclusionResponseData.md
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafExclusionResponseDataAllOf.md
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafExclusionResponseDataAttributes.md
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafExclusionResponseDataAttributesAllOf.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafExclusionResponseDataRelationships.md
--rw-r--r--   0        0        0    19155 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafExclusionsApi.md
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafExclusionsResponse.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafExclusionsResponseAllOf.md
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewall.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewallData.md
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewallDataAttributes.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewallResponse.md
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewallResponseData.md
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewallResponseDataAllOf.md
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewallResponseDataAttributes.md
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewallResponseDataAttributesAllOf.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewallVersion.md
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewallVersionData.md
--rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewallVersionDataAttributes.md
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewallVersionResponse.md
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewallVersionResponseData.md
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewallVersionResponseDataAllOf.md
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewallVersionResponseDataAttributes.md
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewallVersionResponseDataAttributesAllOf.md
--rw-r--r--   0        0        0    24852 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewallVersionsApi.md
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewallVersionsResponse.md
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewallVersionsResponseAllOf.md
--rw-r--r--   0        0        0    17211 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewallsApi.md
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewallsResponse.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafFirewallsResponseAllOf.md
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafRule.md
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafRuleAttributes.md
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafRuleResponse.md
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafRuleResponseData.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafRuleResponseDataAllOf.md
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafRuleRevision.md
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafRuleRevisionAttributes.md
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafRuleRevisionOrLatest.md
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafRuleRevisionResponse.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafRuleRevisionResponseData.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafRuleRevisionResponseDataAllOf.md
--rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafRuleRevisionsApi.md
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafRuleRevisionsResponse.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafRuleRevisionsResponseAllOf.md
--rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafRulesApi.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafRulesResponse.md
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafRulesResponseAllOf.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafTag.md
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafTagAttributes.md
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafTagsApi.md
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafTagsResponse.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafTagsResponseAllOf.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WafTagsResponseDataItem.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-2.2.2/docs/WsMessageFormat.md
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/__init__.py
--rw-r--r--   0        0        0    39346 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api_client.py
--rw-r--r--   0        0        0    18987 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/configuration.py
--rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/exceptions.py
--rw-r--r--   0        0        0    82616 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model_utils.py
--rw-r--r--   0        0        0    14634 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/rest.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/__init__.py
--rw-r--r--   0        0        0    30565 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/acl_api.py
--rw-r--r--   0        0        0    37416 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/acl_entry_api.py
--rw-r--r--   0        0        0    24906 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/apex_redirect_api.py
--rw-r--r--   0        0        0    54123 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/backend_api.py
--rw-r--r--   0        0        0    22509 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/billing_address_api.py
--rw-r--r--   0        0        0    18589 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/billing_api.py
--rw-r--r--   0        0        0    34253 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/cache_settings_api.py
--rw-r--r--   0        0        0    34233 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/condition_api.py
--rw-r--r--   0        0        0    36809 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/config_store_api.py
--rw-r--r--   0        0        0    42045 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/config_store_item_api.py
--rw-r--r--   0        0        0    11779 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/contact_api.py
--rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/content_api.py
--rw-r--r--   0        0        0    34431 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/customer_api.py
--rw-r--r--   0        0        0    31732 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/dictionary_api.py
--rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/dictionary_info_api.py
--rw-r--r--   0        0        0    46055 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/dictionary_item_api.py
--rw-r--r--   0        0        0     7987 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/diff_api.py
--rw-r--r--   0        0        0    26863 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/director_api.py
--rw-r--r--   0        0        0    20598 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/director_backend_api.py
--rw-r--r--   0        0        0    42736 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/domain_api.py
--rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/domain_ownerships_api.py
--rw-r--r--   0        0        0    17704 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/enabled_products_api.py
--rw-r--r--   0        0        0    14137 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/events_api.py
--rw-r--r--   0        0        0    32656 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/gzip_api.py
--rw-r--r--   0        0        0    38546 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/header_api.py
--rw-r--r--   0        0        0    37114 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/healthcheck_api.py
--rw-r--r--   0        0        0    60468 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/historical_api.py
--rw-r--r--   0        0        0    19550 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/http3_api.py
--rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/iam_permissions_api.py
--rw-r--r--   0        0        0    21443 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/iam_roles_api.py
--rw-r--r--   0        0        0    22768 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/iam_service_groups_api.py
--rw-r--r--   0        0        0    34358 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/iam_user_groups_api.py
--rw-r--r--   0        0        0    16493 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/invitations_api.py
--rw-r--r--   0        0        0    21168 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/kv_store_api.py
--rw-r--r--   0        0        0    24533 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/kv_store_item_api.py
--rw-r--r--   0        0        0    45445 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_azureblob_api.py
--rw-r--r--   0        0        0    40102 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_bigquery_api.py
--rw-r--r--   0        0        0    45152 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_cloudfiles_api.py
--rw-r--r--   0        0        0    42863 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_datadog_api.py
--rw-r--r--   0        0        0    44606 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_digitalocean_api.py
--rw-r--r--   0        0        0    45229 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_elasticsearch_api.py
--rw-r--r--   0        0        0    44432 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_ftp_api.py
--rw-r--r--   0        0        0    44765 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_gcs_api.py
--rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_heroku_api.py
--rw-r--r--   0        0        0    36624 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_honeycomb_api.py
--rw-r--r--   0        0        0    46115 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_https_api.py
--rw-r--r--   0        0        0    32568 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_kafka_api.py
--rw-r--r--   0        0        0    28280 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_kinesis_api.py
--rw-r--r--   0        0        0    38489 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_logentries_api.py
--rw-r--r--   0        0        0    36081 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_loggly_api.py
--rw-r--r--   0        0        0    36770 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_logshuttle_api.py
--rw-r--r--   0        0        0    38558 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_newrelic_api.py
--rw-r--r--   0        0        0    44042 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_openstack_api.py
--rw-r--r--   0        0        0    36635 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_papertrail_api.py
--rw-r--r--   0        0        0    39265 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_pubsub_api.py
--rw-r--r--   0        0        0    48777 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_s3_api.py
--rw-r--r--   0        0        0    37469 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_scalyr_api.py
--rw-r--r--   0        0        0    45357 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_sftp_api.py
--rw-r--r--   0        0        0    42255 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_splunk_api.py
--rw-r--r--   0        0        0    36567 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_sumologic_api.py
--rw-r--r--   0        0        0    43033 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/logging_syslog_api.py
--rw-r--r--   0        0        0    28852 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/mutual_authentication_api.py
--rw-r--r--   0        0        0    12896 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/package_api.py
--rw-r--r--   0        0        0    47354 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/pool_api.py
--rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/pop_api.py
--rw-r--r--   0        0        0     5863 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/public_ip_list_api.py
--rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/publish_api.py
--rw-r--r--   0        0        0    18435 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/purge_api.py
--rw-r--r--   0        0        0    16945 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/rate_limiter_api.py
--rw-r--r--   0        0        0    17852 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/realtime_api.py
--rw-r--r--   0        0        0    29291 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/request_settings_api.py
--rw-r--r--   0        0        0    30490 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/resource_api.py
--rw-r--r--   0        0        0    18747 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/response_object_api.py
--rw-r--r--   0        0        0    35038 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/server_api.py
--rw-r--r--   0        0        0    44324 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/service_api.py
--rw-r--r--   0        0        0    27911 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/service_authorizations_api.py
--rw-r--r--   0        0        0    13940 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/settings_api.py
--rw-r--r--   0        0        0    38842 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/snippet_api.py
--rw-r--r--   0        0        0    20513 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/star_api.py
--rw-r--r--   0        0        0     7483 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/stats_api.py
--rw-r--r--   0        0        0    29279 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/tls_activations_api.py
--rw-r--r--   0        0        0    28695 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/tls_bulk_certificates_api.py
--rw-r--r--   0        0        0    29585 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/tls_certificates_api.py
--rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/tls_configurations_api.py
--rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/tls_domains_api.py
--rw-r--r--   0        0        0    22120 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/tls_private_keys_api.py
--rw-r--r--   0        0        0    43908 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/tls_subscriptions_api.py
--rw-r--r--   0        0        0    29964 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/tokens_api.py
--rw-r--r--   0        0        0    40392 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/user_api.py
--rw-r--r--   0        0        0    64804 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/vcl_api.py
--rw-r--r--   0        0        0     8068 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/vcl_diff_api.py
--rw-r--r--   0        0        0    51681 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/version_api.py
--rw-r--r--   0        0        0    46003 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/waf_active_rules_api.py
--rw-r--r--   0        0        0    33986 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/waf_exclusions_api.py
--rw-r--r--   0        0        0    36636 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/waf_firewall_versions_api.py
--rw-r--r--   0        0        0    29601 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/waf_firewalls_api.py
--rw-r--r--   0        0        0    13840 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/waf_rule_revisions_api.py
--rw-r--r--   0        0        0    13963 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/waf_rules_api.py
--rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/api/waf_tags_api.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/apis/__init__.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/__init__.py
--rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/acl.py
--rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/acl_entry.py
--rw-r--r--   0        0        0    17351 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/acl_entry_response.py
--rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/acl_entry_response_all_of.py
--rw-r--r--   0        0        0    15915 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/acl_response.py
--rw-r--r--   0        0        0    12025 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/acl_response_all_of.py
--rw-r--r--   0        0        0    16586 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/apex_redirect.py
--rw-r--r--   0        0        0    12580 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/apex_redirect_all_of.py
--rw-r--r--   0        0        0    14660 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/aws_region.py
--rw-r--r--   0        0        0    26143 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/backend.py
--rw-r--r--   0        0        0    30707 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/backend_response.py
--rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/backend_response_all_of.py
--rw-r--r--   0        0        0    14085 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/billing.py
--rw-r--r--   0        0        0    13567 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/billing_address_attributes.py
--rw-r--r--   0        0        0    12075 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/billing_address_request.py
--rw-r--r--   0        0        0    12080 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/billing_address_request_data.py
--rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/billing_address_response.py
--rw-r--r--   0        0        0    12794 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/billing_address_response_data.py
--rw-r--r--   0        0        0    11909 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/billing_address_verification_error_response.py
--rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/billing_address_verification_error_response_errors.py
--rw-r--r--   0        0        0    16877 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/billing_estimate_response.py
--rw-r--r--   0        0        0    11787 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/billing_estimate_response_all_of.py
--rw-r--r--   0        0        0    13188 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/billing_estimate_response_all_of_line.py
--rw-r--r--   0        0        0    11784 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/billing_estimate_response_all_of_lines.py
--rw-r--r--   0        0        0    16765 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/billing_response.py
--rw-r--r--   0        0        0    11716 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/billing_response_all_of.py
--rw-r--r--   0        0        0    18617 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/billing_response_line_item.py
--rw-r--r--   0        0        0    15190 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/billing_response_line_item_all_of.py
--rw-r--r--   0        0        0    12041 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/billing_status.py
--rw-r--r--   0        0        0    16362 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/billing_total.py
--rw-r--r--   0        0        0    12157 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/billing_total_extras.py
--rw-r--r--   0        0        0    11687 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/bulk_update_acl_entries_request.py
--rw-r--r--   0        0        0    15994 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/bulk_update_acl_entry.py
--rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/bulk_update_acl_entry_all_of.py
--rw-r--r--   0        0        0    14518 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/bulk_update_config_store_item.py
--rw-r--r--   0        0        0    11587 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/bulk_update_config_store_item_all_of.py
--rw-r--r--   0        0        0    11742 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/bulk_update_config_store_list_request.py
--rw-r--r--   0        0        0    14509 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/bulk_update_dictionary_item.py
--rw-r--r--   0        0        0    11731 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/bulk_update_dictionary_list_request.py
--rw-r--r--   0        0        0    11735 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/bulk_waf_active_rule.py
--rw-r--r--   0        0        0    11638 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/bulk_waf_active_rules.py
--rw-r--r--   0        0        0    13506 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/cache_setting.py
--rw-r--r--   0        0        0    17524 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/cache_setting_response.py
--rw-r--r--   0        0        0    13530 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/condition.py
--rw-r--r--   0        0        0    16896 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/condition_response.py
--rw-r--r--   0        0        0    11911 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/conditions_response.py
--rw-r--r--   0        0        0    11444 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/config_store.py
--rw-r--r--   0        0        0    11552 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/config_store_info_response.py
--rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/config_store_item.py
--rw-r--r--   0        0        0    15611 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/config_store_item_response.py
--rw-r--r--   0        0        0    11487 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/config_store_item_response_all_of.py
--rw-r--r--   0        0        0    15289 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/config_store_response.py
--rw-r--r--   0        0        0    11519 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/config_store_response_all_of.py
--rw-r--r--   0        0        0    13577 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/contact.py
--rw-r--r--   0        0        0    17300 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/contact_response.py
--rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/contact_response_all_of.py
--rw-r--r--   0        0        0    12747 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/content.py
--rw-r--r--   0        0        0    20398 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/customer.py
--rw-r--r--   0        0        0    24131 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/customer_response.py
--rw-r--r--   0        0        0    11430 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/customer_response_all_of.py
--rw-r--r--   0        0        0    12110 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/dictionary.py
--rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/dictionary_info_response.py
--rw-r--r--   0        0        0    11765 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/dictionary_item.py
--rw-r--r--   0        0        0    15870 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/dictionary_item_response.py
--rw-r--r--   0        0        0    11758 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/dictionary_item_response_all_of.py
--rw-r--r--   0        0        0    16499 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/dictionary_response.py
--rw-r--r--   0        0        0    11436 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/dictionary_response_all_of.py
--rw-r--r--   0        0        0    12481 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/diff_response.py
--rw-r--r--   0        0        0    14620 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/director.py
--rw-r--r--   0        0        0    15768 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/director_backend.py
--rw-r--r--   0        0        0    11747 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/director_backend_all_of.py
--rw-r--r--   0        0        0    18553 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/director_response.py
--rw-r--r--   0        0        0    11783 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/domain.py
--rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/domain_check_item.py
--rw-r--r--   0        0        0    11897 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/domain_check_response.py
--rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/domain_check_response_list.py
--rw-r--r--   0        0        0    15770 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/domain_response.py
--rw-r--r--   0        0        0    11875 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/domains_response.py
--rw-r--r--   0        0        0    12604 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/enabled_product_response.py
--rw-r--r--   0        0        0    11739 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/enabled_product_response_links.py
--rw-r--r--   0        0        0    11694 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/enabled_product_response_product.py
--rw-r--r--   0        0        0    11694 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/enabled_product_response_service.py
--rw-r--r--   0        0        0    12088 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/event.py
--rw-r--r--   0        0        0    21129 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/event_attributes.py
--rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/event_response.py
--rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/events_response.py
--rw-r--r--   0        0        0    11554 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/events_response_all_of.py
--rw-r--r--   0        0        0    11395 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/generic_token_error.py
--rw-r--r--   0        0        0    12758 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/gzip.py
--rw-r--r--   0        0        0    16735 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/gzip_response.py
--rw-r--r--   0        0        0    15905 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/header.py
--rw-r--r--   0        0        0    19828 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/header_response.py
--rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/healthcheck.py
--rw-r--r--   0        0        0    18979 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/healthcheck_response.py
--rw-r--r--   0        0        0    12267 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical.py
--rw-r--r--   0        0        0    14970 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_aggregate_response.py
--rw-r--r--   0        0        0    11672 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_aggregate_response_all_of.py
--rw-r--r--   0        0        0    15047 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_field_aggregate_response.py
--rw-r--r--   0        0        0    11723 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_field_aggregate_response_all_of.py
--rw-r--r--   0        0        0    15024 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_field_response.py
--rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_field_response_data_field.py
--rw-r--r--   0        0        0    12060 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_field_results.py
--rw-r--r--   0        0        0   100364 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_field_results_attributes.py
--rw-r--r--   0        0        0    11905 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_field_results_attributes_all_of.py
--rw-r--r--   0        0        0    11919 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_meta.py
--rw-r--r--   0        0        0    14797 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_regions_response.py
--rw-r--r--   0        0        0    11445 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_regions_response_all_of.py
--rw-r--r--   0        0        0    15219 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_response.py
--rw-r--r--   0        0        0    11959 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_response_data_field.py
--rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_results.py
--rw-r--r--   0        0        0    11620 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_service.py
--rw-r--r--   0        0        0    11367 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_services.py
--rw-r--r--   0        0        0    15037 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_usage_aggregate_response.py
--rw-r--r--   0        0        0    15087 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_usage_month_response.py
--rw-r--r--   0        0        0    11783 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_usage_month_response_all_of.py
--rw-r--r--   0        0        0    12331 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_usage_month_response_data.py
--rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_usage_results.py
--rw-r--r--   0        0        0    15031 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_usage_service_response.py
--rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/historical_usage_service_response_all_of.py
--rw-r--r--   0        0        0    15675 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/http3.py
--rw-r--r--   0        0        0    11705 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/http3_all_of.py
--rw-r--r--   0        0        0    12796 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/http_response_format.py
--rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/http_stream_format.py
--rw-r--r--   0        0        0    13211 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/iam_permission.py
--rw-r--r--   0        0        0    15987 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/iam_role.py
--rw-r--r--   0        0        0    12962 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/iam_role_all_of.py
--rw-r--r--   0        0        0    15636 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/iam_service_group.py
--rw-r--r--   0        0        0    12570 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/iam_service_group_all_of.py
--rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/iam_user_group.py
--rw-r--r--   0        0        0    12926 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/iam_user_group_all_of.py
--rw-r--r--   0        0        0    12044 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/included_with_waf_active_rule.py
--rw-r--r--   0        0        0    15142 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/included_with_waf_active_rule_item.py
--rw-r--r--   0        0        0    12031 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/included_with_waf_exclusion.py
--rw-r--r--   0        0        0    14619 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/included_with_waf_exclusion_item.py
--rw-r--r--   0        0        0    12000 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/included_with_waf_firewall.py
--rw-r--r--   0        0        0    12104 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/included_with_waf_firewall_version.py
--rw-r--r--   0        0        0    13972 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/included_with_waf_firewall_version_item.py
--rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/included_with_waf_rule.py
--rw-r--r--   0        0        0    14599 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/included_with_waf_rule_item.py
--rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/included_with_waf_rule_revision.py
--rw-r--r--   0        0        0    11416 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/inline_object.py
--rw-r--r--   0        0        0    11419 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/inline_object1.py
--rw-r--r--   0        0        0    11418 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/inline_response200.py
--rw-r--r--   0        0        0    11605 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/inline_response2001.py
--rw-r--r--   0        0        0    11985 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/inline_response2002.py
--rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/inline_response2002_meta.py
--rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/inline_response2003.py
--rw-r--r--   0        0        0    11633 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/inline_response2003_meta.py
--rw-r--r--   0        0        0    11585 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/invitation.py
--rw-r--r--   0        0        0    12539 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/invitation_data.py
--rw-r--r--   0        0        0    12611 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/invitation_data_attributes.py
--rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/invitation_response.py
--rw-r--r--   0        0        0    11681 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/invitation_response_all_of.py
--rw-r--r--   0        0        0    14895 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/invitation_response_data.py
--rw-r--r--   0        0        0    12283 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/invitation_response_data_all_of.py
--rw-r--r--   0        0        0    14597 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/invitations_response.py
--rw-r--r--   0        0        0    11690 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/invitations_response_all_of.py
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_address_and_port.py
--rw-r--r--   0        0        0    22489 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_azureblob.py
--rw-r--r--   0        0        0    14206 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_azureblob_all_of.py
--rw-r--r--   0        0        0    24022 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_azureblob_response.py
--rw-r--r--   0        0        0    19390 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_bigquery.py
--rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_bigquery_all_of.py
--rw-r--r--   0        0        0    20943 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_bigquery_response.py
--rw-r--r--   0        0        0    21831 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_cloudfiles.py
--rw-r--r--   0        0        0    13543 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_cloudfiles_all_of.py
--rw-r--r--   0        0        0    23364 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_cloudfiles_response.py
--rw-r--r--   0        0        0    14144 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_common.py
--rw-r--r--   0        0        0    23211 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_datadog.py
--rw-r--r--   0        0        0    18487 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_datadog_all_of.py
--rw-r--r--   0        0        0    24914 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_datadog_response.py
--rw-r--r--   0        0        0    21812 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_digitalocean.py
--rw-r--r--   0        0        0    13514 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_digitalocean_all_of.py
--rw-r--r--   0        0        0    23345 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_digitalocean_response.py
--rw-r--r--   0        0        0    22734 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_elasticsearch.py
--rw-r--r--   0        0        0    14289 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_elasticsearch_all_of.py
--rw-r--r--   0        0        0    24096 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_elasticsearch_response.py
--rw-r--r--   0        0        0    12403 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_format_version.py
--rw-r--r--   0        0        0    22023 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_ftp.py
--rw-r--r--   0        0        0    13770 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_ftp_all_of.py
--rw-r--r--   0        0        0    23556 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_ftp_response.py
--rw-r--r--   0        0        0    22679 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_gcs.py
--rw-r--r--   0        0        0    12744 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_gcs_all_of.py
--rw-r--r--   0        0        0    12815 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_gcs_common.py
--rw-r--r--   0        0        0    24062 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_gcs_response.py
--rw-r--r--   0        0        0    14090 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_generic_common.py
--rw-r--r--   0        0        0    18898 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_google_pubsub.py
--rw-r--r--   0        0        0    12402 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_google_pubsub_all_of.py
--rw-r--r--   0        0        0    20451 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_google_pubsub_response.py
--rw-r--r--   0        0        0    17238 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_heroku.py
--rw-r--r--   0        0        0    11999 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_heroku_all_of.py
--rw-r--r--   0        0        0    18941 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_heroku_response.py
--rw-r--r--   0        0        0    17018 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_honeycomb.py
--rw-r--r--   0        0        0    12284 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_honeycomb_all_of.py
--rw-r--r--   0        0        0    18721 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_honeycomb_response.py
--rw-r--r--   0        0        0    23100 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_https.py
--rw-r--r--   0        0        0    15781 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_https_all_of.py
--rw-r--r--   0        0        0    24462 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_https_response.py
--rw-r--r--   0        0        0    23053 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_kafka.py
--rw-r--r--   0        0        0    15405 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_kafka_all_of.py
--rw-r--r--   0        0        0    24606 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_kafka_response.py
--rw-r--r--   0        0        0    16368 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_kinesis.py
--rw-r--r--   0        0        0    20332 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_kinesis_response.py
--rw-r--r--   0        0        0    18046 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_logentries.py
--rw-r--r--   0        0        0    12851 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_logentries_all_of.py
--rw-r--r--   0        0        0    19749 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_logentries_response.py
--rw-r--r--   0        0        0    16993 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_loggly.py
--rw-r--r--   0        0        0    11754 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_loggly_all_of.py
--rw-r--r--   0        0        0    18696 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_loggly_response.py
--rw-r--r--   0        0        0    17065 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_logshuttle.py
--rw-r--r--   0        0        0    11806 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_logshuttle_all_of.py
--rw-r--r--   0        0        0    18768 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_logshuttle_response.py
--rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_message_type.py
--rw-r--r--   0        0        0    18795 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_newrelic.py
--rw-r--r--   0        0        0    14066 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_newrelic_all_of.py
--rw-r--r--   0        0        0    20498 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_newrelic_response.py
--rw-r--r--   0        0        0    21509 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_openstack.py
--rw-r--r--   0        0        0    13226 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_openstack_all_of.py
--rw-r--r--   0        0        0    23042 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_openstack_response.py
--rw-r--r--   0        0        0    17068 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_papertrail.py
--rw-r--r--   0        0        0    18776 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_papertrail_response.py
--rw-r--r--   0        0        0    12818 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_placement.py
--rw-r--r--   0        0        0    12265 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_request_caps_common.py
--rw-r--r--   0        0        0    24622 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_s3.py
--rw-r--r--   0        0        0    16374 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_s3_all_of.py
--rw-r--r--   0        0        0    26155 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_s3_response.py
--rw-r--r--   0        0        0    17727 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_scalyr.py
--rw-r--r--   0        0        0    12488 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_scalyr_all_of.py
--rw-r--r--   0        0        0    19430 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_scalyr_response.py
--rw-r--r--   0        0        0    22808 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_sftp.py
--rw-r--r--   0        0        0    14123 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_sftp_all_of.py
--rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_sftp_response.py
--rw-r--r--   0        0        0    21030 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_splunk.py
--rw-r--r--   0        0        0    12164 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_splunk_all_of.py
--rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_splunk_response.py
--rw-r--r--   0        0        0    17102 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_sumologic.py
--rw-r--r--   0        0        0    11912 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_sumologic_all_of.py
--rw-r--r--   0        0        0    18805 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_sumologic_response.py
--rw-r--r--   0        0        0    21452 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_syslog.py
--rw-r--r--   0        0        0    13046 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_syslog_all_of.py
--rw-r--r--   0        0        0    22829 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_syslog_response.py
--rw-r--r--   0        0        0    13547 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_tls_common.py
--rw-r--r--   0        0        0    11595 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/logging_use_tls.py
--rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/mutual_authentication.py
--rw-r--r--   0        0        0    12711 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/mutual_authentication_data.py
--rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/mutual_authentication_data_attributes.py
--rw-r--r--   0        0        0    11767 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/mutual_authentication_response.py
--rw-r--r--   0        0        0    15149 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/mutual_authentication_response_attributes.py
--rw-r--r--   0        0        0    11647 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/mutual_authentication_response_attributes_all_of.py
--rw-r--r--   0        0        0    15368 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/mutual_authentication_response_data.py
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/mutual_authentication_response_data_all_of.py
--rw-r--r--   0        0        0    14749 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/mutual_authentications_response.py
--rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/mutual_authentications_response_all_of.py
--rw-r--r--   0        0        0    11906 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/number_version.py
--rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/package.py
--rw-r--r--   0        0        0    13175 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/package_metadata.py
--rw-r--r--   0        0        0    15990 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/package_response.py
--rw-r--r--   0        0        0    11519 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/package_response_all_of.py
--rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/pagination.py
--rw-r--r--   0        0        0    12267 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/pagination_links.py
--rw-r--r--   0        0        0    12484 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/pagination_meta.py
--rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/permission.py
--rw-r--r--   0        0        0    23511 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/pool.py
--rw-r--r--   0        0        0    18578 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/pool_all_of.py
--rw-r--r--   0        0        0    25586 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/pool_response.py
--rw-r--r--   0        0        0    11418 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/pool_response_all_of.py
--rw-r--r--   0        0        0    15216 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/pop.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/pop_coordinates.py
--rw-r--r--   0        0        0    11742 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/public_ip_list.py
--rw-r--r--   0        0        0    12528 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/publish_item.py
--rw-r--r--   0        0        0    12411 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/publish_item_formats.py
--rw-r--r--   0        0        0    11685 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/publish_request.py
--rw-r--r--   0        0        0    11432 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/purge_keys.py
--rw-r--r--   0        0        0    11165 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/purge_keys_response.py
--rw-r--r--   0        0        0    11594 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/purge_response.py
--rw-r--r--   0        0        0    19002 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/rate_limiter.py
--rw-r--r--   0        0        0    23413 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/rate_limiter_response.py
--rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/rate_limiter_response1.py
--rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/rate_limiter_response_all_of.py
--rw-r--r--   0        0        0    12619 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/realtime.py
--rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/realtime_entry.py
--rw-r--r--   0        0        0    98045 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/realtime_measurements.py
--rw-r--r--   0        0        0    11749 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_common_name.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_customer.py
--rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_customer_customer.py
--rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_member_customer.py
--rw-r--r--   0        0        0    11936 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_member_mutual_authentication.py
--rw-r--r--   0        0        0    11805 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_member_service.py
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_member_service_invitation.py
--rw-r--r--   0        0        0    11866 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_member_tls_activation.py
--rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_member_tls_bulk_certificate.py
--rw-r--r--   0        0        0    11876 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_member_tls_certificate.py
--rw-r--r--   0        0        0    11896 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_member_tls_configuration.py
--rw-r--r--   0        0        0    11857 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_member_tls_dns_record.py
--rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_member_tls_domain.py
--rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_member_tls_private_key.py
--rw-r--r--   0        0        0    11886 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_member_tls_subscription.py
--rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_member_waf_active_rule.py
--rw-r--r--   0        0        0    11846 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_member_waf_firewall.py
--rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_member_waf_firewall_version.py
--rw-r--r--   0        0        0    11806 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_member_waf_rule.py
--rw-r--r--   0        0        0    11995 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_member_waf_rule_revision.py
--rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_member_waf_tag.py
--rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_mutual_authentication.py
--rw-r--r--   0        0        0    11881 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_mutual_authentication_mutual_authentication.py
--rw-r--r--   0        0        0    12027 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_mutual_authentications.py
--rw-r--r--   0        0        0    11893 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_mutual_authentications_mutual_authentications.py
--rw-r--r--   0        0        0    11705 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_service.py
--rw-r--r--   0        0        0    11961 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_service_invitations.py
--rw-r--r--   0        0        0    12022 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_service_invitations_create.py
--rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_service_invitations_create_service_invitations.py
--rw-r--r--   0        0        0    11854 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_service_invitations_service_invitations.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_services.py
--rw-r--r--   0        0        0    11723 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_services_services.py
--rw-r--r--   0        0        0    11851 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_activation.py
--rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_activation_tls_activation.py
--rw-r--r--   0        0        0    11859 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_activations.py
--rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_bulk_certificate.py
--rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_bulk_certificate_tls_bulk_certificate.py
--rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_bulk_certificates.py
--rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_certificate.py
--rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_certificate_tls_certificate.py
--rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_certificates.py
--rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_certificates_tls_certificates.py
--rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_configuration.py
--rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_configuration_for_tls_subscription.py
--rw-r--r--   0        0        0    11829 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_configuration_tls_configuration.py
--rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_configurations.py
--rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_configurations_tls_configurations.py
--rw-r--r--   0        0        0    11794 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_dns_record.py
--rw-r--r--   0        0        0    11775 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_dns_record_dns_record.py
--rw-r--r--   0        0        0    11802 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_dns_records.py
--rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_domain.py
--rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_domain_tls_domain.py
--rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_domains.py
--rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_domains_tls_domains.py
--rw-r--r--   0        0        0    11858 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_private_key.py
--rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_private_key_tls_private_key.py
--rw-r--r--   0        0        0    11880 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_private_keys.py
--rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_private_keys_tls_private_keys.py
--rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_subscription.py
--rw-r--r--   0        0        0    11822 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_subscription_tls_subscription.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_tls_subscriptions.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_user.py
--rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_user_user.py
--rw-r--r--   0        0        0    11880 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_waf_active_rules.py
--rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_waf_active_rules_waf_active_rules.py
--rw-r--r--   0        0        0    11807 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_waf_firewall.py
--rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_waf_firewall_version.py
--rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_waf_firewall_version_waf_firewall_version.py
--rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_waf_firewall_versions.py
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_waf_firewall_waf_firewall.py
--rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_waf_rule.py
--rw-r--r--   0        0        0    11914 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_waf_rule_revision.py
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_waf_rule_revision_waf_rule_revisions.py
--rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_waf_rule_revisions.py
--rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_waf_rule_waf_rule.py
--rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_waf_rules.py
--rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_waf_tags.py
--rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationship_waf_tags_waf_tags.py
--rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationships_for_invitation.py
--rw-r--r--   0        0        0    14050 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationships_for_mutual_authentication.py
--rw-r--r--   0        0        0    14345 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationships_for_star.py
--rw-r--r--   0        0        0    15491 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationships_for_tls_activation.py
--rw-r--r--   0        0        0    14690 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationships_for_tls_bulk_certificate.py
--rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationships_for_tls_configuration.py
--rw-r--r--   0        0        0    14687 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationships_for_tls_domain.py
--rw-r--r--   0        0        0    14589 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationships_for_tls_private_key.py
--rw-r--r--   0        0        0    16266 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationships_for_tls_subscription.py
--rw-r--r--   0        0        0    14951 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationships_for_waf_active_rule.py
--rw-r--r--   0        0        0    14691 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationships_for_waf_exclusion.py
--rw-r--r--   0        0        0    14940 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationships_for_waf_firewall_version.py
--rw-r--r--   0        0        0    14666 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/relationships_for_waf_rule.py
--rw-r--r--   0        0        0    15858 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/request_settings.py
--rw-r--r--   0        0        0    19891 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/request_settings_response.py
--rw-r--r--   0        0        0    11736 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/resource.py
--rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/resource_response.py
--rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/resource_response_all_of.py
--rw-r--r--   0        0        0    13673 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/response_object.py
--rw-r--r--   0        0        0    17701 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/response_object_response.py
--rw-r--r--   0        0        0    97280 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/results.py
--rw-r--r--   0        0        0    12451 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/role_user.py
--rw-r--r--   0        0        0    17321 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/schemas_contact_response.py
--rw-r--r--   0        0        0    17519 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/schemas_snippet_response.py
--rw-r--r--   0        0        0    18068 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/schemas_user_response.py
--rw-r--r--   0        0        0    15953 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/schemas_vcl_response.py
--rw-r--r--   0        0        0    13626 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/schemas_version.py
--rw-r--r--   0        0        0    17433 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/schemas_version_response.py
--rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/schemas_waf_firewall_version.py
--rw-r--r--   0        0        0    12179 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/schemas_waf_firewall_version_data.py
--rw-r--r--   0        0        0    14569 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/server.py
--rw-r--r--   0        0        0    18752 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/server_response.py
--rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/server_response_all_of.py
--rw-r--r--   0        0        0    12015 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service.py
--rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_authorization.py
--rw-r--r--   0        0        0    12718 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_authorization_data.py
--rw-r--r--   0        0        0    11658 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_authorization_data_attributes.py
--rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_authorization_data_relationships.py
--rw-r--r--   0        0        0    11899 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_authorization_data_relationships_user.py
--rw-r--r--   0        0        0    11844 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_authorization_data_relationships_user_data.py
--rw-r--r--   0        0        0    11767 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_authorization_response.py
--rw-r--r--   0        0        0    15176 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_authorization_response_data.py
--rw-r--r--   0        0        0    11863 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_authorization_response_data_all_of.py
--rw-r--r--   0        0        0    14749 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_authorizations_response.py
--rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_authorizations_response_all_of.py
--rw-r--r--   0        0        0    14640 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_create.py
--rw-r--r--   0        0        0    11543 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_create_all_of.py
--rw-r--r--   0        0        0    18255 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_detail.py
--rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_detail_all_of.py
--rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_id_and_version.py
--rw-r--r--   0        0        0    11656 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_invitation.py
--rw-r--r--   0        0        0    12646 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_invitation_data.py
--rw-r--r--   0        0        0    11922 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_invitation_data_attributes.py
--rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_invitation_data_relationships.py
--rw-r--r--   0        0        0    14111 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_invitation_response.py
--rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_invitation_response_all_of.py
--rw-r--r--   0        0        0    11854 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_invitation_response_all_of_data.py
--rw-r--r--   0        0        0    17024 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_list_response.py
--rw-r--r--   0        0        0    12407 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_list_response_all_of.py
--rw-r--r--   0        0        0    17544 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_response.py
--rw-r--r--   0        0        0    12948 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_response_all_of.py
--rw-r--r--   0        0        0    23835 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_version_detail.py
--rw-r--r--   0        0        0    23852 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/service_version_detail_or_null.py
--rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/settings.py
--rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/settings_response.py
--rw-r--r--   0        0        0    13165 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/snippet.py
--rw-r--r--   0        0        0    17498 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/snippet_response.py
--rw-r--r--   0        0        0    12037 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/snippet_response_all_of.py
--rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/star.py
--rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/star_data.py
--rw-r--r--   0        0        0    13825 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/star_response.py
--rw-r--r--   0        0        0    11571 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/star_response_all_of.py
--rw-r--r--   0        0        0    11555 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/stats.py
--rw-r--r--   0        0        0    11440 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/store.py
--rw-r--r--   0        0        0    11668 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/store_response.py
--rw-r--r--   0        0        0    12287 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/timestamps.py
--rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/timestamps_no_delete.py
--rw-r--r--   0        0        0    11616 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_activation.py
--rw-r--r--   0        0        0    12100 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_activation_data.py
--rw-r--r--   0        0        0    11697 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_activation_response.py
--rw-r--r--   0        0        0    14980 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_activation_response_data.py
--rw-r--r--   0        0        0    11842 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_activation_response_data_all_of.py
--rw-r--r--   0        0        0    14644 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_activations_response.py
--rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_activations_response_all_of.py
--rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_bulk_certificate.py
--rw-r--r--   0        0        0    12666 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_bulk_certificate_data.py
--rw-r--r--   0        0        0    12407 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_bulk_certificate_data_attributes.py
--rw-r--r--   0        0        0    11748 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_bulk_certificate_response.py
--rw-r--r--   0        0        0    16192 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_bulk_certificate_response_attributes.py
--rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_bulk_certificate_response_attributes_all_of.py
--rw-r--r--   0        0        0    15305 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_bulk_certificate_response_data.py
--rw-r--r--   0        0        0    12043 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_bulk_certificate_response_data_all_of.py
--rw-r--r--   0        0        0    14721 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_bulk_certificates_response.py
--rw-r--r--   0        0        0    11772 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_bulk_certificates_response_all_of.py
--rw-r--r--   0        0        0    11626 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_certificate.py
--rw-r--r--   0        0        0    12510 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_certificate_data.py
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_certificate_data_attributes.py
--rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_certificate_response.py
--rw-r--r--   0        0        0    17609 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_certificate_response_attributes.py
--rw-r--r--   0        0        0    14137 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_certificate_response_attributes_all_of.py
--rw-r--r--   0        0        0    15107 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_certificate_response_data.py
--rw-r--r--   0        0        0    12002 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_certificate_response_data_all_of.py
--rw-r--r--   0        0        0    14659 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_certificates_response.py
--rw-r--r--   0        0        0    11731 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_certificates_response_all_of.py
--rw-r--r--   0        0        0    13892 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_common.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_configuration.py
--rw-r--r--   0        0        0    12615 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_configuration_data.py
--rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_configuration_data_attributes.py
--rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_configuration_response.py
--rw-r--r--   0        0        0    16408 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_configuration_response_attributes.py
--rw-r--r--   0        0        0    12926 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_configuration_response_attributes_all_of.py
--rw-r--r--   0        0        0    15232 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_configuration_response_data.py
--rw-r--r--   0        0        0    12022 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_configuration_response_data_all_of.py
--rw-r--r--   0        0        0    14689 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_configurations_response.py
--rw-r--r--   0        0        0    11751 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_configurations_response_all_of.py
--rw-r--r--   0        0        0    13196 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_dns_record.py
--rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_domain_data.py
--rw-r--r--   0        0        0    14527 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_domains_response.py
--rw-r--r--   0        0        0    11624 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_domains_response_all_of.py
--rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_private_key.py
--rw-r--r--   0        0        0    12546 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_private_key_data.py
--rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_private_key_data_attributes.py
--rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_private_key_response.py
--rw-r--r--   0        0        0    16480 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_private_key_response_attributes.py
--rw-r--r--   0        0        0    13012 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_private_key_response_attributes_all_of.py
--rw-r--r--   0        0        0    12321 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_private_key_response_data.py
--rw-r--r--   0        0        0    14646 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_private_keys_response.py
--rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_private_keys_response_all_of.py
--rw-r--r--   0        0        0    11636 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_subscription.py
--rw-r--r--   0        0        0    12591 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_subscription_data.py
--rw-r--r--   0        0        0    11818 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_subscription_data_attributes.py
--rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_subscription_response.py
--rw-r--r--   0        0        0    15234 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_subscription_response_attributes.py
--rw-r--r--   0        0        0    11757 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_subscription_response_attributes_all_of.py
--rw-r--r--   0        0        0    14191 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_subscription_response_data.py
--rw-r--r--   0        0        0    12012 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_subscription_response_data_all_of.py
--rw-r--r--   0        0        0    14645 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_subscriptions_response.py
--rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/tls_subscriptions_response_all_of.py
--rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/token.py
--rw-r--r--   0        0        0    18055 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/token_created_response.py
--rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/token_created_response_all_of.py
--rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/token_response.py
--rw-r--r--   0        0        0    13237 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/token_response_all_of.py
--rw-r--r--   0        0        0    11733 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_billing_address.py
--rw-r--r--   0        0        0    11616 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_contact.py
--rw-r--r--   0        0        0    11631 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_customer.py
--rw-r--r--   0        0        0    11586 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_event.py
--rw-r--r--   0        0        0    11661 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_invitation.py
--rw-r--r--   0        0        0    11823 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_mutual_authentication.py
--rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_resource.py
--rw-r--r--   0        0        0    11616 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_service.py
--rw-r--r--   0        0        0    11823 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_service_authorization.py
--rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_service_invitation.py
--rw-r--r--   0        0        0    11571 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_star.py
--rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_tls_activation.py
--rw-r--r--   0        0        0    11805 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_tls_bulk_certificate.py
--rw-r--r--   0        0        0    11733 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_tls_certificate.py
--rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_tls_configuration.py
--rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_tls_dns_record.py
--rw-r--r--   0        0        0    11658 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_tls_domain.py
--rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_tls_private_key.py
--rw-r--r--   0        0        0    11748 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_tls_subscription.py
--rw-r--r--   0        0        0    11571 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_user.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_waf_active_rule.py
--rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_waf_exclusion.py
--rw-r--r--   0        0        0    11692 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_waf_firewall.py
--rw-r--r--   0        0        0    11809 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_waf_firewall_version.py
--rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_waf_rule.py
--rw-r--r--   0        0        0    11764 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_waf_rule_revision.py
--rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/type_waf_tag.py
--rw-r--r--   0        0        0    12136 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/update_billing_address_request.py
--rw-r--r--   0        0        0    12402 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/update_billing_address_request_data.py
--rw-r--r--   0        0        0    13820 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/user.py
--rw-r--r--   0        0        0    18047 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/user_response.py
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/user_response_all_of.py
--rw-r--r--   0        0        0    12570 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/validator_result.py
--rw-r--r--   0        0        0    12325 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/validator_result_messages.py
--rw-r--r--   0        0        0    11960 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/vcl.py
--rw-r--r--   0        0        0    12644 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/vcl_diff.py
--rw-r--r--   0        0        0    15932 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/vcl_response.py
--rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/version.py
--rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/version_create_response.py
--rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/version_detail.py
--rw-r--r--   0        0        0    12978 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/version_detail_settings.py
--rw-r--r--   0        0        0    17376 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/version_response.py
--rw-r--r--   0        0        0    11475 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/version_response_all_of.py
--rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_active_rule.py
--rw-r--r--   0        0        0    15118 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_active_rule_creation_response.py
--rw-r--r--   0        0        0    12546 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_active_rule_data.py
--rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_active_rule_data_attributes.py
--rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_active_rule_response.py
--rw-r--r--   0        0        0    15228 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_active_rule_response_data.py
--rw-r--r--   0        0        0    12559 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_active_rule_response_data_all_of.py
--rw-r--r--   0        0        0    15589 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_active_rule_response_data_attributes.py
--rw-r--r--   0        0        0    12100 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_active_rule_response_data_attributes_all_of.py
--rw-r--r--   0        0        0    14978 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_active_rule_response_data_relationships.py
--rw-r--r--   0        0        0    15066 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_active_rules_response.py
--rw-r--r--   0        0        0    12142 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_active_rules_response_all_of.py
--rw-r--r--   0        0        0    11606 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_exclusion.py
--rw-r--r--   0        0        0    12519 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_exclusion_data.py
--rw-r--r--   0        0        0    13837 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_exclusion_data_attributes.py
--rw-r--r--   0        0        0    11687 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_exclusion_response.py
--rw-r--r--   0        0        0    15289 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_exclusion_response_data.py
--rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_exclusion_response_data_all_of.py
--rw-r--r--   0        0        0    17359 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_exclusion_response_data_attributes.py
--rw-r--r--   0        0        0    13876 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_exclusion_response_data_attributes_all_of.py
--rw-r--r--   0        0        0    14718 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_exclusion_response_data_relationships.py
--rw-r--r--   0        0        0    15041 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_exclusions_response.py
--rw-r--r--   0        0        0    12123 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_exclusions_response_all_of.py
--rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_firewall.py
--rw-r--r--   0        0        0    12037 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_firewall_data.py
--rw-r--r--   0        0        0    12561 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_firewall_data_attributes.py
--rw-r--r--   0        0        0    12082 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_firewall_response.py
--rw-r--r--   0        0        0    15119 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_firewall_response_data.py
--rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_firewall_response_data_all_of.py
--rw-r--r--   0        0        0    19383 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_firewall_response_data_attributes.py
--rw-r--r--   0        0        0    15905 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_firewall_response_data_attributes_all_of.py
--rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_firewall_version.py
--rw-r--r--   0        0        0    12158 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_firewall_version_data.py
--rw-r--r--   0        0        0    24857 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_firewall_version_data_attributes.py
--rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_firewall_version_response.py
--rw-r--r--   0        0        0    15440 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_firewall_version_response_data.py
--rw-r--r--   0        0        0    12686 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_firewall_version_response_data_all_of.py
--rw-r--r--   0        0        0    20346 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_firewall_version_response_data_attributes.py
--rw-r--r--   0        0        0    16832 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_firewall_version_response_data_attributes_all_of.py
--rw-r--r--   0        0        0    15176 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_firewall_versions_response.py
--rw-r--r--   0        0        0    12227 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_firewall_versions_response_all_of.py
--rw-r--r--   0        0        0    15019 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_firewalls_response.py
--rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_firewalls_response_all_of.py
--rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_rule.py
--rw-r--r--   0        0        0    12553 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_rule_attributes.py
--rw-r--r--   0        0        0    12014 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_rule_response.py
--rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_rule_response_data.py
--rw-r--r--   0        0        0    11737 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_rule_response_data_all_of.py
--rw-r--r--   0        0        0    12370 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_rule_revision.py
--rw-r--r--   0        0        0    13775 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_rule_revision_attributes.py
--rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_rule_revision_or_latest.py
--rw-r--r--   0        0        0    12152 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_rule_revision_response.py
--rw-r--r--   0        0        0    15147 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_rule_revision_response_data.py
--rw-r--r--   0        0        0    11732 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_rule_revision_response_data_all_of.py
--rw-r--r--   0        0        0    15110 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_rule_revisions_response.py
--rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_rule_revisions_response_all_of.py
--rw-r--r--   0        0        0    14931 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_rules_response.py
--rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_rules_response_all_of.py
--rw-r--r--   0        0        0    12195 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_tag.py
--rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_tag_attributes.py
--rw-r--r--   0        0        0    14872 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_tags_response.py
--rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_tags_response_all_of.py
--rw-r--r--   0        0        0    14941 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/waf_tags_response_data_item.py
--rw-r--r--   0        0        0    11832 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/model/ws_message_format.py
--rw-r--r--   0        0        0    45122 2020-02-02 00:00:00.000000 fastly-2.2.2/fastly/models/__init__.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 fastly-2.2.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 fastly-2.2.2/LICENSE
--rw-r--r--   0        0        0    89067 2020-02-02 00:00:00.000000 fastly-2.2.2/README.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastly-2.2.2/pyproject.toml
--rw-r--r--   0        0        0    89559 2020-02-02 00:00:00.000000 fastly-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 fastly-2.3.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 fastly-2.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 fastly-2.3.0/MANIFEST.in
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 fastly-2.3.0/SECURITY.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fastly-2.3.0/requirements.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fastly-2.3.0/setup.cfg
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 fastly-2.3.0/setup.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastly-2.3.0/sig.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 fastly-2.3.0/test-requirements.txt
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 fastly-2.3.0/tox.ini
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 fastly-2.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rwxr-xr-x   0        0        0      619 2020-02-02 00:00:00.000000 fastly-2.3.0/.github/scripts/pack.sh
+-rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 fastly-2.3.0/.github/scripts/prepare.sh
+-rwxr-xr-x   0        0        0      812 2020-02-02 00:00:00.000000 fastly-2.3.0/.github/scripts/publish_env.sh
+-rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 fastly-2.3.0/.github/scripts/release_body.sh
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 fastly-2.3.0/.github/workflows/ci-release.yaml
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Acl.md
+-rw-r--r--   0        0        0    15695 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/AclApi.md
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/AclEntry.md
+-rw-r--r--   0        0        0    20447 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/AclEntryApi.md
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/AclEntryResponse.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/AclEntryResponseAllOf.md
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/AclResponse.md
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/AclResponseAllOf.md
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ApexRedirect.md
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ApexRedirectAllOf.md
+-rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ApexRedirectApi.md
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/AwsRegion.md
+-rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Backend.md
+-rw-r--r--   0        0        0    38268 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BackendApi.md
+-rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BackendResponse.md
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BackendResponseAllOf.md
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Billing.md
+-rw-r--r--   0        0        0    13259 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BillingAddressApi.md
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BillingAddressAttributes.md
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BillingAddressRequest.md
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BillingAddressRequestData.md
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BillingAddressResponse.md
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BillingAddressResponseData.md
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BillingAddressVerificationErrorResponse.md
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BillingAddressVerificationErrorResponseErrors.md
+-rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BillingApi.md
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BillingEstimateResponse.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BillingEstimateResponseAllOf.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BillingEstimateResponseAllOfLine.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BillingEstimateResponseAllOfLines.md
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BillingResponse.md
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BillingResponseAllOf.md
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BillingResponseLineItem.md
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BillingResponseLineItemAllOf.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BillingStatus.md
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BillingTotal.md
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BillingTotalExtras.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BulkUpdateAclEntriesRequest.md
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BulkUpdateAclEntry.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BulkUpdateAclEntryAllOf.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BulkUpdateConfigStoreItem.md
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BulkUpdateConfigStoreItemAllOf.md
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BulkUpdateConfigStoreListRequest.md
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BulkUpdateDictionaryItem.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BulkUpdateDictionaryListRequest.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BulkWafActiveRule.md
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/BulkWafActiveRules.md
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/CacheSetting.md
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/CacheSettingResponse.md
+-rw-r--r--   0        0        0    18846 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/CacheSettingsApi.md
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Condition.md
+-rw-r--r--   0        0        0    17741 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ConditionApi.md
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ConditionResponse.md
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ConditionsResponse.md
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ConfigStore.md
+-rw-r--r--   0        0        0    18464 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ConfigStoreApi.md
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ConfigStoreInfoResponse.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ConfigStoreItem.md
+-rw-r--r--   0        0        0    23504 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ConfigStoreItemApi.md
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ConfigStoreItemResponse.md
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ConfigStoreItemResponseAllOf.md
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ConfigStoreResponse.md
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ConfigStoreResponseAllOf.md
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Contact.md
+-rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ContactApi.md
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ContactResponse.md
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ContactResponseAllOf.md
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Content.md
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ContentApi.md
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Customer.md
+-rw-r--r--   0        0        0    18926 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/CustomerApi.md
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/CustomerResponse.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/CustomerResponseAllOf.md
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Dictionary.md
+-rw-r--r--   0        0        0    17237 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DictionaryApi.md
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DictionaryInfoApi.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DictionaryInfoResponse.md
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DictionaryItem.md
+-rw-r--r--   0        0        0    26138 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DictionaryItemApi.md
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DictionaryItemResponse.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DictionaryItemResponseAllOf.md
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DictionaryResponse.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DictionaryResponseAllOf.md
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DiffApi.md
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DiffResponse.md
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Director.md
+-rw-r--r--   0        0        0    15015 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DirectorApi.md
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DirectorBackend.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DirectorBackendAllOf.md
+-rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DirectorBackendApi.md
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DirectorResponse.md
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Domain.md
+-rw-r--r--   0        0        0    21769 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DomainApi.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DomainCheckItem.md
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DomainCheckResponse.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DomainCheckResponseList.md
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DomainOwnershipsApi.md
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DomainResponse.md
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/DomainsResponse.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/EnabledProductResponse.md
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/EnabledProductResponseLinks.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/EnabledProductResponseProduct.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/EnabledProductResponseService.md
+-rw-r--r--   0        0        0     8351 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/EnabledProductsApi.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Event.md
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/EventAttributes.md
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/EventResponse.md
+-rw-r--r--   0        0        0     7243 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/EventsApi.md
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/EventsResponse.md
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/EventsResponseAllOf.md
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/GenericTokenError.md
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Gzip.md
+-rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/GzipApi.md
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/GzipResponse.md
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Header.md
+-rw-r--r--   0        0        0    20925 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HeaderApi.md
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HeaderResponse.md
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Healthcheck.md
+-rw-r--r--   0        0        0    20120 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HealthcheckApi.md
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HealthcheckResponse.md
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Historical.md
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalAggregateResponse.md
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalAggregateResponseAllOf.md
+-rw-r--r--   0        0        0    39081 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalApi.md
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalFieldAggregateResponse.md
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalFieldAggregateResponseAllOf.md
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalFieldResponse.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalFieldResponseDataField.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalFieldResults.md
+-rw-r--r--   0        0        0    27230 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalFieldResultsAttributes.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalFieldResultsAttributesAllOf.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalMeta.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalRegionsResponse.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalRegionsResponseAllOf.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalResponse.md
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalResponseDataField.md
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalResults.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalService.md
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalServices.md
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalUsageAggregateResponse.md
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalUsageMonthResponse.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalUsageMonthResponseAllOf.md
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalUsageMonthResponseData.md
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalUsageResults.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalUsageServiceResponse.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HistoricalUsageServiceResponseAllOf.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Http3.md
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Http3AllOf.md
+-rw-r--r--   0        0        0     9629 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Http3Api.md
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HttpResponseFormat.md
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/HttpStreamFormat.md
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/IamPermission.md
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/IamPermissionsApi.md
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/IamRole.md
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/IamRoleAllOf.md
+-rw-r--r--   0        0        0     9918 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/IamRolesApi.md
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/IamServiceGroup.md
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/IamServiceGroupAllOf.md
+-rw-r--r--   0        0        0    11406 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/IamServiceGroupsApi.md
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/IamUserGroup.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/IamUserGroupAllOf.md
+-rw-r--r--   0        0        0    17911 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/IamUserGroupsApi.md
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/IncludedWithWafActiveRule.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/IncludedWithWafActiveRuleItem.md
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/IncludedWithWafExclusion.md
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/IncludedWithWafExclusionItem.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/IncludedWithWafFirewall.md
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/IncludedWithWafFirewallVersion.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/IncludedWithWafFirewallVersionItem.md
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/IncludedWithWafRule.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/IncludedWithWafRuleItem.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/IncludedWithWafRuleRevision.md
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/InlineObject.md
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/InlineObject1.md
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/InlineResponse200.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/InlineResponse2001.md
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/InlineResponse2002.md
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/InlineResponse2002Meta.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/InlineResponse2003.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/InlineResponse2003Meta.md
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Invitation.md
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/InvitationData.md
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/InvitationDataAttributes.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/InvitationResponse.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/InvitationResponseAllOf.md
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/InvitationResponseData.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/InvitationResponseDataAllOf.md
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/InvitationsApi.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/InvitationsResponse.md
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/InvitationsResponseAllOf.md
+-rw-r--r--   0        0        0     9883 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/KvStoreApi.md
+-rw-r--r--   0        0        0    12230 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/KvStoreItemApi.md
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingAddressAndPort.md
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingAzureblob.md
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingAzureblobAllOf.md
+-rw-r--r--   0        0        0    29125 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingAzureblobApi.md
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingAzureblobResponse.md
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingBigquery.md
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingBigqueryAllOf.md
+-rw-r--r--   0        0        0    24678 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingBigqueryApi.md
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingBigqueryResponse.md
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingCloudfiles.md
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingCloudfilesAllOf.md
+-rw-r--r--   0        0        0    27524 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingCloudfilesApi.md
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingCloudfilesResponse.md
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingCommon.md
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingDatadog.md
+-rw-r--r--   0        0        0     3883 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingDatadogAllOf.md
+-rw-r--r--   0        0        0    38955 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingDatadogApi.md
+-rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingDatadogResponse.md
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingDigitalocean.md
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingDigitaloceanAllOf.md
+-rw-r--r--   0        0        0    28174 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingDigitaloceanApi.md
+-rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingDigitaloceanResponse.md
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingElasticsearch.md
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingElasticsearchAllOf.md
+-rw-r--r--   0        0        0    30259 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingElasticsearchApi.md
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingElasticsearchResponse.md
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingFormatVersion.md
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingFtp.md
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingFtpAllOf.md
+-rw-r--r--   0        0        0    27244 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingFtpApi.md
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingFtpResponse.md
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingGcs.md
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingGcsAllOf.md
+-rw-r--r--   0        0        0    28487 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingGcsApi.md
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingGcsCommon.md
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingGcsResponse.md
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingGenericCommon.md
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingGooglePubsub.md
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingGooglePubsubAllOf.md
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingGooglePubsubResponse.md
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingHeroku.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingHerokuAllOf.md
+-rw-r--r--   0        0        0    21127 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingHerokuApi.md
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingHerokuResponse.md
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingHoneycomb.md
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingHoneycombAllOf.md
+-rw-r--r--   0        0        0    20986 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingHoneycombApi.md
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingHoneycombResponse.md
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingHttps.md
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingHttpsAllOf.md
+-rw-r--r--   0        0        0    29036 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingHttpsApi.md
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingHttpsResponse.md
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingKafka.md
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingKafkaAllOf.md
+-rw-r--r--   0        0        0    18733 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingKafkaApi.md
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingKafkaResponse.md
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingKinesis.md
+-rw-r--r--   0        0        0    17289 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingKinesisApi.md
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingKinesisResponse.md
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingLogentries.md
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingLogentriesAllOf.md
+-rw-r--r--   0        0        0    22258 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingLogentriesApi.md
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingLogentriesResponse.md
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingLoggly.md
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingLogglyAllOf.md
+-rw-r--r--   0        0        0    20871 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingLogglyApi.md
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingLogglyResponse.md
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingLogshuttle.md
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingLogshuttleAllOf.md
+-rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingLogshuttleApi.md
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingLogshuttleResponse.md
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingMessageType.md
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingNewrelic.md
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingNewrelicAllOf.md
+-rw-r--r--   0        0        0    25794 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingNewrelicApi.md
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingNewrelicResponse.md
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingOpenstack.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingOpenstackAllOf.md
+-rw-r--r--   0        0        0    27216 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingOpenstackApi.md
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingOpenstackResponse.md
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingPapertrail.md
+-rw-r--r--   0        0        0    21189 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingPapertrailApi.md
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingPapertrailResponse.md
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingPlacement.md
+-rw-r--r--   0        0        0    24358 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingPubsubApi.md
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingRequestCapsCommon.md
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingS3.md
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingS3AllOf.md
+-rw-r--r--   0        0        0    31697 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingS3Api.md
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingS3Response.md
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingScalyr.md
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingScalyrAllOf.md
+-rw-r--r--   0        0        0    21715 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingScalyrApi.md
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingScalyrResponse.md
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingSftp.md
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingSftpAllOf.md
+-rw-r--r--   0        0        0    28475 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingSftpApi.md
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingSftpResponse.md
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingSplunk.md
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingSplunkAllOf.md
+-rw-r--r--   0        0        0    26444 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingSplunkApi.md
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingSplunkResponse.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingSumologic.md
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingSumologicAllOf.md
+-rw-r--r--   0        0        0    21088 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingSumologicApi.md
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingSumologicResponse.md
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingSyslog.md
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingSyslogAllOf.md
+-rw-r--r--   0        0        0    26805 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingSyslogApi.md
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingSyslogResponse.md
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingTlsCommon.md
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/LoggingUseTls.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/MutualAuthentication.md
+-rw-r--r--   0        0        0    17143 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/MutualAuthenticationApi.md
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/MutualAuthenticationData.md
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/MutualAuthenticationDataAttributes.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/MutualAuthenticationResponse.md
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/MutualAuthenticationResponseAttributes.md
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/MutualAuthenticationResponseAttributesAllOf.md
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/MutualAuthenticationResponseData.md
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/MutualAuthenticationResponseDataAllOf.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/MutualAuthenticationsResponse.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/MutualAuthenticationsResponseAllOf.md
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/NumberVersion.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Package.md
+-rw-r--r--   0        0        0     6678 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PackageApi.md
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PackageMetadata.md
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PackageResponse.md
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PackageResponseAllOf.md
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Pagination.md
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PaginationLinks.md
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PaginationMeta.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Permission.md
+-rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Pool.md
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PoolAllOf.md
+-rw-r--r--   0        0        0    29387 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PoolApi.md
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PoolResponse.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PoolResponseAllOf.md
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Pop.md
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PopApi.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PopCoordinates.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PublicIpList.md
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PublicIpListApi.md
+-rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PublishApi.md
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PublishItem.md
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PublishItemFormats.md
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PublishRequest.md
+-rw-r--r--   0        0        0    10418 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PurgeApi.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PurgeKeys.md
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PurgeKeysResponse.md
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/PurgeResponse.md
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RateLimiter.md
+-rw-r--r--   0        0        0    21841 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RateLimiterApi.md
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RateLimiterResponse.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RateLimiterResponseAllOf.md
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ReadOnlyIdService.md
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Realtime.md
+-rw-r--r--   0        0        0     8759 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RealtimeApi.md
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RealtimeEntry.md
+-rw-r--r--   0        0        0    27336 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RealtimeMeasurements.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipCommonName.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipCustomer.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipCustomerCustomer.md
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMemberCustomer.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMemberMutualAuthentication.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMemberService.md
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMemberServiceInvitation.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMemberTlsActivation.md
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMemberTlsBulkCertificate.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMemberTlsCertificate.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMemberTlsConfiguration.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMemberTlsDnsRecord.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMemberTlsDomain.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMemberTlsPrivateKey.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMemberTlsSubscription.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMemberWafActiveRule.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMemberWafFirewall.md
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMemberWafFirewallVersion.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMemberWafRule.md
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMemberWafRuleRevision.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMemberWafTag.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMutualAuthentication.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMutualAuthenticationMutualAuthentication.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMutualAuthentications.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipMutualAuthenticationsMutualAuthentications.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipService.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipServiceInvitations.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipServiceInvitationsCreate.md
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipServiceInvitationsCreateServiceInvitations.md
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipServiceInvitationsServiceInvitations.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipServices.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipServicesServices.md
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsActivation.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsActivationTlsActivation.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsActivations.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsBulkCertificate.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsBulkCertificateTlsBulkCertificate.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsBulkCertificates.md
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsCertificate.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsCertificateTlsCertificate.md
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsCertificates.md
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsCertificatesTlsCertificates.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsConfiguration.md
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsConfigurationForTlsSubscription.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsConfigurationTlsConfiguration.md
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsConfigurations.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsConfigurationsTlsConfigurations.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsDnsRecord.md
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsDnsRecordDnsRecord.md
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsDnsRecords.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsDomain.md
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsDomainTlsDomain.md
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsDomains.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsDomainsTlsDomains.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsPrivateKey.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsPrivateKeyTlsPrivateKey.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsPrivateKeys.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsPrivateKeysTlsPrivateKeys.md
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsSubscription.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsSubscriptionTlsSubscription.md
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipTlsSubscriptions.md
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipUser.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipUserUser.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipWafActiveRules.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipWafActiveRulesWafActiveRules.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipWafFirewall.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipWafFirewallVersion.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipWafFirewallVersionWafFirewallVersion.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipWafFirewallVersions.md
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipWafFirewallWafFirewall.md
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipWafRule.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipWafRuleRevision.md
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipWafRuleRevisionWafRuleRevisions.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipWafRuleRevisions.md
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipWafRuleWafRule.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipWafRules.md
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipWafTags.md
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipWafTagsWafTags.md
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipsForInvitation.md
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipsForMutualAuthentication.md
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipsForStar.md
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipsForTlsActivation.md
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipsForTlsBulkCertificate.md
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipsForTlsConfiguration.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipsForTlsDomain.md
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipsForTlsPrivateKey.md
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipsForTlsSubscription.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipsForWafActiveRule.md
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipsForWafExclusion.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipsForWafFirewallVersion.md
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RelationshipsForWafRule.md
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RequestSettings.md
+-rw-r--r--   0        0        0    15635 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RequestSettingsApi.md
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RequestSettingsResponse.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Resource.md
+-rw-r--r--   0        0        0    15552 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ResourceApi.md
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ResourceResponse.md
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ResourceResponseAllOf.md
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ResponseObject.md
+-rw-r--r--   0        0        0     8900 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ResponseObjectApi.md
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ResponseObjectResponse.md
+-rw-r--r--   0        0        0    27224 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Results.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/RoleUser.md
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/SchemasContactResponse.md
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/SchemasSnippetResponse.md
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/SchemasUserResponse.md
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/SchemasVclResponse.md
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/SchemasVersion.md
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/SchemasVersionResponse.md
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/SchemasWafFirewallVersion.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/SchemasWafFirewallVersionData.md
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Server.md
+-rw-r--r--   0        0        0    19968 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServerApi.md
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServerResponse.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServerResponseAllOf.md
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Service.md
+-rw-r--r--   0        0        0    22475 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceApi.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceAuthorization.md
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceAuthorizationData.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceAuthorizationDataAttributes.md
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceAuthorizationDataRelationships.md
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceAuthorizationDataRelationshipsUser.md
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceAuthorizationDataRelationshipsUserData.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceAuthorizationResponse.md
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceAuthorizationResponseData.md
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceAuthorizationResponseDataAllOf.md
+-rw-r--r--   0        0        0    16177 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceAuthorizationsApi.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceAuthorizationsResponse.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceAuthorizationsResponseAllOf.md
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceCreate.md
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceCreateAllOf.md
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceDetail.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceDetailAllOf.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceIdAndVersion.md
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceInvitation.md
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceInvitationData.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceInvitationDataAttributes.md
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceInvitationDataRelationships.md
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceInvitationResponse.md
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceInvitationResponseAllOf.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceInvitationResponseAllOfData.md
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceListResponse.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceListResponseAllOf.md
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceResponse.md
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceResponseAllOf.md
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceVersionDetail.md
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ServiceVersionDetailOrNull.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Settings.md
+-rw-r--r--   0        0        0     7419 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/SettingsApi.md
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/SettingsResponse.md
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Snippet.md
+-rw-r--r--   0        0        0    19437 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/SnippetApi.md
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/SnippetResponse.md
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/SnippetResponseAllOf.md
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Star.md
+-rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/StarApi.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/StarData.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/StarResponse.md
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/StarResponseAllOf.md
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Stats.md
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/StatsApi.md
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Store.md
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/StoreResponse.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Timestamps.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TimestampsNoDelete.md
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsActivation.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsActivationData.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsActivationResponse.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsActivationResponseData.md
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsActivationResponseDataAllOf.md
+-rw-r--r--   0        0        0    16586 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsActivationsApi.md
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsActivationsResponse.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsActivationsResponseAllOf.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsBulkCertificate.md
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsBulkCertificateData.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsBulkCertificateDataAttributes.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsBulkCertificateResponse.md
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsBulkCertificateResponseAttributes.md
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsBulkCertificateResponseAttributesAllOf.md
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsBulkCertificateResponseData.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsBulkCertificateResponseDataAllOf.md
+-rw-r--r--   0        0        0    16217 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsBulkCertificatesApi.md
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsBulkCertificatesResponse.md
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsBulkCertificatesResponseAllOf.md
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsCertificate.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsCertificateData.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsCertificateDataAttributes.md
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsCertificateResponse.md
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsCertificateResponseAttributes.md
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsCertificateResponseAttributesAllOf.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsCertificateResponseData.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsCertificateResponseDataAllOf.md
+-rw-r--r--   0        0        0    17205 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsCertificatesApi.md
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsCertificatesResponse.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsCertificatesResponseAllOf.md
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsCommon.md
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsConfiguration.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsConfigurationData.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsConfigurationDataAttributes.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsConfigurationResponse.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsConfigurationResponseAttributes.md
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsConfigurationResponseAttributesAllOf.md
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsConfigurationResponseData.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsConfigurationResponseDataAllOf.md
+-rw-r--r--   0        0        0    10339 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsConfigurationsApi.md
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsConfigurationsResponse.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsConfigurationsResponseAllOf.md
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsDnsRecord.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsDomainData.md
+-rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsDomainsApi.md
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsDomainsResponse.md
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsDomainsResponseAllOf.md
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsPrivateKey.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsPrivateKeyData.md
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsPrivateKeyDataAttributes.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsPrivateKeyResponse.md
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsPrivateKeyResponseAttributes.md
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsPrivateKeyResponseAttributesAllOf.md
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsPrivateKeyResponseData.md
+-rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsPrivateKeysApi.md
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsPrivateKeysResponse.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsPrivateKeysResponseAllOf.md
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsSubscription.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsSubscriptionData.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsSubscriptionDataAttributes.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsSubscriptionResponse.md
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsSubscriptionResponseAttributes.md
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsSubscriptionResponseAttributesAllOf.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsSubscriptionResponseData.md
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsSubscriptionResponseDataAllOf.md
+-rw-r--r--   0        0        0    26148 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsSubscriptionsApi.md
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsSubscriptionsResponse.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TlsSubscriptionsResponseAllOf.md
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Token.md
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TokenCreatedResponse.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TokenCreatedResponseAllOf.md
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TokenResponse.md
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TokenResponseAllOf.md
+-rw-r--r--   0        0        0    14773 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TokensApi.md
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeBillingAddress.md
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeContact.md
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeCustomer.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeEvent.md
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeInvitation.md
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeMutualAuthentication.md
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeResource.md
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeService.md
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeServiceAuthorization.md
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeServiceInvitation.md
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeStar.md
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeTlsActivation.md
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeTlsBulkCertificate.md
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeTlsCertificate.md
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeTlsConfiguration.md
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeTlsDnsRecord.md
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeTlsDomain.md
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeTlsPrivateKey.md
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeTlsSubscription.md
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeUser.md
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeWafActiveRule.md
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeWafExclusion.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeWafFirewall.md
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeWafFirewallVersion.md
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeWafRule.md
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeWafRuleRevision.md
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/TypeWafTag.md
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/UpdateBillingAddressRequest.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/UpdateBillingAddressRequestData.md
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/User.md
+-rw-r--r--   0        0        0    20765 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/UserApi.md
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/UserResponse.md
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/UserResponseAllOf.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ValidatorResult.md
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/ValidatorResultMessages.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Vcl.md
+-rw-r--r--   0        0        0    32742 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/VclApi.md
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/VclDiff.md
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/VclDiffApi.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/VclResponse.md
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/Version.md
+-rw-r--r--   0        0        0    26131 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/VersionApi.md
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/VersionCreateResponse.md
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/VersionDetail.md
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/VersionDetailSettings.md
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/VersionResponse.md
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/VersionResponseAllOf.md
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafActiveRule.md
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafActiveRuleCreationResponse.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafActiveRuleData.md
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafActiveRuleDataAttributes.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafActiveRuleResponse.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafActiveRuleResponseData.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafActiveRuleResponseDataAllOf.md
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafActiveRuleResponseDataAttributes.md
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafActiveRuleResponseDataAttributesAllOf.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafActiveRuleResponseDataRelationships.md
+-rw-r--r--   0        0        0    27789 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafActiveRulesApi.md
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafActiveRulesResponse.md
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafActiveRulesResponseAllOf.md
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafExclusion.md
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafExclusionData.md
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafExclusionDataAttributes.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafExclusionResponse.md
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafExclusionResponseData.md
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafExclusionResponseDataAllOf.md
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafExclusionResponseDataAttributes.md
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafExclusionResponseDataAttributesAllOf.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafExclusionResponseDataRelationships.md
+-rw-r--r--   0        0        0    19155 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafExclusionsApi.md
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafExclusionsResponse.md
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafExclusionsResponseAllOf.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewall.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewallData.md
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewallDataAttributes.md
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewallResponse.md
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewallResponseData.md
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewallResponseDataAllOf.md
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewallResponseDataAttributes.md
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewallResponseDataAttributesAllOf.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewallVersion.md
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewallVersionData.md
+-rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewallVersionDataAttributes.md
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewallVersionResponse.md
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewallVersionResponseData.md
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewallVersionResponseDataAllOf.md
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewallVersionResponseDataAttributes.md
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewallVersionResponseDataAttributesAllOf.md
+-rw-r--r--   0        0        0    24852 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewallVersionsApi.md
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewallVersionsResponse.md
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewallVersionsResponseAllOf.md
+-rw-r--r--   0        0        0    17211 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewallsApi.md
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewallsResponse.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafFirewallsResponseAllOf.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafRule.md
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafRuleAttributes.md
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafRuleResponse.md
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafRuleResponseData.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafRuleResponseDataAllOf.md
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafRuleRevision.md
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafRuleRevisionAttributes.md
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafRuleRevisionOrLatest.md
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafRuleRevisionResponse.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafRuleRevisionResponseData.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafRuleRevisionResponseDataAllOf.md
+-rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafRuleRevisionsApi.md
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafRuleRevisionsResponse.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafRuleRevisionsResponseAllOf.md
+-rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafRulesApi.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafRulesResponse.md
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafRulesResponseAllOf.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafTag.md
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafTagAttributes.md
+-rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafTagsApi.md
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafTagsResponse.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafTagsResponseAllOf.md
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WafTagsResponseDataItem.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-2.3.0/docs/WsMessageFormat.md
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/__init__.py
+-rw-r--r--   0        0        0    39346 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api_client.py
+-rw-r--r--   0        0        0    18987 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/configuration.py
+-rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/exceptions.py
+-rw-r--r--   0        0        0    82616 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model_utils.py
+-rw-r--r--   0        0        0    14634 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/rest.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/__init__.py
+-rw-r--r--   0        0        0    30565 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/acl_api.py
+-rw-r--r--   0        0        0    37416 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/acl_entry_api.py
+-rw-r--r--   0        0        0    24906 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/apex_redirect_api.py
+-rw-r--r--   0        0        0    54123 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/backend_api.py
+-rw-r--r--   0        0        0    22509 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/billing_address_api.py
+-rw-r--r--   0        0        0    18589 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/billing_api.py
+-rw-r--r--   0        0        0    34253 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/cache_settings_api.py
+-rw-r--r--   0        0        0    34233 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/condition_api.py
+-rw-r--r--   0        0        0    36809 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/config_store_api.py
+-rw-r--r--   0        0        0    42045 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/config_store_item_api.py
+-rw-r--r--   0        0        0    11779 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/contact_api.py
+-rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/content_api.py
+-rw-r--r--   0        0        0    34431 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/customer_api.py
+-rw-r--r--   0        0        0    31732 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/dictionary_api.py
+-rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/dictionary_info_api.py
+-rw-r--r--   0        0        0    46055 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/dictionary_item_api.py
+-rw-r--r--   0        0        0     7987 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/diff_api.py
+-rw-r--r--   0        0        0    26863 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/director_api.py
+-rw-r--r--   0        0        0    20598 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/director_backend_api.py
+-rw-r--r--   0        0        0    42736 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/domain_api.py
+-rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/domain_ownerships_api.py
+-rw-r--r--   0        0        0    17704 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/enabled_products_api.py
+-rw-r--r--   0        0        0    14137 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/events_api.py
+-rw-r--r--   0        0        0    32656 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/gzip_api.py
+-rw-r--r--   0        0        0    38546 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/header_api.py
+-rw-r--r--   0        0        0    37114 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/healthcheck_api.py
+-rw-r--r--   0        0        0    60468 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/historical_api.py
+-rw-r--r--   0        0        0    19550 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/http3_api.py
+-rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/iam_permissions_api.py
+-rw-r--r--   0        0        0    21443 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/iam_roles_api.py
+-rw-r--r--   0        0        0    22768 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/iam_service_groups_api.py
+-rw-r--r--   0        0        0    34358 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/iam_user_groups_api.py
+-rw-r--r--   0        0        0    16493 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/invitations_api.py
+-rw-r--r--   0        0        0    21168 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/kv_store_api.py
+-rw-r--r--   0        0        0    24533 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/kv_store_item_api.py
+-rw-r--r--   0        0        0    45445 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_azureblob_api.py
+-rw-r--r--   0        0        0    40102 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_bigquery_api.py
+-rw-r--r--   0        0        0    45152 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_cloudfiles_api.py
+-rw-r--r--   0        0        0    42863 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_datadog_api.py
+-rw-r--r--   0        0        0    44606 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_digitalocean_api.py
+-rw-r--r--   0        0        0    45229 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_elasticsearch_api.py
+-rw-r--r--   0        0        0    44432 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_ftp_api.py
+-rw-r--r--   0        0        0    44765 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_gcs_api.py
+-rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_heroku_api.py
+-rw-r--r--   0        0        0    36624 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_honeycomb_api.py
+-rw-r--r--   0        0        0    46115 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_https_api.py
+-rw-r--r--   0        0        0    32568 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_kafka_api.py
+-rw-r--r--   0        0        0    28280 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_kinesis_api.py
+-rw-r--r--   0        0        0    38489 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_logentries_api.py
+-rw-r--r--   0        0        0    36081 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_loggly_api.py
+-rw-r--r--   0        0        0    36770 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_logshuttle_api.py
+-rw-r--r--   0        0        0    38558 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_newrelic_api.py
+-rw-r--r--   0        0        0    44042 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_openstack_api.py
+-rw-r--r--   0        0        0    36635 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_papertrail_api.py
+-rw-r--r--   0        0        0    39265 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_pubsub_api.py
+-rw-r--r--   0        0        0    48777 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_s3_api.py
+-rw-r--r--   0        0        0    37469 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_scalyr_api.py
+-rw-r--r--   0        0        0    45357 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_sftp_api.py
+-rw-r--r--   0        0        0    42255 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_splunk_api.py
+-rw-r--r--   0        0        0    36567 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_sumologic_api.py
+-rw-r--r--   0        0        0    43033 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/logging_syslog_api.py
+-rw-r--r--   0        0        0    28852 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/mutual_authentication_api.py
+-rw-r--r--   0        0        0    12896 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/package_api.py
+-rw-r--r--   0        0        0    47354 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/pool_api.py
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/pop_api.py
+-rw-r--r--   0        0        0     5863 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/public_ip_list_api.py
+-rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/publish_api.py
+-rw-r--r--   0        0        0    18435 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/purge_api.py
+-rw-r--r--   0        0        0    43466 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/rate_limiter_api.py
+-rw-r--r--   0        0        0    17852 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/realtime_api.py
+-rw-r--r--   0        0        0    29291 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/request_settings_api.py
+-rw-r--r--   0        0        0    30490 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/resource_api.py
+-rw-r--r--   0        0        0    18747 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/response_object_api.py
+-rw-r--r--   0        0        0    35038 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/server_api.py
+-rw-r--r--   0        0        0    44324 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/service_api.py
+-rw-r--r--   0        0        0    27911 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/service_authorizations_api.py
+-rw-r--r--   0        0        0    13940 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/settings_api.py
+-rw-r--r--   0        0        0    38842 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/snippet_api.py
+-rw-r--r--   0        0        0    20513 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/star_api.py
+-rw-r--r--   0        0        0     7483 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/stats_api.py
+-rw-r--r--   0        0        0    29279 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/tls_activations_api.py
+-rw-r--r--   0        0        0    28695 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/tls_bulk_certificates_api.py
+-rw-r--r--   0        0        0    29585 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/tls_certificates_api.py
+-rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/tls_configurations_api.py
+-rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/tls_domains_api.py
+-rw-r--r--   0        0        0    22120 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/tls_private_keys_api.py
+-rw-r--r--   0        0        0    43908 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/tls_subscriptions_api.py
+-rw-r--r--   0        0        0    29964 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/tokens_api.py
+-rw-r--r--   0        0        0    40392 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/user_api.py
+-rw-r--r--   0        0        0    64804 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/vcl_api.py
+-rw-r--r--   0        0        0     8068 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/vcl_diff_api.py
+-rw-r--r--   0        0        0    51681 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/version_api.py
+-rw-r--r--   0        0        0    46003 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/waf_active_rules_api.py
+-rw-r--r--   0        0        0    33986 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/waf_exclusions_api.py
+-rw-r--r--   0        0        0    36636 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/waf_firewall_versions_api.py
+-rw-r--r--   0        0        0    29601 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/waf_firewalls_api.py
+-rw-r--r--   0        0        0    13840 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/waf_rule_revisions_api.py
+-rw-r--r--   0        0        0    13963 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/waf_rules_api.py
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/api/waf_tags_api.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/apis/__init__.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/__init__.py
+-rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/acl.py
+-rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/acl_entry.py
+-rw-r--r--   0        0        0    17351 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/acl_entry_response.py
+-rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/acl_entry_response_all_of.py
+-rw-r--r--   0        0        0    15915 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/acl_response.py
+-rw-r--r--   0        0        0    12025 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/acl_response_all_of.py
+-rw-r--r--   0        0        0    16586 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/apex_redirect.py
+-rw-r--r--   0        0        0    12580 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/apex_redirect_all_of.py
+-rw-r--r--   0        0        0    14660 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/aws_region.py
+-rw-r--r--   0        0        0    26143 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/backend.py
+-rw-r--r--   0        0        0    30707 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/backend_response.py
+-rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/backend_response_all_of.py
+-rw-r--r--   0        0        0    14085 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/billing.py
+-rw-r--r--   0        0        0    13567 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/billing_address_attributes.py
+-rw-r--r--   0        0        0    12075 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/billing_address_request.py
+-rw-r--r--   0        0        0    12080 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/billing_address_request_data.py
+-rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/billing_address_response.py
+-rw-r--r--   0        0        0    12794 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/billing_address_response_data.py
+-rw-r--r--   0        0        0    11909 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/billing_address_verification_error_response.py
+-rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/billing_address_verification_error_response_errors.py
+-rw-r--r--   0        0        0    16877 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/billing_estimate_response.py
+-rw-r--r--   0        0        0    11787 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/billing_estimate_response_all_of.py
+-rw-r--r--   0        0        0    13188 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/billing_estimate_response_all_of_line.py
+-rw-r--r--   0        0        0    11784 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/billing_estimate_response_all_of_lines.py
+-rw-r--r--   0        0        0    16765 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/billing_response.py
+-rw-r--r--   0        0        0    11716 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/billing_response_all_of.py
+-rw-r--r--   0        0        0    18617 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/billing_response_line_item.py
+-rw-r--r--   0        0        0    15190 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/billing_response_line_item_all_of.py
+-rw-r--r--   0        0        0    12041 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/billing_status.py
+-rw-r--r--   0        0        0    16362 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/billing_total.py
+-rw-r--r--   0        0        0    12157 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/billing_total_extras.py
+-rw-r--r--   0        0        0    11687 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/bulk_update_acl_entries_request.py
+-rw-r--r--   0        0        0    15994 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/bulk_update_acl_entry.py
+-rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/bulk_update_acl_entry_all_of.py
+-rw-r--r--   0        0        0    14518 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/bulk_update_config_store_item.py
+-rw-r--r--   0        0        0    11587 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/bulk_update_config_store_item_all_of.py
+-rw-r--r--   0        0        0    11742 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/bulk_update_config_store_list_request.py
+-rw-r--r--   0        0        0    14509 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/bulk_update_dictionary_item.py
+-rw-r--r--   0        0        0    11731 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/bulk_update_dictionary_list_request.py
+-rw-r--r--   0        0        0    11735 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/bulk_waf_active_rule.py
+-rw-r--r--   0        0        0    11638 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/bulk_waf_active_rules.py
+-rw-r--r--   0        0        0    13506 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/cache_setting.py
+-rw-r--r--   0        0        0    17524 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/cache_setting_response.py
+-rw-r--r--   0        0        0    13530 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/condition.py
+-rw-r--r--   0        0        0    16896 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/condition_response.py
+-rw-r--r--   0        0        0    11911 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/conditions_response.py
+-rw-r--r--   0        0        0    11444 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/config_store.py
+-rw-r--r--   0        0        0    11552 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/config_store_info_response.py
+-rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/config_store_item.py
+-rw-r--r--   0        0        0    15611 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/config_store_item_response.py
+-rw-r--r--   0        0        0    11487 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/config_store_item_response_all_of.py
+-rw-r--r--   0        0        0    15289 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/config_store_response.py
+-rw-r--r--   0        0        0    11519 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/config_store_response_all_of.py
+-rw-r--r--   0        0        0    13577 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/contact.py
+-rw-r--r--   0        0        0    17300 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/contact_response.py
+-rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/contact_response_all_of.py
+-rw-r--r--   0        0        0    12747 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/content.py
+-rw-r--r--   0        0        0    20398 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/customer.py
+-rw-r--r--   0        0        0    24131 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/customer_response.py
+-rw-r--r--   0        0        0    11430 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/customer_response_all_of.py
+-rw-r--r--   0        0        0    12110 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/dictionary.py
+-rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/dictionary_info_response.py
+-rw-r--r--   0        0        0    11765 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/dictionary_item.py
+-rw-r--r--   0        0        0    15870 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/dictionary_item_response.py
+-rw-r--r--   0        0        0    11758 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/dictionary_item_response_all_of.py
+-rw-r--r--   0        0        0    16499 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/dictionary_response.py
+-rw-r--r--   0        0        0    11436 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/dictionary_response_all_of.py
+-rw-r--r--   0        0        0    12481 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/diff_response.py
+-rw-r--r--   0        0        0    14620 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/director.py
+-rw-r--r--   0        0        0    15768 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/director_backend.py
+-rw-r--r--   0        0        0    11747 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/director_backend_all_of.py
+-rw-r--r--   0        0        0    18553 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/director_response.py
+-rw-r--r--   0        0        0    11783 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/domain.py
+-rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/domain_check_item.py
+-rw-r--r--   0        0        0    11897 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/domain_check_response.py
+-rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/domain_check_response_list.py
+-rw-r--r--   0        0        0    15770 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/domain_response.py
+-rw-r--r--   0        0        0    11875 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/domains_response.py
+-rw-r--r--   0        0        0    12604 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/enabled_product_response.py
+-rw-r--r--   0        0        0    11739 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/enabled_product_response_links.py
+-rw-r--r--   0        0        0    11694 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/enabled_product_response_product.py
+-rw-r--r--   0        0        0    11694 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/enabled_product_response_service.py
+-rw-r--r--   0        0        0    12088 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/event.py
+-rw-r--r--   0        0        0    21129 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/event_attributes.py
+-rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/event_response.py
+-rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/events_response.py
+-rw-r--r--   0        0        0    11554 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/events_response_all_of.py
+-rw-r--r--   0        0        0    11395 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/generic_token_error.py
+-rw-r--r--   0        0        0    12758 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/gzip.py
+-rw-r--r--   0        0        0    16735 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/gzip_response.py
+-rw-r--r--   0        0        0    15905 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/header.py
+-rw-r--r--   0        0        0    19828 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/header_response.py
+-rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/healthcheck.py
+-rw-r--r--   0        0        0    18979 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/healthcheck_response.py
+-rw-r--r--   0        0        0    12267 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical.py
+-rw-r--r--   0        0        0    14970 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_aggregate_response.py
+-rw-r--r--   0        0        0    11672 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_aggregate_response_all_of.py
+-rw-r--r--   0        0        0    15047 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_field_aggregate_response.py
+-rw-r--r--   0        0        0    11723 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_field_aggregate_response_all_of.py
+-rw-r--r--   0        0        0    15024 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_field_response.py
+-rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_field_response_data_field.py
+-rw-r--r--   0        0        0    12060 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_field_results.py
+-rw-r--r--   0        0        0   100322 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_field_results_attributes.py
+-rw-r--r--   0        0        0    11927 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_field_results_attributes_all_of.py
+-rw-r--r--   0        0        0    11919 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_meta.py
+-rw-r--r--   0        0        0    14797 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_regions_response.py
+-rw-r--r--   0        0        0    11445 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_regions_response_all_of.py
+-rw-r--r--   0        0        0    15219 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_response.py
+-rw-r--r--   0        0        0    11959 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_response_data_field.py
+-rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_results.py
+-rw-r--r--   0        0        0    11620 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_service.py
+-rw-r--r--   0        0        0    11367 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_services.py
+-rw-r--r--   0        0        0    15037 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_usage_aggregate_response.py
+-rw-r--r--   0        0        0    15087 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_usage_month_response.py
+-rw-r--r--   0        0        0    11783 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_usage_month_response_all_of.py
+-rw-r--r--   0        0        0    12331 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_usage_month_response_data.py
+-rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_usage_results.py
+-rw-r--r--   0        0        0    15031 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_usage_service_response.py
+-rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/historical_usage_service_response_all_of.py
+-rw-r--r--   0        0        0    15675 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/http3.py
+-rw-r--r--   0        0        0    11705 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/http3_all_of.py
+-rw-r--r--   0        0        0    12796 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/http_response_format.py
+-rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/http_stream_format.py
+-rw-r--r--   0        0        0    13211 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/iam_permission.py
+-rw-r--r--   0        0        0    15987 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/iam_role.py
+-rw-r--r--   0        0        0    12962 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/iam_role_all_of.py
+-rw-r--r--   0        0        0    15636 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/iam_service_group.py
+-rw-r--r--   0        0        0    12570 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/iam_service_group_all_of.py
+-rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/iam_user_group.py
+-rw-r--r--   0        0        0    12926 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/iam_user_group_all_of.py
+-rw-r--r--   0        0        0    12044 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/included_with_waf_active_rule.py
+-rw-r--r--   0        0        0    15142 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/included_with_waf_active_rule_item.py
+-rw-r--r--   0        0        0    12031 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/included_with_waf_exclusion.py
+-rw-r--r--   0        0        0    14619 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/included_with_waf_exclusion_item.py
+-rw-r--r--   0        0        0    12000 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/included_with_waf_firewall.py
+-rw-r--r--   0        0        0    12104 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/included_with_waf_firewall_version.py
+-rw-r--r--   0        0        0    13972 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/included_with_waf_firewall_version_item.py
+-rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/included_with_waf_rule.py
+-rw-r--r--   0        0        0    14599 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/included_with_waf_rule_item.py
+-rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/included_with_waf_rule_revision.py
+-rw-r--r--   0        0        0    11416 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/inline_object.py
+-rw-r--r--   0        0        0    11419 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/inline_object1.py
+-rw-r--r--   0        0        0    11418 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/inline_response200.py
+-rw-r--r--   0        0        0    11605 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/inline_response2001.py
+-rw-r--r--   0        0        0    11985 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/inline_response2002.py
+-rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/inline_response2002_meta.py
+-rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/inline_response2003.py
+-rw-r--r--   0        0        0    11633 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/inline_response2003_meta.py
+-rw-r--r--   0        0        0    11585 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/invitation.py
+-rw-r--r--   0        0        0    12539 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/invitation_data.py
+-rw-r--r--   0        0        0    12611 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/invitation_data_attributes.py
+-rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/invitation_response.py
+-rw-r--r--   0        0        0    11681 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/invitation_response_all_of.py
+-rw-r--r--   0        0        0    14895 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/invitation_response_data.py
+-rw-r--r--   0        0        0    12283 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/invitation_response_data_all_of.py
+-rw-r--r--   0        0        0    14597 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/invitations_response.py
+-rw-r--r--   0        0        0    11690 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/invitations_response_all_of.py
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_address_and_port.py
+-rw-r--r--   0        0        0    22489 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_azureblob.py
+-rw-r--r--   0        0        0    14206 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_azureblob_all_of.py
+-rw-r--r--   0        0        0    24022 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_azureblob_response.py
+-rw-r--r--   0        0        0    19390 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_bigquery.py
+-rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_bigquery_all_of.py
+-rw-r--r--   0        0        0    20943 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_bigquery_response.py
+-rw-r--r--   0        0        0    21831 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_cloudfiles.py
+-rw-r--r--   0        0        0    13543 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_cloudfiles_all_of.py
+-rw-r--r--   0        0        0    23364 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_cloudfiles_response.py
+-rw-r--r--   0        0        0    14144 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_common.py
+-rw-r--r--   0        0        0    23211 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_datadog.py
+-rw-r--r--   0        0        0    18487 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_datadog_all_of.py
+-rw-r--r--   0        0        0    24914 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_datadog_response.py
+-rw-r--r--   0        0        0    21812 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_digitalocean.py
+-rw-r--r--   0        0        0    13514 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_digitalocean_all_of.py
+-rw-r--r--   0        0        0    23345 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_digitalocean_response.py
+-rw-r--r--   0        0        0    22734 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_elasticsearch.py
+-rw-r--r--   0        0        0    14289 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_elasticsearch_all_of.py
+-rw-r--r--   0        0        0    24096 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_elasticsearch_response.py
+-rw-r--r--   0        0        0    12403 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_format_version.py
+-rw-r--r--   0        0        0    22023 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_ftp.py
+-rw-r--r--   0        0        0    13770 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_ftp_all_of.py
+-rw-r--r--   0        0        0    23556 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_ftp_response.py
+-rw-r--r--   0        0        0    22679 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_gcs.py
+-rw-r--r--   0        0        0    12744 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_gcs_all_of.py
+-rw-r--r--   0        0        0    12815 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_gcs_common.py
+-rw-r--r--   0        0        0    24062 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_gcs_response.py
+-rw-r--r--   0        0        0    14090 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_generic_common.py
+-rw-r--r--   0        0        0    18898 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_google_pubsub.py
+-rw-r--r--   0        0        0    12402 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_google_pubsub_all_of.py
+-rw-r--r--   0        0        0    20451 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_google_pubsub_response.py
+-rw-r--r--   0        0        0    17238 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_heroku.py
+-rw-r--r--   0        0        0    11999 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_heroku_all_of.py
+-rw-r--r--   0        0        0    18941 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_heroku_response.py
+-rw-r--r--   0        0        0    17018 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_honeycomb.py
+-rw-r--r--   0        0        0    12284 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_honeycomb_all_of.py
+-rw-r--r--   0        0        0    18721 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_honeycomb_response.py
+-rw-r--r--   0        0        0    23100 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_https.py
+-rw-r--r--   0        0        0    15781 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_https_all_of.py
+-rw-r--r--   0        0        0    24462 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_https_response.py
+-rw-r--r--   0        0        0    23053 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_kafka.py
+-rw-r--r--   0        0        0    15405 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_kafka_all_of.py
+-rw-r--r--   0        0        0    24606 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_kafka_response.py
+-rw-r--r--   0        0        0    16368 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_kinesis.py
+-rw-r--r--   0        0        0    20332 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_kinesis_response.py
+-rw-r--r--   0        0        0    18046 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_logentries.py
+-rw-r--r--   0        0        0    12851 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_logentries_all_of.py
+-rw-r--r--   0        0        0    19749 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_logentries_response.py
+-rw-r--r--   0        0        0    16993 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_loggly.py
+-rw-r--r--   0        0        0    11754 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_loggly_all_of.py
+-rw-r--r--   0        0        0    18696 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_loggly_response.py
+-rw-r--r--   0        0        0    17065 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_logshuttle.py
+-rw-r--r--   0        0        0    11806 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_logshuttle_all_of.py
+-rw-r--r--   0        0        0    18768 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_logshuttle_response.py
+-rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_message_type.py
+-rw-r--r--   0        0        0    18795 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_newrelic.py
+-rw-r--r--   0        0        0    14066 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_newrelic_all_of.py
+-rw-r--r--   0        0        0    20498 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_newrelic_response.py
+-rw-r--r--   0        0        0    21509 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_openstack.py
+-rw-r--r--   0        0        0    13226 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_openstack_all_of.py
+-rw-r--r--   0        0        0    23042 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_openstack_response.py
+-rw-r--r--   0        0        0    17068 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_papertrail.py
+-rw-r--r--   0        0        0    18776 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_papertrail_response.py
+-rw-r--r--   0        0        0    12818 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_placement.py
+-rw-r--r--   0        0        0    12265 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_request_caps_common.py
+-rw-r--r--   0        0        0    24622 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_s3.py
+-rw-r--r--   0        0        0    16374 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_s3_all_of.py
+-rw-r--r--   0        0        0    26155 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_s3_response.py
+-rw-r--r--   0        0        0    17727 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_scalyr.py
+-rw-r--r--   0        0        0    12488 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_scalyr_all_of.py
+-rw-r--r--   0        0        0    19430 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_scalyr_response.py
+-rw-r--r--   0        0        0    22808 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_sftp.py
+-rw-r--r--   0        0        0    14123 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_sftp_all_of.py
+-rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_sftp_response.py
+-rw-r--r--   0        0        0    21030 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_splunk.py
+-rw-r--r--   0        0        0    12164 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_splunk_all_of.py
+-rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_splunk_response.py
+-rw-r--r--   0        0        0    17102 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_sumologic.py
+-rw-r--r--   0        0        0    11912 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_sumologic_all_of.py
+-rw-r--r--   0        0        0    18805 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_sumologic_response.py
+-rw-r--r--   0        0        0    21452 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_syslog.py
+-rw-r--r--   0        0        0    13046 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_syslog_all_of.py
+-rw-r--r--   0        0        0    22829 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_syslog_response.py
+-rw-r--r--   0        0        0    13547 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_tls_common.py
+-rw-r--r--   0        0        0    11595 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/logging_use_tls.py
+-rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/mutual_authentication.py
+-rw-r--r--   0        0        0    12711 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/mutual_authentication_data.py
+-rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/mutual_authentication_data_attributes.py
+-rw-r--r--   0        0        0    11767 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/mutual_authentication_response.py
+-rw-r--r--   0        0        0    15149 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/mutual_authentication_response_attributes.py
+-rw-r--r--   0        0        0    11647 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/mutual_authentication_response_attributes_all_of.py
+-rw-r--r--   0        0        0    15368 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/mutual_authentication_response_data.py
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/mutual_authentication_response_data_all_of.py
+-rw-r--r--   0        0        0    14749 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/mutual_authentications_response.py
+-rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/mutual_authentications_response_all_of.py
+-rw-r--r--   0        0        0    11906 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/number_version.py
+-rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/package.py
+-rw-r--r--   0        0        0    13175 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/package_metadata.py
+-rw-r--r--   0        0        0    15990 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/package_response.py
+-rw-r--r--   0        0        0    11519 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/package_response_all_of.py
+-rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/pagination.py
+-rw-r--r--   0        0        0    12267 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/pagination_links.py
+-rw-r--r--   0        0        0    12484 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/pagination_meta.py
+-rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/permission.py
+-rw-r--r--   0        0        0    23511 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/pool.py
+-rw-r--r--   0        0        0    18578 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/pool_all_of.py
+-rw-r--r--   0        0        0    25586 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/pool_response.py
+-rw-r--r--   0        0        0    11418 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/pool_response_all_of.py
+-rw-r--r--   0        0        0    15216 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/pop.py
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/pop_coordinates.py
+-rw-r--r--   0        0        0    11742 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/public_ip_list.py
+-rw-r--r--   0        0        0    12528 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/publish_item.py
+-rw-r--r--   0        0        0    12411 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/publish_item_formats.py
+-rw-r--r--   0        0        0    11685 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/publish_request.py
+-rw-r--r--   0        0        0    11432 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/purge_keys.py
+-rw-r--r--   0        0        0    11165 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/purge_keys_response.py
+-rw-r--r--   0        0        0    11594 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/purge_response.py
+-rw-r--r--   0        0        0    19010 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/rate_limiter.py
+-rw-r--r--   0        0        0    23485 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/rate_limiter_response.py
+-rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/rate_limiter_response_all_of.py
+-rw-r--r--   0        0        0    10947 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/read_only_id_service.py
+-rw-r--r--   0        0        0    12619 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/realtime.py
+-rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/realtime_entry.py
+-rw-r--r--   0        0        0    98045 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/realtime_measurements.py
+-rw-r--r--   0        0        0    11749 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_common_name.py
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_customer.py
+-rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_customer_customer.py
+-rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_member_customer.py
+-rw-r--r--   0        0        0    11936 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_member_mutual_authentication.py
+-rw-r--r--   0        0        0    11805 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_member_service.py
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_member_service_invitation.py
+-rw-r--r--   0        0        0    11866 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_member_tls_activation.py
+-rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_member_tls_bulk_certificate.py
+-rw-r--r--   0        0        0    11876 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_member_tls_certificate.py
+-rw-r--r--   0        0        0    11896 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_member_tls_configuration.py
+-rw-r--r--   0        0        0    11857 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_member_tls_dns_record.py
+-rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_member_tls_domain.py
+-rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_member_tls_private_key.py
+-rw-r--r--   0        0        0    11886 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_member_tls_subscription.py
+-rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_member_waf_active_rule.py
+-rw-r--r--   0        0        0    11846 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_member_waf_firewall.py
+-rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_member_waf_firewall_version.py
+-rw-r--r--   0        0        0    11806 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_member_waf_rule.py
+-rw-r--r--   0        0        0    11995 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_member_waf_rule_revision.py
+-rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_member_waf_tag.py
+-rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_mutual_authentication.py
+-rw-r--r--   0        0        0    11881 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_mutual_authentication_mutual_authentication.py
+-rw-r--r--   0        0        0    12027 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_mutual_authentications.py
+-rw-r--r--   0        0        0    11893 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_mutual_authentications_mutual_authentications.py
+-rw-r--r--   0        0        0    11705 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_service.py
+-rw-r--r--   0        0        0    11961 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_service_invitations.py
+-rw-r--r--   0        0        0    12022 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_service_invitations_create.py
+-rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_service_invitations_create_service_invitations.py
+-rw-r--r--   0        0        0    11854 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_service_invitations_service_invitations.py
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_services.py
+-rw-r--r--   0        0        0    11723 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_services_services.py
+-rw-r--r--   0        0        0    11851 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_activation.py
+-rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_activation_tls_activation.py
+-rw-r--r--   0        0        0    11859 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_activations.py
+-rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_bulk_certificate.py
+-rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_bulk_certificate_tls_bulk_certificate.py
+-rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_bulk_certificates.py
+-rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_certificate.py
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_certificate_tls_certificate.py
+-rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_certificates.py
+-rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_certificates_tls_certificates.py
+-rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_configuration.py
+-rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_configuration_for_tls_subscription.py
+-rw-r--r--   0        0        0    11829 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_configuration_tls_configuration.py
+-rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_configurations.py
+-rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_configurations_tls_configurations.py
+-rw-r--r--   0        0        0    11794 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_dns_record.py
+-rw-r--r--   0        0        0    11775 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_dns_record_dns_record.py
+-rw-r--r--   0        0        0    11802 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_dns_records.py
+-rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_domain.py
+-rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_domain_tls_domain.py
+-rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_domains.py
+-rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_domains_tls_domains.py
+-rw-r--r--   0        0        0    11858 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_private_key.py
+-rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_private_key_tls_private_key.py
+-rw-r--r--   0        0        0    11880 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_private_keys.py
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_private_keys_tls_private_keys.py
+-rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_subscription.py
+-rw-r--r--   0        0        0    11822 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_subscription_tls_subscription.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_tls_subscriptions.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_user.py
+-rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_user_user.py
+-rw-r--r--   0        0        0    11880 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_waf_active_rules.py
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_waf_active_rules_waf_active_rules.py
+-rw-r--r--   0        0        0    11807 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_waf_firewall.py
+-rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_waf_firewall_version.py
+-rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_waf_firewall_version_waf_firewall_version.py
+-rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_waf_firewall_versions.py
+-rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_waf_firewall_waf_firewall.py
+-rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_waf_rule.py
+-rw-r--r--   0        0        0    11914 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_waf_rule_revision.py
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_waf_rule_revision_waf_rule_revisions.py
+-rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_waf_rule_revisions.py
+-rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_waf_rule_waf_rule.py
+-rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_waf_rules.py
+-rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_waf_tags.py
+-rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationship_waf_tags_waf_tags.py
+-rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationships_for_invitation.py
+-rw-r--r--   0        0        0    14050 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationships_for_mutual_authentication.py
+-rw-r--r--   0        0        0    14345 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationships_for_star.py
+-rw-r--r--   0        0        0    15491 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationships_for_tls_activation.py
+-rw-r--r--   0        0        0    14690 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationships_for_tls_bulk_certificate.py
+-rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationships_for_tls_configuration.py
+-rw-r--r--   0        0        0    14687 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationships_for_tls_domain.py
+-rw-r--r--   0        0        0    14589 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationships_for_tls_private_key.py
+-rw-r--r--   0        0        0    16266 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationships_for_tls_subscription.py
+-rw-r--r--   0        0        0    14951 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationships_for_waf_active_rule.py
+-rw-r--r--   0        0        0    14691 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationships_for_waf_exclusion.py
+-rw-r--r--   0        0        0    14940 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationships_for_waf_firewall_version.py
+-rw-r--r--   0        0        0    14666 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/relationships_for_waf_rule.py
+-rw-r--r--   0        0        0    15858 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/request_settings.py
+-rw-r--r--   0        0        0    19891 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/request_settings_response.py
+-rw-r--r--   0        0        0    11736 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/resource.py
+-rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/resource_response.py
+-rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/resource_response_all_of.py
+-rw-r--r--   0        0        0    13673 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/response_object.py
+-rw-r--r--   0        0        0    17701 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/response_object_response.py
+-rw-r--r--   0        0        0    97280 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/results.py
+-rw-r--r--   0        0        0    12451 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/role_user.py
+-rw-r--r--   0        0        0    17321 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/schemas_contact_response.py
+-rw-r--r--   0        0        0    17519 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/schemas_snippet_response.py
+-rw-r--r--   0        0        0    18068 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/schemas_user_response.py
+-rw-r--r--   0        0        0    15953 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/schemas_vcl_response.py
+-rw-r--r--   0        0        0    13626 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/schemas_version.py
+-rw-r--r--   0        0        0    17433 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/schemas_version_response.py
+-rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/schemas_waf_firewall_version.py
+-rw-r--r--   0        0        0    12179 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/schemas_waf_firewall_version_data.py
+-rw-r--r--   0        0        0    14569 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/server.py
+-rw-r--r--   0        0        0    18752 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/server_response.py
+-rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/server_response_all_of.py
+-rw-r--r--   0        0        0    12015 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service.py
+-rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_authorization.py
+-rw-r--r--   0        0        0    12718 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_authorization_data.py
+-rw-r--r--   0        0        0    11658 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_authorization_data_attributes.py
+-rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_authorization_data_relationships.py
+-rw-r--r--   0        0        0    11899 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_authorization_data_relationships_user.py
+-rw-r--r--   0        0        0    11844 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_authorization_data_relationships_user_data.py
+-rw-r--r--   0        0        0    11767 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_authorization_response.py
+-rw-r--r--   0        0        0    15176 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_authorization_response_data.py
+-rw-r--r--   0        0        0    11863 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_authorization_response_data_all_of.py
+-rw-r--r--   0        0        0    14749 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_authorizations_response.py
+-rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_authorizations_response_all_of.py
+-rw-r--r--   0        0        0    14640 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_create.py
+-rw-r--r--   0        0        0    11543 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_create_all_of.py
+-rw-r--r--   0        0        0    18255 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_detail.py
+-rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_detail_all_of.py
+-rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_id_and_version.py
+-rw-r--r--   0        0        0    11656 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_invitation.py
+-rw-r--r--   0        0        0    12646 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_invitation_data.py
+-rw-r--r--   0        0        0    11922 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_invitation_data_attributes.py
+-rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_invitation_data_relationships.py
+-rw-r--r--   0        0        0    14111 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_invitation_response.py
+-rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_invitation_response_all_of.py
+-rw-r--r--   0        0        0    11854 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_invitation_response_all_of_data.py
+-rw-r--r--   0        0        0    17024 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_list_response.py
+-rw-r--r--   0        0        0    12407 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_list_response_all_of.py
+-rw-r--r--   0        0        0    17544 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_response.py
+-rw-r--r--   0        0        0    12948 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_response_all_of.py
+-rw-r--r--   0        0        0    23835 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_version_detail.py
+-rw-r--r--   0        0        0    23852 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/service_version_detail_or_null.py
+-rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/settings.py
+-rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/settings_response.py
+-rw-r--r--   0        0        0    13165 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/snippet.py
+-rw-r--r--   0        0        0    17498 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/snippet_response.py
+-rw-r--r--   0        0        0    12037 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/snippet_response_all_of.py
+-rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/star.py
+-rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/star_data.py
+-rw-r--r--   0        0        0    13825 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/star_response.py
+-rw-r--r--   0        0        0    11571 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/star_response_all_of.py
+-rw-r--r--   0        0        0    11555 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/stats.py
+-rw-r--r--   0        0        0    11440 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/store.py
+-rw-r--r--   0        0        0    11668 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/store_response.py
+-rw-r--r--   0        0        0    12287 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/timestamps.py
+-rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/timestamps_no_delete.py
+-rw-r--r--   0        0        0    11616 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_activation.py
+-rw-r--r--   0        0        0    12100 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_activation_data.py
+-rw-r--r--   0        0        0    11697 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_activation_response.py
+-rw-r--r--   0        0        0    14980 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_activation_response_data.py
+-rw-r--r--   0        0        0    11842 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_activation_response_data_all_of.py
+-rw-r--r--   0        0        0    14644 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_activations_response.py
+-rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_activations_response_all_of.py
+-rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_bulk_certificate.py
+-rw-r--r--   0        0        0    12666 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_bulk_certificate_data.py
+-rw-r--r--   0        0        0    12407 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_bulk_certificate_data_attributes.py
+-rw-r--r--   0        0        0    11748 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_bulk_certificate_response.py
+-rw-r--r--   0        0        0    16192 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_bulk_certificate_response_attributes.py
+-rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_bulk_certificate_response_attributes_all_of.py
+-rw-r--r--   0        0        0    15305 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_bulk_certificate_response_data.py
+-rw-r--r--   0        0        0    12043 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_bulk_certificate_response_data_all_of.py
+-rw-r--r--   0        0        0    14721 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_bulk_certificates_response.py
+-rw-r--r--   0        0        0    11772 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_bulk_certificates_response_all_of.py
+-rw-r--r--   0        0        0    11626 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_certificate.py
+-rw-r--r--   0        0        0    12510 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_certificate_data.py
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_certificate_data_attributes.py
+-rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_certificate_response.py
+-rw-r--r--   0        0        0    17609 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_certificate_response_attributes.py
+-rw-r--r--   0        0        0    14137 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_certificate_response_attributes_all_of.py
+-rw-r--r--   0        0        0    15107 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_certificate_response_data.py
+-rw-r--r--   0        0        0    12002 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_certificate_response_data_all_of.py
+-rw-r--r--   0        0        0    14659 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_certificates_response.py
+-rw-r--r--   0        0        0    11731 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_certificates_response_all_of.py
+-rw-r--r--   0        0        0    13892 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_common.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_configuration.py
+-rw-r--r--   0        0        0    12615 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_configuration_data.py
+-rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_configuration_data_attributes.py
+-rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_configuration_response.py
+-rw-r--r--   0        0        0    16408 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_configuration_response_attributes.py
+-rw-r--r--   0        0        0    12926 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_configuration_response_attributes_all_of.py
+-rw-r--r--   0        0        0    15232 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_configuration_response_data.py
+-rw-r--r--   0        0        0    12022 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_configuration_response_data_all_of.py
+-rw-r--r--   0        0        0    14689 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_configurations_response.py
+-rw-r--r--   0        0        0    11751 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_configurations_response_all_of.py
+-rw-r--r--   0        0        0    13196 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_dns_record.py
+-rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_domain_data.py
+-rw-r--r--   0        0        0    14527 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_domains_response.py
+-rw-r--r--   0        0        0    11624 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_domains_response_all_of.py
+-rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_private_key.py
+-rw-r--r--   0        0        0    12546 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_private_key_data.py
+-rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_private_key_data_attributes.py
+-rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_private_key_response.py
+-rw-r--r--   0        0        0    16480 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_private_key_response_attributes.py
+-rw-r--r--   0        0        0    13012 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_private_key_response_attributes_all_of.py
+-rw-r--r--   0        0        0    12321 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_private_key_response_data.py
+-rw-r--r--   0        0        0    14646 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_private_keys_response.py
+-rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_private_keys_response_all_of.py
+-rw-r--r--   0        0        0    11636 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_subscription.py
+-rw-r--r--   0        0        0    12591 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_subscription_data.py
+-rw-r--r--   0        0        0    11818 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_subscription_data_attributes.py
+-rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_subscription_response.py
+-rw-r--r--   0        0        0    15234 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_subscription_response_attributes.py
+-rw-r--r--   0        0        0    11757 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_subscription_response_attributes_all_of.py
+-rw-r--r--   0        0        0    14191 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_subscription_response_data.py
+-rw-r--r--   0        0        0    12012 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_subscription_response_data_all_of.py
+-rw-r--r--   0        0        0    14645 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_subscriptions_response.py
+-rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/tls_subscriptions_response_all_of.py
+-rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/token.py
+-rw-r--r--   0        0        0    18055 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/token_created_response.py
+-rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/token_created_response_all_of.py
+-rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/token_response.py
+-rw-r--r--   0        0        0    13237 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/token_response_all_of.py
+-rw-r--r--   0        0        0    11733 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_billing_address.py
+-rw-r--r--   0        0        0    11616 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_contact.py
+-rw-r--r--   0        0        0    11631 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_customer.py
+-rw-r--r--   0        0        0    11586 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_event.py
+-rw-r--r--   0        0        0    11661 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_invitation.py
+-rw-r--r--   0        0        0    11823 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_mutual_authentication.py
+-rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_resource.py
+-rw-r--r--   0        0        0    11616 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_service.py
+-rw-r--r--   0        0        0    11823 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_service_authorization.py
+-rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_service_invitation.py
+-rw-r--r--   0        0        0    11571 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_star.py
+-rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_tls_activation.py
+-rw-r--r--   0        0        0    11805 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_tls_bulk_certificate.py
+-rw-r--r--   0        0        0    11733 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_tls_certificate.py
+-rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_tls_configuration.py
+-rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_tls_dns_record.py
+-rw-r--r--   0        0        0    11658 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_tls_domain.py
+-rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_tls_private_key.py
+-rw-r--r--   0        0        0    11748 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_tls_subscription.py
+-rw-r--r--   0        0        0    11571 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_user.py
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_waf_active_rule.py
+-rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_waf_exclusion.py
+-rw-r--r--   0        0        0    11692 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_waf_firewall.py
+-rw-r--r--   0        0        0    11809 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_waf_firewall_version.py
+-rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_waf_rule.py
+-rw-r--r--   0        0        0    11764 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_waf_rule_revision.py
+-rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/type_waf_tag.py
+-rw-r--r--   0        0        0    12136 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/update_billing_address_request.py
+-rw-r--r--   0        0        0    12402 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/update_billing_address_request_data.py
+-rw-r--r--   0        0        0    13820 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/user.py
+-rw-r--r--   0        0        0    18047 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/user_response.py
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/user_response_all_of.py
+-rw-r--r--   0        0        0    12570 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/validator_result.py
+-rw-r--r--   0        0        0    12325 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/validator_result_messages.py
+-rw-r--r--   0        0        0    11960 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/vcl.py
+-rw-r--r--   0        0        0    12644 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/vcl_diff.py
+-rw-r--r--   0        0        0    15932 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/vcl_response.py
+-rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/version.py
+-rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/version_create_response.py
+-rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/version_detail.py
+-rw-r--r--   0        0        0    12978 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/version_detail_settings.py
+-rw-r--r--   0        0        0    17376 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/version_response.py
+-rw-r--r--   0        0        0    11475 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/version_response_all_of.py
+-rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_active_rule.py
+-rw-r--r--   0        0        0    15118 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_active_rule_creation_response.py
+-rw-r--r--   0        0        0    12546 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_active_rule_data.py
+-rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_active_rule_data_attributes.py
+-rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_active_rule_response.py
+-rw-r--r--   0        0        0    15228 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_active_rule_response_data.py
+-rw-r--r--   0        0        0    12559 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_active_rule_response_data_all_of.py
+-rw-r--r--   0        0        0    15589 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_active_rule_response_data_attributes.py
+-rw-r--r--   0        0        0    12100 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_active_rule_response_data_attributes_all_of.py
+-rw-r--r--   0        0        0    14978 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_active_rule_response_data_relationships.py
+-rw-r--r--   0        0        0    15066 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_active_rules_response.py
+-rw-r--r--   0        0        0    12142 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_active_rules_response_all_of.py
+-rw-r--r--   0        0        0    11606 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_exclusion.py
+-rw-r--r--   0        0        0    12519 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_exclusion_data.py
+-rw-r--r--   0        0        0    13837 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_exclusion_data_attributes.py
+-rw-r--r--   0        0        0    11687 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_exclusion_response.py
+-rw-r--r--   0        0        0    15289 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_exclusion_response_data.py
+-rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_exclusion_response_data_all_of.py
+-rw-r--r--   0        0        0    17359 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_exclusion_response_data_attributes.py
+-rw-r--r--   0        0        0    13876 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_exclusion_response_data_attributes_all_of.py
+-rw-r--r--   0        0        0    14718 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_exclusion_response_data_relationships.py
+-rw-r--r--   0        0        0    15041 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_exclusions_response.py
+-rw-r--r--   0        0        0    12123 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_exclusions_response_all_of.py
+-rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_firewall.py
+-rw-r--r--   0        0        0    12037 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_firewall_data.py
+-rw-r--r--   0        0        0    12561 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_firewall_data_attributes.py
+-rw-r--r--   0        0        0    12082 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_firewall_response.py
+-rw-r--r--   0        0        0    15119 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_firewall_response_data.py
+-rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_firewall_response_data_all_of.py
+-rw-r--r--   0        0        0    19383 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_firewall_response_data_attributes.py
+-rw-r--r--   0        0        0    15905 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_firewall_response_data_attributes_all_of.py
+-rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_firewall_version.py
+-rw-r--r--   0        0        0    12158 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_firewall_version_data.py
+-rw-r--r--   0        0        0    24857 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_firewall_version_data_attributes.py
+-rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_firewall_version_response.py
+-rw-r--r--   0        0        0    15440 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_firewall_version_response_data.py
+-rw-r--r--   0        0        0    12686 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_firewall_version_response_data_all_of.py
+-rw-r--r--   0        0        0    20346 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_firewall_version_response_data_attributes.py
+-rw-r--r--   0        0        0    16832 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_firewall_version_response_data_attributes_all_of.py
+-rw-r--r--   0        0        0    15176 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_firewall_versions_response.py
+-rw-r--r--   0        0        0    12227 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_firewall_versions_response_all_of.py
+-rw-r--r--   0        0        0    15019 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_firewalls_response.py
+-rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_firewalls_response_all_of.py
+-rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_rule.py
+-rw-r--r--   0        0        0    12553 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_rule_attributes.py
+-rw-r--r--   0        0        0    12014 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_rule_response.py
+-rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_rule_response_data.py
+-rw-r--r--   0        0        0    11737 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_rule_response_data_all_of.py
+-rw-r--r--   0        0        0    12370 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_rule_revision.py
+-rw-r--r--   0        0        0    13775 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_rule_revision_attributes.py
+-rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_rule_revision_or_latest.py
+-rw-r--r--   0        0        0    12152 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_rule_revision_response.py
+-rw-r--r--   0        0        0    15147 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_rule_revision_response_data.py
+-rw-r--r--   0        0        0    11732 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_rule_revision_response_data_all_of.py
+-rw-r--r--   0        0        0    15110 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_rule_revisions_response.py
+-rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_rule_revisions_response_all_of.py
+-rw-r--r--   0        0        0    14931 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_rules_response.py
+-rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_rules_response_all_of.py
+-rw-r--r--   0        0        0    12195 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_tag.py
+-rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_tag_attributes.py
+-rw-r--r--   0        0        0    14872 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_tags_response.py
+-rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_tags_response_all_of.py
+-rw-r--r--   0        0        0    14941 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/waf_tags_response_data_item.py
+-rw-r--r--   0        0        0    11832 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/model/ws_message_format.py
+-rw-r--r--   0        0        0    45117 2020-02-02 00:00:00.000000 fastly-2.3.0/fastly/models/__init__.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 fastly-2.3.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 fastly-2.3.0/LICENSE
+-rw-r--r--   0        0        0    89149 2020-02-02 00:00:00.000000 fastly-2.3.0/README.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastly-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0    89641 2020-02-02 00:00:00.000000 fastly-2.3.0/PKG-INFO
```

### Comparing `fastly-2.2.2/CHANGELOG.md` & `fastly-2.3.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## [v2.3.0](https://github.com/fastly/fastly-py/releases/tag/release/v2.3.0) (2023-06-27)
+
+**Enhancements:**
+
+- feat(rate_limiter): implement POST/PUT endpoints.
+
+**Bug fixes:**
+
+- fix(historical_stats): extract primitive into custom type.
+
 ## [v2.2.2](https://github.com/fastly/fastly-py/releases/tag/release/v2.2.2) (2023-06-23)
 
 **Bug fixes:**
 
 - fix(historical_stats): generate missing models.
 - fix(historical_stats): apply upstream fix to partial models.
```

### Comparing `fastly-2.2.2/SECURITY.md` & `fastly-2.3.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/setup.py` & `fastly-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 from pathlib import Path
 
 NAME = "fastly"
-VERSION = "2.2.2"
+VERSION = "2.3.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `fastly-2.2.2/.github/scripts/pack.sh` & `fastly-2.3.0/.github/scripts/pack.sh`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/.github/scripts/publish_env.sh` & `fastly-2.3.0/.github/scripts/publish_env.sh`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/.github/scripts/release_body.sh` & `fastly-2.3.0/.github/scripts/release_body.sh`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/.github/workflows/ci-release.yaml` & `fastly-2.3.0/.github/workflows/ci-release.yaml`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Acl.md` & `fastly-2.3.0/docs/Acl.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/AclApi.md` & `fastly-2.3.0/docs/AclApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/AclEntry.md` & `fastly-2.3.0/docs/AclEntry.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/AclEntryApi.md` & `fastly-2.3.0/docs/AclEntryApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/AclEntryResponse.md` & `fastly-2.3.0/docs/AclEntryResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/AclEntryResponseAllOf.md` & `fastly-2.3.0/docs/AclEntryResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/AclResponse.md` & `fastly-2.3.0/docs/AclResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/AclResponseAllOf.md` & `fastly-2.3.0/docs/AclResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ApexRedirect.md` & `fastly-2.3.0/docs/ApexRedirect.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ApexRedirectAllOf.md` & `fastly-2.3.0/docs/ApexRedirectAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ApexRedirectApi.md` & `fastly-2.3.0/docs/ApexRedirectApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/AwsRegion.md` & `fastly-2.3.0/docs/AwsRegion.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Backend.md` & `fastly-2.3.0/docs/Backend.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BackendApi.md` & `fastly-2.3.0/docs/BackendApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BackendResponse.md` & `fastly-2.3.0/docs/BackendResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BackendResponseAllOf.md` & `fastly-2.3.0/docs/BackendResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Billing.md` & `fastly-2.3.0/docs/Billing.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BillingAddressApi.md` & `fastly-2.3.0/docs/BillingAddressApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BillingAddressAttributes.md` & `fastly-2.3.0/docs/BillingAddressAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BillingAddressRequest.md` & `fastly-2.3.0/docs/BillingAddressRequest.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BillingAddressRequestData.md` & `fastly-2.3.0/docs/BillingAddressRequestData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BillingAddressResponse.md` & `fastly-2.3.0/docs/BillingAddressResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BillingAddressResponseData.md` & `fastly-2.3.0/docs/BillingAddressResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BillingAddressVerificationErrorResponse.md` & `fastly-2.3.0/docs/BillingAddressVerificationErrorResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BillingAddressVerificationErrorResponseErrors.md` & `fastly-2.3.0/docs/BillingAddressVerificationErrorResponseErrors.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BillingApi.md` & `fastly-2.3.0/docs/BillingApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BillingEstimateResponse.md` & `fastly-2.3.0/docs/BillingEstimateResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BillingEstimateResponseAllOf.md` & `fastly-2.3.0/docs/BillingEstimateResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BillingEstimateResponseAllOfLine.md` & `fastly-2.3.0/docs/BillingEstimateResponseAllOfLine.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BillingEstimateResponseAllOfLines.md` & `fastly-2.3.0/docs/BillingEstimateResponseAllOfLines.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BillingResponse.md` & `fastly-2.3.0/docs/BillingResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BillingResponseAllOf.md` & `fastly-2.3.0/docs/BillingResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BillingResponseLineItem.md` & `fastly-2.3.0/docs/BillingResponseLineItem.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BillingResponseLineItemAllOf.md` & `fastly-2.3.0/docs/BillingResponseLineItemAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BillingStatus.md` & `fastly-2.3.0/docs/BillingStatus.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BillingTotal.md` & `fastly-2.3.0/docs/BillingTotal.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BillingTotalExtras.md` & `fastly-2.3.0/docs/BillingTotalExtras.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BulkUpdateAclEntriesRequest.md` & `fastly-2.3.0/docs/BulkUpdateAclEntriesRequest.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BulkUpdateAclEntry.md` & `fastly-2.3.0/docs/BulkUpdateAclEntry.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BulkUpdateAclEntryAllOf.md` & `fastly-2.3.0/docs/BulkUpdateAclEntryAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BulkUpdateConfigStoreItem.md` & `fastly-2.3.0/docs/BulkUpdateConfigStoreItem.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BulkUpdateConfigStoreItemAllOf.md` & `fastly-2.3.0/docs/BulkUpdateConfigStoreItemAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BulkUpdateConfigStoreListRequest.md` & `fastly-2.3.0/docs/BulkUpdateConfigStoreListRequest.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BulkUpdateDictionaryItem.md` & `fastly-2.3.0/docs/BulkUpdateDictionaryItem.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BulkUpdateDictionaryListRequest.md` & `fastly-2.3.0/docs/BulkUpdateDictionaryListRequest.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/BulkWafActiveRules.md` & `fastly-2.3.0/docs/BulkWafActiveRules.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/CacheSetting.md` & `fastly-2.3.0/docs/CacheSetting.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/CacheSettingResponse.md` & `fastly-2.3.0/docs/CacheSettingResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/CacheSettingsApi.md` & `fastly-2.3.0/docs/CacheSettingsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Condition.md` & `fastly-2.3.0/docs/Condition.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ConditionApi.md` & `fastly-2.3.0/docs/ConditionApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ConditionResponse.md` & `fastly-2.3.0/docs/ConditionResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ConfigStore.md` & `fastly-2.3.0/docs/ConfigStore.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ConfigStoreApi.md` & `fastly-2.3.0/docs/ConfigStoreApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ConfigStoreInfoResponse.md` & `fastly-2.3.0/docs/ConfigStoreInfoResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ConfigStoreItem.md` & `fastly-2.3.0/docs/ConfigStoreItem.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ConfigStoreItemApi.md` & `fastly-2.3.0/docs/ConfigStoreItemApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ConfigStoreItemResponse.md` & `fastly-2.3.0/docs/ConfigStoreItemResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ConfigStoreItemResponseAllOf.md` & `fastly-2.3.0/docs/ConfigStoreItemResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ConfigStoreResponse.md` & `fastly-2.3.0/docs/ConfigStoreResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ConfigStoreResponseAllOf.md` & `fastly-2.3.0/docs/ConfigStoreResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Contact.md` & `fastly-2.3.0/docs/Contact.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ContactApi.md` & `fastly-2.3.0/docs/ContactApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ContactResponse.md` & `fastly-2.3.0/docs/ContactResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ContactResponseAllOf.md` & `fastly-2.3.0/docs/ContactResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Content.md` & `fastly-2.3.0/docs/Content.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ContentApi.md` & `fastly-2.3.0/docs/ContentApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Customer.md` & `fastly-2.3.0/docs/Customer.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/CustomerApi.md` & `fastly-2.3.0/docs/CustomerApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/CustomerResponse.md` & `fastly-2.3.0/docs/CustomerResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/CustomerResponseAllOf.md` & `fastly-2.3.0/docs/CustomerResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Dictionary.md` & `fastly-2.3.0/docs/Dictionary.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/DictionaryApi.md` & `fastly-2.3.0/docs/DictionaryApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/DictionaryInfoApi.md` & `fastly-2.3.0/docs/DictionaryInfoApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/DictionaryInfoResponse.md` & `fastly-2.3.0/docs/DictionaryInfoResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/DictionaryItem.md` & `fastly-2.3.0/docs/DictionaryItem.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/DictionaryItemApi.md` & `fastly-2.3.0/docs/DictionaryItemApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/DictionaryItemResponse.md` & `fastly-2.3.0/docs/DictionaryItemResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/DictionaryItemResponseAllOf.md` & `fastly-2.3.0/docs/DictionaryItemResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/DictionaryResponse.md` & `fastly-2.3.0/docs/DictionaryResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/DictionaryResponseAllOf.md` & `fastly-2.3.0/docs/DictionaryResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/DiffApi.md` & `fastly-2.3.0/docs/DiffApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/DiffResponse.md` & `fastly-2.3.0/docs/DiffResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Director.md` & `fastly-2.3.0/docs/Director.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/DirectorApi.md` & `fastly-2.3.0/docs/DirectorApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/DirectorBackend.md` & `fastly-2.3.0/docs/DirectorBackend.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/DirectorBackendAllOf.md` & `fastly-2.3.0/docs/DirectorBackendAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/DirectorBackendApi.md` & `fastly-2.3.0/docs/DirectorBackendApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/DirectorResponse.md` & `fastly-2.3.0/docs/DirectorResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Domain.md` & `fastly-2.3.0/docs/Domain.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/DomainApi.md` & `fastly-2.3.0/docs/DomainApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/DomainCheckItem.md` & `fastly-2.3.0/docs/DomainCheckItem.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/DomainOwnershipsApi.md` & `fastly-2.3.0/docs/DomainOwnershipsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/DomainResponse.md` & `fastly-2.3.0/docs/DomainResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/EnabledProductResponse.md` & `fastly-2.3.0/docs/EnabledProductResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/EnabledProductResponseLinks.md` & `fastly-2.3.0/docs/EnabledProductResponseLinks.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/EnabledProductResponseProduct.md` & `fastly-2.3.0/docs/EnabledProductResponseProduct.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/EnabledProductResponseService.md` & `fastly-2.3.0/docs/EnabledProductResponseService.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/EnabledProductsApi.md` & `fastly-2.3.0/docs/EnabledProductsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Event.md` & `fastly-2.3.0/docs/Event.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/EventAttributes.md` & `fastly-2.3.0/docs/EventAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/EventsApi.md` & `fastly-2.3.0/docs/EventsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/EventsResponse.md` & `fastly-2.3.0/docs/EventsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/EventsResponseAllOf.md` & `fastly-2.3.0/docs/EventsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Gzip.md` & `fastly-2.3.0/docs/Gzip.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/GzipApi.md` & `fastly-2.3.0/docs/GzipApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/GzipResponse.md` & `fastly-2.3.0/docs/GzipResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Header.md` & `fastly-2.3.0/docs/Header.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HeaderApi.md` & `fastly-2.3.0/docs/HeaderApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HeaderResponse.md` & `fastly-2.3.0/docs/HeaderResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Healthcheck.md` & `fastly-2.3.0/docs/Healthcheck.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HealthcheckApi.md` & `fastly-2.3.0/docs/HealthcheckApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HealthcheckResponse.md` & `fastly-2.3.0/docs/HealthcheckResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Historical.md` & `fastly-2.3.0/docs/Historical.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HistoricalAggregateResponse.md` & `fastly-2.3.0/docs/HistoricalAggregateResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HistoricalAggregateResponseAllOf.md` & `fastly-2.3.0/docs/HistoricalAggregateResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HistoricalApi.md` & `fastly-2.3.0/docs/HistoricalApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HistoricalFieldAggregateResponse.md` & `fastly-2.3.0/docs/HistoricalFieldAggregateResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HistoricalFieldAggregateResponseAllOf.md` & `fastly-2.3.0/docs/HistoricalFieldAggregateResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HistoricalFieldResponse.md` & `fastly-2.3.0/docs/HistoricalFieldResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HistoricalFieldResponseDataField.md` & `fastly-2.3.0/docs/HistoricalFieldResponseDataField.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HistoricalFieldResultsAttributes.md` & `fastly-2.3.0/docs/HistoricalFieldResultsAttributes.md`

 * *Files 0% similar despite different names*

```diff
@@ -216,14 +216,14 @@
 **fanout_conn_time_ms** | **int** | Total duration of Fanout connections with end users. | [optional] 
 **ddos_action_limit_streams_connections** | **int** | For HTTP/2, the number of connections the limit-streams action was applied to. The limit-streams action caps the allowed number of concurrent streams in a connection. | [optional] 
 **ddos_action_limit_streams_requests** | **int** | For HTTP/2, the number of requests made on a connection for which the limit-streams action was taken. The limit-streams action caps the allowed number of concurrent streams in a connection. | [optional] 
 **ddos_action_tarpit_accept** | **int** | The number of times the tarpit-accept action was taken. The tarpit-accept action adds a delay when accepting future connections. | [optional] 
 **ddos_action_tarpit** | **int** | The number of times the tarpit action was taken. The tarpit action delays writing the response to the client. | [optional] 
 **ddos_action_close** | **int** | The number of times the close action was taken. The close action aborts the connection as soon as possible. The close action takes effect either right after accept, right after the client hello, or right after the response was sent. | [optional] 
 **ddos_action_blackhole** | **int** | The number of times the blackhole action was taken. The blackhole action quietly closes a TCP connection without sending a reset. The blackhole action quietly closes a TCP connection without notifying its peer (all TCP state is dropped). | [optional] 
-**service_id** | **bool, date, datetime, dict, float, int, list, str, none_type** |  | [optional] [readonly] 
+**service_id** | [**ReadOnlyIdService**](ReadOnlyIdService.md) |  | [optional] 
 **start_time** | **int** |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-2.2.2/docs/HistoricalFieldResultsAttributesAllOf.md` & `fastly-2.3.0/docs/InlineResponse2002Meta.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-# HistoricalFieldResultsAttributesAllOf
+# InlineResponse2002Meta
 
+Meta for the pagination.
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**service_id** | **bool, date, datetime, dict, float, int, list, str, none_type** |  | [optional] [readonly] 
-**start_time** | **int** |  | [optional] 
+**next_cursor** | **str** | Cursor for the next page. | [optional] 
+**limit** | **int** | Entries returned. | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-2.2.2/docs/HistoricalMeta.md` & `fastly-2.3.0/docs/HistoricalMeta.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HistoricalRegionsResponse.md` & `fastly-2.3.0/docs/HistoricalRegionsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HistoricalRegionsResponseAllOf.md` & `fastly-2.3.0/docs/HistoricalRegionsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HistoricalResponse.md` & `fastly-2.3.0/docs/HistoricalResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HistoricalResponseDataField.md` & `fastly-2.3.0/docs/HistoricalResponseDataField.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HistoricalService.md` & `fastly-2.3.0/docs/HistoricalService.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HistoricalUsageAggregateResponse.md` & `fastly-2.3.0/docs/HistoricalUsageAggregateResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HistoricalUsageMonthResponse.md` & `fastly-2.3.0/docs/HistoricalUsageMonthResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HistoricalUsageMonthResponseAllOf.md` & `fastly-2.3.0/docs/HistoricalUsageMonthResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HistoricalUsageMonthResponseData.md` & `fastly-2.3.0/docs/HistoricalUsageMonthResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HistoricalUsageResults.md` & `fastly-2.3.0/docs/HistoricalUsageResults.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HistoricalUsageServiceResponse.md` & `fastly-2.3.0/docs/HistoricalUsageServiceResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HistoricalUsageServiceResponseAllOf.md` & `fastly-2.3.0/docs/HistoricalUsageServiceResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Http3.md` & `fastly-2.3.0/docs/Http3.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Http3AllOf.md` & `fastly-2.3.0/docs/Http3AllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Http3Api.md` & `fastly-2.3.0/docs/Http3Api.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HttpResponseFormat.md` & `fastly-2.3.0/docs/HttpResponseFormat.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/HttpStreamFormat.md` & `fastly-2.3.0/docs/HttpStreamFormat.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/IamPermission.md` & `fastly-2.3.0/docs/IamPermission.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/IamPermissionsApi.md` & `fastly-2.3.0/docs/IamPermissionsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/IamRole.md` & `fastly-2.3.0/docs/IamRole.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/IamRoleAllOf.md` & `fastly-2.3.0/docs/IamRoleAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/IamRolesApi.md` & `fastly-2.3.0/docs/IamRolesApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/IamServiceGroup.md` & `fastly-2.3.0/docs/IamServiceGroup.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/IamServiceGroupAllOf.md` & `fastly-2.3.0/docs/IamServiceGroupAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/IamServiceGroupsApi.md` & `fastly-2.3.0/docs/IamServiceGroupsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/IamUserGroup.md` & `fastly-2.3.0/docs/IamUserGroup.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/IamUserGroupAllOf.md` & `fastly-2.3.0/docs/IamUserGroupAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/IamUserGroupsApi.md` & `fastly-2.3.0/docs/IamUserGroupsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/IncludedWithWafActiveRuleItem.md` & `fastly-2.3.0/docs/IncludedWithWafActiveRuleItem.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/IncludedWithWafExclusionItem.md` & `fastly-2.3.0/docs/IncludedWithWafExclusionItem.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/IncludedWithWafFirewallVersionItem.md` & `fastly-2.3.0/docs/IncludedWithWafFirewallVersionItem.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/IncludedWithWafRuleItem.md` & `fastly-2.3.0/docs/IncludedWithWafRuleItem.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/InlineResponse2001.md` & `fastly-2.3.0/docs/InlineResponse2001.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/InlineResponse2002.md` & `fastly-2.3.0/docs/InlineResponse2002.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/InlineResponse2002Meta.md` & `fastly-2.3.0/docs/LoggingSumologicAllOf.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-# InlineResponse2002Meta
+# LoggingSumologicAllOf
 
-Meta for the pagination.
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**next_cursor** | **str** | Cursor for the next page. | [optional] 
-**limit** | **int** | Entries returned. | [optional] 
+**message_type** | [**LoggingMessageType**](LoggingMessageType.md) |  | [optional] 
+**url** | **str** | The URL to post logs to. | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-2.2.2/docs/InlineResponse2003.md` & `fastly-2.3.0/docs/InlineResponse2003.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/InlineResponse2003Meta.md` & `fastly-2.3.0/docs/InlineResponse2003Meta.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Invitation.md` & `fastly-2.3.0/docs/Invitation.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/InvitationData.md` & `fastly-2.3.0/docs/InvitationData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/InvitationDataAttributes.md` & `fastly-2.3.0/docs/InvitationDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/InvitationResponse.md` & `fastly-2.3.0/docs/InvitationResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/InvitationResponseAllOf.md` & `fastly-2.3.0/docs/InvitationResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/InvitationResponseData.md` & `fastly-2.3.0/docs/InvitationResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/InvitationResponseDataAllOf.md` & `fastly-2.3.0/docs/InvitationResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/InvitationsApi.md` & `fastly-2.3.0/docs/InvitationsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/InvitationsResponse.md` & `fastly-2.3.0/docs/InvitationsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/InvitationsResponseAllOf.md` & `fastly-2.3.0/docs/InvitationsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/KvStoreApi.md` & `fastly-2.3.0/docs/KvStoreApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/KvStoreItemApi.md` & `fastly-2.3.0/docs/KvStoreItemApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingAddressAndPort.md` & `fastly-2.3.0/docs/LoggingAddressAndPort.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingAzureblob.md` & `fastly-2.3.0/docs/LoggingAzureblob.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingAzureblobAllOf.md` & `fastly-2.3.0/docs/LoggingAzureblobAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingAzureblobApi.md` & `fastly-2.3.0/docs/LoggingAzureblobApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingAzureblobResponse.md` & `fastly-2.3.0/docs/LoggingAzureblobResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingBigquery.md` & `fastly-2.3.0/docs/LoggingBigquery.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingBigqueryAllOf.md` & `fastly-2.3.0/docs/LoggingBigqueryAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingBigqueryApi.md` & `fastly-2.3.0/docs/LoggingBigqueryApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingBigqueryResponse.md` & `fastly-2.3.0/docs/LoggingBigqueryResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingCloudfiles.md` & `fastly-2.3.0/docs/LoggingCloudfiles.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingCloudfilesAllOf.md` & `fastly-2.3.0/docs/LoggingCloudfilesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingCloudfilesApi.md` & `fastly-2.3.0/docs/LoggingCloudfilesApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingCloudfilesResponse.md` & `fastly-2.3.0/docs/LoggingCloudfilesResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingCommon.md` & `fastly-2.3.0/docs/LoggingCommon.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingDatadog.md` & `fastly-2.3.0/docs/LoggingDatadog.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingDatadogAllOf.md` & `fastly-2.3.0/docs/LoggingDatadogAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingDatadogApi.md` & `fastly-2.3.0/docs/LoggingDatadogApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingDatadogResponse.md` & `fastly-2.3.0/docs/LoggingDatadogResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingDigitalocean.md` & `fastly-2.3.0/docs/LoggingDigitalocean.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingDigitaloceanAllOf.md` & `fastly-2.3.0/docs/LoggingDigitaloceanAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingDigitaloceanApi.md` & `fastly-2.3.0/docs/LoggingDigitaloceanApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingDigitaloceanResponse.md` & `fastly-2.3.0/docs/LoggingDigitaloceanResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingElasticsearch.md` & `fastly-2.3.0/docs/LoggingElasticsearch.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingElasticsearchAllOf.md` & `fastly-2.3.0/docs/LoggingElasticsearchAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingElasticsearchApi.md` & `fastly-2.3.0/docs/LoggingElasticsearchApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingElasticsearchResponse.md` & `fastly-2.3.0/docs/LoggingElasticsearchResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingFormatVersion.md` & `fastly-2.3.0/docs/LoggingFormatVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingFtp.md` & `fastly-2.3.0/docs/LoggingFtp.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingFtpAllOf.md` & `fastly-2.3.0/docs/LoggingFtpAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingFtpApi.md` & `fastly-2.3.0/docs/LoggingFtpApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingFtpResponse.md` & `fastly-2.3.0/docs/LoggingFtpResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingGcs.md` & `fastly-2.3.0/docs/LoggingGcs.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingGcsAllOf.md` & `fastly-2.3.0/docs/LoggingGcsAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingGcsApi.md` & `fastly-2.3.0/docs/LoggingGcsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingGcsCommon.md` & `fastly-2.3.0/docs/LoggingGcsCommon.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingGcsResponse.md` & `fastly-2.3.0/docs/LoggingGcsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingGenericCommon.md` & `fastly-2.3.0/docs/LoggingGenericCommon.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingGooglePubsub.md` & `fastly-2.3.0/docs/LoggingGooglePubsub.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingGooglePubsubAllOf.md` & `fastly-2.3.0/docs/LoggingGooglePubsubAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingGooglePubsubResponse.md` & `fastly-2.3.0/docs/LoggingGooglePubsubResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingHeroku.md` & `fastly-2.3.0/docs/LoggingHeroku.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingHerokuAllOf.md` & `fastly-2.3.0/docs/LoggingHerokuAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingHerokuApi.md` & `fastly-2.3.0/docs/LoggingHerokuApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingHerokuResponse.md` & `fastly-2.3.0/docs/LoggingHerokuResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingHoneycomb.md` & `fastly-2.3.0/docs/LoggingHoneycomb.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingHoneycombAllOf.md` & `fastly-2.3.0/docs/LoggingHoneycombAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingHoneycombApi.md` & `fastly-2.3.0/docs/LoggingHoneycombApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingHoneycombResponse.md` & `fastly-2.3.0/docs/LoggingHoneycombResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingHttps.md` & `fastly-2.3.0/docs/LoggingHttps.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingHttpsAllOf.md` & `fastly-2.3.0/docs/LoggingHttpsAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingHttpsApi.md` & `fastly-2.3.0/docs/LoggingHttpsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingHttpsResponse.md` & `fastly-2.3.0/docs/LoggingHttpsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingKafka.md` & `fastly-2.3.0/docs/LoggingKafka.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingKafkaAllOf.md` & `fastly-2.3.0/docs/LoggingKafkaAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingKafkaApi.md` & `fastly-2.3.0/docs/LoggingKafkaApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingKafkaResponse.md` & `fastly-2.3.0/docs/LoggingKafkaResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingKinesis.md` & `fastly-2.3.0/docs/LoggingKinesis.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingKinesisApi.md` & `fastly-2.3.0/docs/LoggingKinesisApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingKinesisResponse.md` & `fastly-2.3.0/docs/LoggingKinesisResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingLogentries.md` & `fastly-2.3.0/docs/LoggingLogentries.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingLogentriesAllOf.md` & `fastly-2.3.0/docs/LoggingLogentriesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingLogentriesApi.md` & `fastly-2.3.0/docs/LoggingLogentriesApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingLogentriesResponse.md` & `fastly-2.3.0/docs/LoggingLogentriesResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingLoggly.md` & `fastly-2.3.0/docs/LoggingLoggly.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingLogglyAllOf.md` & `fastly-2.3.0/docs/LoggingLogglyAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingLogglyApi.md` & `fastly-2.3.0/docs/LoggingLogglyApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingLogglyResponse.md` & `fastly-2.3.0/docs/LoggingLogglyResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingLogshuttle.md` & `fastly-2.3.0/docs/LoggingLogshuttle.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingLogshuttleAllOf.md` & `fastly-2.3.0/docs/LoggingLogshuttleAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingLogshuttleApi.md` & `fastly-2.3.0/docs/LoggingLogshuttleApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingLogshuttleResponse.md` & `fastly-2.3.0/docs/LoggingLogshuttleResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingNewrelic.md` & `fastly-2.3.0/docs/LoggingNewrelic.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingNewrelicAllOf.md` & `fastly-2.3.0/docs/LoggingNewrelicAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingNewrelicApi.md` & `fastly-2.3.0/docs/LoggingNewrelicApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingNewrelicResponse.md` & `fastly-2.3.0/docs/LoggingNewrelicResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingOpenstack.md` & `fastly-2.3.0/docs/LoggingOpenstack.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingOpenstackAllOf.md` & `fastly-2.3.0/docs/LoggingOpenstackAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingOpenstackApi.md` & `fastly-2.3.0/docs/LoggingOpenstackApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingOpenstackResponse.md` & `fastly-2.3.0/docs/LoggingOpenstackResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingPapertrail.md` & `fastly-2.3.0/docs/LoggingPapertrail.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingPapertrailApi.md` & `fastly-2.3.0/docs/LoggingPapertrailApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingPapertrailResponse.md` & `fastly-2.3.0/docs/LoggingPapertrailResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingPlacement.md` & `fastly-2.3.0/docs/LoggingPlacement.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingPubsubApi.md` & `fastly-2.3.0/docs/LoggingPubsubApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingRequestCapsCommon.md` & `fastly-2.3.0/docs/LoggingRequestCapsCommon.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingS3.md` & `fastly-2.3.0/docs/LoggingS3.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingS3AllOf.md` & `fastly-2.3.0/docs/LoggingS3AllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingS3Api.md` & `fastly-2.3.0/docs/LoggingS3Api.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingS3Response.md` & `fastly-2.3.0/docs/LoggingS3Response.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingScalyr.md` & `fastly-2.3.0/docs/LoggingScalyr.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingScalyrAllOf.md` & `fastly-2.3.0/docs/LoggingScalyrAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingScalyrApi.md` & `fastly-2.3.0/docs/LoggingScalyrApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingScalyrResponse.md` & `fastly-2.3.0/docs/LoggingScalyrResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingSftp.md` & `fastly-2.3.0/docs/LoggingSftp.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingSftpAllOf.md` & `fastly-2.3.0/docs/LoggingSftpAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingSftpApi.md` & `fastly-2.3.0/docs/LoggingSftpApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingSftpResponse.md` & `fastly-2.3.0/docs/LoggingSftpResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingSplunk.md` & `fastly-2.3.0/docs/LoggingSplunk.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingSplunkAllOf.md` & `fastly-2.3.0/docs/LoggingSplunkAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingSplunkApi.md` & `fastly-2.3.0/docs/LoggingSplunkApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingSplunkResponse.md` & `fastly-2.3.0/docs/LoggingSplunkResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingSumologic.md` & `fastly-2.3.0/docs/LoggingSumologic.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingSumologicAllOf.md` & `fastly-2.3.0/docs/RelationshipMemberWafFirewall.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# LoggingSumologicAllOf
+# RelationshipMemberWafFirewall
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**message_type** | [**LoggingMessageType**](LoggingMessageType.md) |  | [optional] 
-**url** | **str** | The URL to post logs to. | [optional] 
+**type** | [**TypeWafFirewall**](TypeWafFirewall.md) |  | [optional] 
+**id** | **str** |  | [optional] [readonly] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-2.2.2/docs/LoggingSumologicApi.md` & `fastly-2.3.0/docs/LoggingSumologicApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingSumologicResponse.md` & `fastly-2.3.0/docs/LoggingSumologicResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingSyslog.md` & `fastly-2.3.0/docs/LoggingSyslog.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingSyslogAllOf.md` & `fastly-2.3.0/docs/LoggingSyslogAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingSyslogApi.md` & `fastly-2.3.0/docs/LoggingSyslogApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingSyslogResponse.md` & `fastly-2.3.0/docs/LoggingSyslogResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/LoggingTlsCommon.md` & `fastly-2.3.0/docs/LoggingTlsCommon.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/MutualAuthentication.md` & `fastly-2.3.0/docs/MutualAuthentication.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/MutualAuthenticationApi.md` & `fastly-2.3.0/docs/MutualAuthenticationApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/MutualAuthenticationData.md` & `fastly-2.3.0/docs/MutualAuthenticationData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/MutualAuthenticationDataAttributes.md` & `fastly-2.3.0/docs/MutualAuthenticationDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/MutualAuthenticationResponse.md` & `fastly-2.3.0/docs/MutualAuthenticationResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/MutualAuthenticationResponseAttributes.md` & `fastly-2.3.0/docs/MutualAuthenticationResponseAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/MutualAuthenticationResponseAttributesAllOf.md` & `fastly-2.3.0/docs/MutualAuthenticationResponseAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/MutualAuthenticationResponseData.md` & `fastly-2.3.0/docs/MutualAuthenticationResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/MutualAuthenticationResponseDataAllOf.md` & `fastly-2.3.0/docs/MutualAuthenticationResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/MutualAuthenticationsResponse.md` & `fastly-2.3.0/docs/MutualAuthenticationsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/MutualAuthenticationsResponseAllOf.md` & `fastly-2.3.0/docs/MutualAuthenticationsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Package.md` & `fastly-2.3.0/docs/Package.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/PackageApi.md` & `fastly-2.3.0/docs/PackageApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/PackageMetadata.md` & `fastly-2.3.0/docs/PackageMetadata.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/PackageResponse.md` & `fastly-2.3.0/docs/PackageResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/PackageResponseAllOf.md` & `fastly-2.3.0/docs/PackageResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Pagination.md` & `fastly-2.3.0/docs/Pagination.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/PaginationLinks.md` & `fastly-2.3.0/docs/PaginationLinks.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/PaginationMeta.md` & `fastly-2.3.0/docs/PaginationMeta.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Permission.md` & `fastly-2.3.0/docs/Permission.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Pool.md` & `fastly-2.3.0/docs/Pool.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/PoolAllOf.md` & `fastly-2.3.0/docs/PoolAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/PoolApi.md` & `fastly-2.3.0/docs/PoolApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/PoolResponse.md` & `fastly-2.3.0/docs/PoolResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Pop.md` & `fastly-2.3.0/docs/Pop.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/PopApi.md` & `fastly-2.3.0/docs/PopApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/PopCoordinates.md` & `fastly-2.3.0/docs/PopCoordinates.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/PublicIpList.md` & `fastly-2.3.0/docs/PublicIpList.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/PublicIpListApi.md` & `fastly-2.3.0/docs/PublicIpListApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/PublishApi.md` & `fastly-2.3.0/docs/PublishApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/PublishItem.md` & `fastly-2.3.0/docs/PublishItem.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/PublishItemFormats.md` & `fastly-2.3.0/docs/PublishItemFormats.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/PublishRequest.md` & `fastly-2.3.0/docs/PublishRequest.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/PurgeApi.md` & `fastly-2.3.0/docs/PurgeApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/PurgeKeys.md` & `fastly-2.3.0/docs/PurgeKeys.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/PurgeResponse.md` & `fastly-2.3.0/docs/PurgeResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RateLimiter.md` & `fastly-2.3.0/docs/RateLimiter.md`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 **uri_dictionary_name** | **str, none_type** | The name of an Edge Dictionary containing URIs as keys. If not defined or `null`, all origin URIs will be rate limited. | [optional] 
 **http_methods** | **[str]** | Array of HTTP methods to apply rate limiting to. | [optional] 
 **rps_limit** | **int** | Upper limit of requests per second allowed by the rate limiter. | [optional] 
 **window_size** | **int** | Number of seconds during which the RPS limit must be exceeded in order to trigger a violation. | [optional] 
 **client_key** | **[str]** | Array of VCL variables used to generate a counter key to identify a client. Example variables include `req.http.Fastly-Client-IP`, `req.http.User-Agent`, or a custom header like `req.http.API-Key`. | [optional] 
 **penalty_box_duration** | **int** | Length of time in minutes that the rate limiter is in effect after the initial violation is detected. | [optional] 
 **action** | **str** | The action to take when a rate limiter violation is detected. | [optional] 
-**response** | [**RateLimiterResponse1**](RateLimiterResponse1.md) |  | [optional] 
+**response** | **{str: (str,)}, none_type** | Custom response to be sent when the rate limit is exceeded. Required if `action` is `response`. | [optional] 
 **response_object_name** | **str, none_type** | Name of existing response object. Required if `action` is `response_object`. Note that the rate limiter response is only updated to reflect the response object content when saving the rate limiter configuration. | [optional] 
 **logger_type** | **str** | Name of the type of logging endpoint to be used when action is `log_only`. The logging endpoint type is used to determine the appropriate log format to use when emitting log entries. | [optional] 
 **feature_revision** | **int** | Revision number of the rate limiting feature implementation. Defaults to the most recent revision. | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-2.2.2/docs/RateLimiterApi.md` & `fastly-2.3.0/docs/ResponseObjectApi.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# fastly.RateLimiterApi
+# fastly.ResponseObjectApi
 
 All URIs are relative to *https://api.fastly.com*
 
 Method | HTTP request | Description
 ------------- | ------------- | -------------
-[**delete_rate_limiter**](RateLimiterApi.md#delete_rate_limiter) | **DELETE** /rate-limiters/{rate_limiter_id} | Delete a rate limiter
-[**get_rate_limiter**](RateLimiterApi.md#get_rate_limiter) | **GET** /rate-limiters/{rate_limiter_id} | Get a rate limiter
-[**list_rate_limiters**](RateLimiterApi.md#list_rate_limiters) | **GET** /service/{service_id}/version/{version_id}/rate-limiters | List rate limiters
+[**delete_response_object**](ResponseObjectApi.md#delete_response_object) | **DELETE** /service/{service_id}/version/{version_id}/response_object/{response_object_name} | Delete a Response Object
+[**get_response_object**](ResponseObjectApi.md#get_response_object) | **GET** /service/{service_id}/version/{version_id}/response_object/{response_object_name} | Get a Response object
+[**list_response_objects**](ResponseObjectApi.md#list_response_objects) | **GET** /service/{service_id}/version/{version_id}/response_object | List Response objects
 
 
-# **delete_rate_limiter**
-> InlineResponse200 delete_rate_limiter(rate_limiter_id)
+# **delete_response_object**
+> InlineResponse200 delete_response_object(service_id, version_id, response_object_name)
 
-Delete a rate limiter
+Delete a Response Object
 
-Delete a rate limiter by its ID.
+Deletes the specified Response Object.
 
 ### Example
 
 * Api Key Authentication (token):
 
 ```python
 import time
 import fastly
-from fastly.api import rate_limiter_api
+from fastly.api import response_object_api
 from fastly.model.inline_response200 import InlineResponse200
 from pprint import pprint
 # Defining the host is optional and defaults to https://api.fastly.com
 # See configuration.py for a list of all supported configuration parameters.
 configuration = fastly.Configuration(
     host = "https://api.fastly.com"
 )
@@ -42,32 +42,36 @@
 
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['token'] = 'Bearer'
 
 # Enter a context with an instance of the API client
 with fastly.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = rate_limiter_api.RateLimiterApi(api_client)
-    rate_limiter_id = "s7aqgcJjqqKhwiTRMaP11" # str | Alphanumeric string identifying the rate limiter.
+    api_instance = response_object_api.ResponseObjectApi(api_client)
+    service_id = "SU1Z0isxPaozGVKXdv0eY" # str | Alphanumeric string identifying the service.
+    version_id = 1 # int | Integer identifying a service version.
+    response_object_name = "test-response" # str | Name for the request settings.
 
     # example passing only required values which don't have defaults set
     try:
-        # Delete a rate limiter
-        api_response = api_instance.delete_rate_limiter(rate_limiter_id)
+        # Delete a Response Object
+        api_response = api_instance.delete_response_object(service_id, version_id, response_object_name)
         pprint(api_response)
     except fastly.ApiException as e:
-        print("Exception when calling RateLimiterApi->delete_rate_limiter: %s\n" % e)
+        print("Exception when calling ResponseObjectApi->delete_response_object: %s\n" % e)
 ```
 
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
- **rate_limiter_id** | **str**| Alphanumeric string identifying the rate limiter. |
+ **service_id** | **str**| Alphanumeric string identifying the service. |
+ **version_id** | **int**| Integer identifying a service version. |
+ **response_object_name** | **str**| Name for the request settings. |
 
 ### Return type
 
 [**InlineResponse200**](InlineResponse200.md)
 
 ### Authorization
 
@@ -83,30 +87,30 @@
 
 | Status code | Description | Response headers |
 |-------------|-------------|------------------|
 **200** | OK |  -  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
-# **get_rate_limiter**
-> RateLimiterResponse get_rate_limiter(rate_limiter_id)
+# **get_response_object**
+> ResponseObjectResponse get_response_object(service_id, version_id, response_object_name)
 
-Get a rate limiter
+Get a Response object
 
-Get a rate limiter by its ID.
+Gets the specified Response Object.
 
 ### Example
 
 * Api Key Authentication (token):
 
 ```python
 import time
 import fastly
-from fastly.api import rate_limiter_api
-from fastly.model.rate_limiter_response import RateLimiterResponse
+from fastly.api import response_object_api
+from fastly.model.response_object_response import ResponseObjectResponse
 from pprint import pprint
 # Defining the host is optional and defaults to https://api.fastly.com
 # See configuration.py for a list of all supported configuration parameters.
 configuration = fastly.Configuration(
     host = "https://api.fastly.com"
 )
 
@@ -120,36 +124,40 @@
 
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['token'] = 'Bearer'
 
 # Enter a context with an instance of the API client
 with fastly.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = rate_limiter_api.RateLimiterApi(api_client)
-    rate_limiter_id = "s7aqgcJjqqKhwiTRMaP11" # str | Alphanumeric string identifying the rate limiter.
+    api_instance = response_object_api.ResponseObjectApi(api_client)
+    service_id = "SU1Z0isxPaozGVKXdv0eY" # str | Alphanumeric string identifying the service.
+    version_id = 1 # int | Integer identifying a service version.
+    response_object_name = "test-response" # str | Name for the request settings.
 
     # example passing only required values which don't have defaults set
     try:
-        # Get a rate limiter
-        api_response = api_instance.get_rate_limiter(rate_limiter_id)
+        # Get a Response object
+        api_response = api_instance.get_response_object(service_id, version_id, response_object_name)
         pprint(api_response)
     except fastly.ApiException as e:
-        print("Exception when calling RateLimiterApi->get_rate_limiter: %s\n" % e)
+        print("Exception when calling ResponseObjectApi->get_response_object: %s\n" % e)
 ```
 
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
- **rate_limiter_id** | **str**| Alphanumeric string identifying the rate limiter. |
+ **service_id** | **str**| Alphanumeric string identifying the service. |
+ **version_id** | **int**| Integer identifying a service version. |
+ **response_object_name** | **str**| Name for the request settings. |
 
 ### Return type
 
-[**RateLimiterResponse**](RateLimiterResponse.md)
+[**ResponseObjectResponse**](ResponseObjectResponse.md)
 
 ### Authorization
 
 [token](../README.md#token)
 
 ### HTTP request headers
 
@@ -161,30 +169,30 @@
 
 | Status code | Description | Response headers |
 |-------------|-------------|------------------|
 **200** | OK |  -  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
-# **list_rate_limiters**
-> [RateLimiterResponse] list_rate_limiters(service_id, version_id)
+# **list_response_objects**
+> [ResponseObjectResponse] list_response_objects(service_id, version_id)
 
-List rate limiters
+List Response objects
 
-List all rate limiters for a particular service and version.
+Returns all Response Objects for the specified service and version.
 
 ### Example
 
 * Api Key Authentication (token):
 
 ```python
 import time
 import fastly
-from fastly.api import rate_limiter_api
-from fastly.model.rate_limiter_response import RateLimiterResponse
+from fastly.api import response_object_api
+from fastly.model.response_object_response import ResponseObjectResponse
 from pprint import pprint
 # Defining the host is optional and defaults to https://api.fastly.com
 # See configuration.py for a list of all supported configuration parameters.
 configuration = fastly.Configuration(
     host = "https://api.fastly.com"
 )
 
@@ -198,38 +206,38 @@
 
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['token'] = 'Bearer'
 
 # Enter a context with an instance of the API client
 with fastly.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = rate_limiter_api.RateLimiterApi(api_client)
+    api_instance = response_object_api.ResponseObjectApi(api_client)
     service_id = "SU1Z0isxPaozGVKXdv0eY" # str | Alphanumeric string identifying the service.
     version_id = 1 # int | Integer identifying a service version.
 
     # example passing only required values which don't have defaults set
     try:
-        # List rate limiters
-        api_response = api_instance.list_rate_limiters(service_id, version_id)
+        # List Response objects
+        api_response = api_instance.list_response_objects(service_id, version_id)
         pprint(api_response)
     except fastly.ApiException as e:
-        print("Exception when calling RateLimiterApi->list_rate_limiters: %s\n" % e)
+        print("Exception when calling ResponseObjectApi->list_response_objects: %s\n" % e)
 ```
 
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **service_id** | **str**| Alphanumeric string identifying the service. |
  **version_id** | **int**| Integer identifying a service version. |
 
 ### Return type
 
-[**[RateLimiterResponse]**](RateLimiterResponse.md)
+[**[ResponseObjectResponse]**](ResponseObjectResponse.md)
 
 ### Authorization
 
 [token](../README.md#token)
 
 ### HTTP request headers
```

### Comparing `fastly-2.2.2/docs/RateLimiterResponse.md` & `fastly-2.3.0/docs/RateLimiterResponse.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 **uri_dictionary_name** | **str, none_type** | The name of an Edge Dictionary containing URIs as keys. If not defined or `null`, all origin URIs will be rate limited. | [optional] 
 **http_methods** | **[str]** | Array of HTTP methods to apply rate limiting to. | [optional] 
 **rps_limit** | **int** | Upper limit of requests per second allowed by the rate limiter. | [optional] 
 **window_size** | **int** | Number of seconds during which the RPS limit must be exceeded in order to trigger a violation. | [optional] 
 **client_key** | **[str]** | Array of VCL variables used to generate a counter key to identify a client. Example variables include `req.http.Fastly-Client-IP`, `req.http.User-Agent`, or a custom header like `req.http.API-Key`. | [optional] 
 **penalty_box_duration** | **int** | Length of time in minutes that the rate limiter is in effect after the initial violation is detected. | [optional] 
 **action** | **str** | The action to take when a rate limiter violation is detected. | [optional] 
-**response** | [**RateLimiterResponse1**](RateLimiterResponse1.md) |  | [optional] 
+**response** | **{str: (str,)}, none_type** | Custom response to be sent when the rate limit is exceeded. Required if `action` is `response`. | [optional] 
 **response_object_name** | **str, none_type** | Name of existing response object. Required if `action` is `response_object`. Note that the rate limiter response is only updated to reflect the response object content when saving the rate limiter configuration. | [optional] 
 **logger_type** | **str** | Name of the type of logging endpoint to be used when action is `log_only`. The logging endpoint type is used to determine the appropriate log format to use when emitting log entries. | [optional] 
 **feature_revision** | **int** | Revision number of the rate limiting feature implementation. Defaults to the most recent revision. | [optional] 
 **service_id** | **str** |  | [optional] [readonly] 
 **version** | **int** |  | [optional] [readonly] 
 **created_at** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly] 
 **deleted_at** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly]
```

### Comparing `fastly-2.2.2/docs/RateLimiterResponse1.md` & `fastly-2.3.0/docs/Service.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-# RateLimiterResponse1
+# Service
 
-Custom response to be sent when the rate limit is exceeded. Required if `action` is `response`.
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**status** | **int** | HTTP status code for custom limit enforcement response. | [optional] 
-**content_type** | **str** | MIME type for custom limit enforcement response. | [optional] 
-**content** | **str** | Response body for custom limit enforcement response. | [optional] 
+**comment** | **str, none_type** | A freeform descriptive note. | [optional] 
+**name** | **str** | The name of the service. | [optional] 
+**customer_id** | **str** | Alphanumeric string identifying the customer. | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-2.2.2/docs/RateLimiterResponseAllOf.md` & `fastly-2.3.0/docs/RateLimiterResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Realtime.md` & `fastly-2.3.0/docs/Realtime.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RealtimeApi.md` & `fastly-2.3.0/docs/RealtimeApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RealtimeEntry.md` & `fastly-2.3.0/docs/RealtimeEntry.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RealtimeMeasurements.md` & `fastly-2.3.0/docs/RealtimeMeasurements.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipCommonName.md` & `fastly-2.3.0/docs/RelationshipCommonName.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipCustomer.md` & `fastly-2.3.0/docs/RelationshipCustomer.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipCustomerCustomer.md` & `fastly-2.3.0/docs/RelationshipCustomerCustomer.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipMemberCustomer.md` & `fastly-2.3.0/docs/RelationshipMemberCustomer.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipMemberMutualAuthentication.md` & `fastly-2.3.0/docs/RelationshipMemberMutualAuthentication.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipMemberService.md` & `fastly-2.3.0/docs/RelationshipMemberService.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipMemberServiceInvitation.md` & `fastly-2.3.0/docs/RelationshipMemberServiceInvitation.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipMemberTlsActivation.md` & `fastly-2.3.0/docs/RelationshipMemberTlsActivation.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipMemberTlsBulkCertificate.md` & `fastly-2.3.0/docs/RelationshipMemberTlsBulkCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipMemberTlsCertificate.md` & `fastly-2.3.0/docs/RelationshipMemberTlsCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipMemberTlsConfiguration.md` & `fastly-2.3.0/docs/RelationshipMemberTlsConfiguration.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipMemberTlsDnsRecord.md` & `fastly-2.3.0/docs/RelationshipMemberTlsDnsRecord.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipMemberTlsDomain.md` & `fastly-2.3.0/docs/RelationshipMemberTlsDomain.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipMemberTlsPrivateKey.md` & `fastly-2.3.0/docs/RelationshipMemberTlsPrivateKey.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipMemberTlsSubscription.md` & `fastly-2.3.0/docs/RelationshipMemberTlsSubscription.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipMemberWafActiveRule.md` & `fastly-2.3.0/docs/RelationshipMemberWafActiveRule.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipMemberWafFirewall.md` & `fastly-2.3.0/docs/RelationshipMemberWafRule.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# RelationshipMemberWafFirewall
+# RelationshipMemberWafRule
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**type** | [**TypeWafFirewall**](TypeWafFirewall.md) |  | [optional] 
+**type** | [**TypeWafRule**](TypeWafRule.md) |  | [optional] 
 **id** | **str** |  | [optional] [readonly] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-2.2.2/docs/RelationshipMemberWafFirewallVersion.md` & `fastly-2.3.0/docs/RelationshipMemberWafFirewallVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipMemberWafRule.md` & `fastly-2.3.0/docs/TlsActivationResponseDataAllOf.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# RelationshipMemberWafRule
+# TlsActivationResponseDataAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**type** | [**TypeWafRule**](TypeWafRule.md) |  | [optional] 
 **id** | **str** |  | [optional] [readonly] 
+**attributes** | [**Timestamps**](Timestamps.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-2.2.2/docs/RelationshipMemberWafRuleRevision.md` & `fastly-2.3.0/docs/RelationshipMemberWafRuleRevision.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipMemberWafTag.md` & `fastly-2.3.0/docs/RelationshipMemberWafTag.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipMutualAuthentication.md` & `fastly-2.3.0/docs/RelationshipMutualAuthentication.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipMutualAuthenticationMutualAuthentication.md` & `fastly-2.3.0/docs/RelationshipMutualAuthenticationMutualAuthentication.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipMutualAuthentications.md` & `fastly-2.3.0/docs/RelationshipMutualAuthentications.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipMutualAuthenticationsMutualAuthentications.md` & `fastly-2.3.0/docs/RelationshipMutualAuthenticationsMutualAuthentications.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipService.md` & `fastly-2.3.0/docs/RelationshipService.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipServiceInvitations.md` & `fastly-2.3.0/docs/RelationshipServiceInvitations.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipServiceInvitationsCreate.md` & `fastly-2.3.0/docs/RelationshipServiceInvitationsCreate.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipServiceInvitationsCreateServiceInvitations.md` & `fastly-2.3.0/docs/RelationshipServiceInvitationsCreateServiceInvitations.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipServiceInvitationsServiceInvitations.md` & `fastly-2.3.0/docs/RelationshipServiceInvitationsServiceInvitations.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipServices.md` & `fastly-2.3.0/docs/RelationshipServices.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipServicesServices.md` & `fastly-2.3.0/docs/RelationshipServicesServices.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsActivation.md` & `fastly-2.3.0/docs/RelationshipTlsActivation.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsActivationTlsActivation.md` & `fastly-2.3.0/docs/RelationshipTlsActivationTlsActivation.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsActivations.md` & `fastly-2.3.0/docs/RelationshipTlsActivations.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsBulkCertificate.md` & `fastly-2.3.0/docs/RelationshipTlsBulkCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsBulkCertificateTlsBulkCertificate.md` & `fastly-2.3.0/docs/RelationshipTlsBulkCertificateTlsBulkCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsBulkCertificates.md` & `fastly-2.3.0/docs/RelationshipTlsBulkCertificates.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsCertificate.md` & `fastly-2.3.0/docs/RelationshipTlsCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsCertificateTlsCertificate.md` & `fastly-2.3.0/docs/RelationshipTlsCertificateTlsCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsCertificates.md` & `fastly-2.3.0/docs/RelationshipTlsCertificates.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsCertificatesTlsCertificates.md` & `fastly-2.3.0/docs/RelationshipTlsCertificatesTlsCertificates.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsConfiguration.md` & `fastly-2.3.0/docs/RelationshipTlsConfiguration.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsConfigurationForTlsSubscription.md` & `fastly-2.3.0/docs/RelationshipTlsConfigurationForTlsSubscription.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsConfigurationTlsConfiguration.md` & `fastly-2.3.0/docs/RelationshipTlsConfigurationTlsConfiguration.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsConfigurations.md` & `fastly-2.3.0/docs/RelationshipTlsConfigurations.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsConfigurationsTlsConfigurations.md` & `fastly-2.3.0/docs/RelationshipTlsConfigurationsTlsConfigurations.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsDnsRecord.md` & `fastly-2.3.0/docs/RelationshipTlsDnsRecord.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsDnsRecordDnsRecord.md` & `fastly-2.3.0/docs/RelationshipTlsDnsRecordDnsRecord.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsDnsRecords.md` & `fastly-2.3.0/docs/RelationshipTlsDnsRecords.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsDomain.md` & `fastly-2.3.0/docs/RelationshipTlsDomain.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsDomainTlsDomain.md` & `fastly-2.3.0/docs/RelationshipTlsDomainTlsDomain.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsDomains.md` & `fastly-2.3.0/docs/RelationshipTlsDomains.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsDomainsTlsDomains.md` & `fastly-2.3.0/docs/RelationshipTlsDomainsTlsDomains.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsPrivateKey.md` & `fastly-2.3.0/docs/RelationshipTlsPrivateKey.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsPrivateKeyTlsPrivateKey.md` & `fastly-2.3.0/docs/RelationshipTlsPrivateKeyTlsPrivateKey.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsPrivateKeys.md` & `fastly-2.3.0/docs/RelationshipTlsPrivateKeys.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsPrivateKeysTlsPrivateKeys.md` & `fastly-2.3.0/docs/RelationshipTlsPrivateKeysTlsPrivateKeys.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsSubscription.md` & `fastly-2.3.0/docs/RelationshipTlsSubscription.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsSubscriptionTlsSubscription.md` & `fastly-2.3.0/docs/RelationshipTlsSubscriptionTlsSubscription.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipTlsSubscriptions.md` & `fastly-2.3.0/docs/RelationshipTlsSubscriptions.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipUser.md` & `fastly-2.3.0/docs/RelationshipUser.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipUserUser.md` & `fastly-2.3.0/docs/RelationshipUserUser.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipWafActiveRules.md` & `fastly-2.3.0/docs/RelationshipWafActiveRules.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipWafActiveRulesWafActiveRules.md` & `fastly-2.3.0/docs/RelationshipWafActiveRulesWafActiveRules.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipWafFirewall.md` & `fastly-2.3.0/docs/RelationshipWafFirewall.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipWafFirewallVersion.md` & `fastly-2.3.0/docs/RelationshipWafFirewallVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipWafFirewallVersionWafFirewallVersion.md` & `fastly-2.3.0/docs/RelationshipWafFirewallVersionWafFirewallVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipWafFirewallVersions.md` & `fastly-2.3.0/docs/RelationshipWafFirewallVersions.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipWafFirewallWafFirewall.md` & `fastly-2.3.0/docs/RelationshipWafFirewallWafFirewall.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipWafRule.md` & `fastly-2.3.0/docs/RelationshipWafRule.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipWafRuleRevision.md` & `fastly-2.3.0/docs/RelationshipWafRuleRevision.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipWafRuleRevisionWafRuleRevisions.md` & `fastly-2.3.0/docs/RelationshipWafRuleRevisionWafRuleRevisions.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipWafRuleRevisions.md` & `fastly-2.3.0/docs/RelationshipWafRuleRevisions.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipWafRuleWafRule.md` & `fastly-2.3.0/docs/RelationshipWafRuleWafRule.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipWafRules.md` & `fastly-2.3.0/docs/RelationshipWafRules.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipWafTags.md` & `fastly-2.3.0/docs/RelationshipWafTags.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipWafTagsWafTags.md` & `fastly-2.3.0/docs/RelationshipWafTagsWafTags.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipsForInvitation.md` & `fastly-2.3.0/docs/RelationshipsForInvitation.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipsForMutualAuthentication.md` & `fastly-2.3.0/docs/RelationshipsForMutualAuthentication.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipsForStar.md` & `fastly-2.3.0/docs/RelationshipsForStar.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipsForTlsActivation.md` & `fastly-2.3.0/docs/RelationshipsForTlsActivation.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipsForTlsBulkCertificate.md` & `fastly-2.3.0/docs/RelationshipsForTlsBulkCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipsForTlsConfiguration.md` & `fastly-2.3.0/docs/RelationshipsForTlsConfiguration.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipsForTlsDomain.md` & `fastly-2.3.0/docs/RelationshipsForTlsDomain.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipsForTlsPrivateKey.md` & `fastly-2.3.0/docs/RelationshipsForTlsPrivateKey.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipsForTlsSubscription.md` & `fastly-2.3.0/docs/RelationshipsForTlsSubscription.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipsForWafActiveRule.md` & `fastly-2.3.0/docs/RelationshipsForWafActiveRule.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipsForWafExclusion.md` & `fastly-2.3.0/docs/RelationshipsForWafExclusion.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipsForWafFirewallVersion.md` & `fastly-2.3.0/docs/RelationshipsForWafFirewallVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RelationshipsForWafRule.md` & `fastly-2.3.0/docs/RelationshipsForWafRule.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RequestSettings.md` & `fastly-2.3.0/docs/RequestSettings.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RequestSettingsApi.md` & `fastly-2.3.0/docs/RequestSettingsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RequestSettingsResponse.md` & `fastly-2.3.0/docs/RequestSettingsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Resource.md` & `fastly-2.3.0/docs/Resource.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ResourceApi.md` & `fastly-2.3.0/docs/ResourceApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ResourceResponse.md` & `fastly-2.3.0/docs/ResourceResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ResourceResponseAllOf.md` & `fastly-2.3.0/docs/ResourceResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ResponseObject.md` & `fastly-2.3.0/docs/ResponseObject.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ResponseObjectApi.md` & `fastly-2.3.0/docs/WafRuleRevisionsApi.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-# fastly.ResponseObjectApi
+# fastly.WafRuleRevisionsApi
 
 All URIs are relative to *https://api.fastly.com*
 
 Method | HTTP request | Description
 ------------- | ------------- | -------------
-[**delete_response_object**](ResponseObjectApi.md#delete_response_object) | **DELETE** /service/{service_id}/version/{version_id}/response_object/{response_object_name} | Delete a Response Object
-[**get_response_object**](ResponseObjectApi.md#get_response_object) | **GET** /service/{service_id}/version/{version_id}/response_object/{response_object_name} | Get a Response object
-[**list_response_objects**](ResponseObjectApi.md#list_response_objects) | **GET** /service/{service_id}/version/{version_id}/response_object | List Response objects
+[**get_waf_rule_revision**](WafRuleRevisionsApi.md#get_waf_rule_revision) | **GET** /waf/rules/{waf_rule_id}/revisions/{waf_rule_revision_number} | Get a revision of a rule
+[**list_waf_rule_revisions**](WafRuleRevisionsApi.md#list_waf_rule_revisions) | **GET** /waf/rules/{waf_rule_id}/revisions | List revisions for a rule
 
 
-# **delete_response_object**
-> InlineResponse200 delete_response_object(service_id, version_id, response_object_name)
+# **get_waf_rule_revision**
+> WafRuleRevisionResponse get_waf_rule_revision(waf_rule_id, waf_rule_revision_number)
 
-Delete a Response Object
+Get a revision of a rule
 
-Deletes the specified Response Object.
+Get a specific rule revision.
 
 ### Example
 
 * Api Key Authentication (token):
 
 ```python
 import time
 import fastly
-from fastly.api import response_object_api
-from fastly.model.inline_response200 import InlineResponse200
+from fastly.api import waf_rule_revisions_api
+from fastly.model.waf_rule_revision_response import WafRuleRevisionResponse
 from pprint import pprint
 # Defining the host is optional and defaults to https://api.fastly.com
 # See configuration.py for a list of all supported configuration parameters.
 configuration = fastly.Configuration(
     host = "https://api.fastly.com"
 )
 
@@ -42,157 +41,84 @@
 
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['token'] = 'Bearer'
 
 # Enter a context with an instance of the API client
 with fastly.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = response_object_api.ResponseObjectApi(api_client)
-    service_id = "SU1Z0isxPaozGVKXdv0eY" # str | Alphanumeric string identifying the service.
-    version_id = 1 # int | Integer identifying a service version.
-    response_object_name = "test-response" # str | Name for the request settings.
+    api_instance = waf_rule_revisions_api.WafRuleRevisionsApi(api_client)
+    waf_rule_id = "3krg2uUGZzb2W9Euo4moOR" # str | Alphanumeric string identifying a WAF rule.
+    waf_rule_revision_number = 2 # int | Revision number.
+    include = "source,vcl,waf_rule" # str | Include relationships. Optional, comma-separated values. Permitted values: `waf_rule`, `vcl`, and `source`. The `vcl` and `source` relationships show the WAF VCL and corresponding ModSecurity source. These fields are blank unless the relationship is included.  (optional)
 
     # example passing only required values which don't have defaults set
     try:
-        # Delete a Response Object
-        api_response = api_instance.delete_response_object(service_id, version_id, response_object_name)
+        # Get a revision of a rule
+        api_response = api_instance.get_waf_rule_revision(waf_rule_id, waf_rule_revision_number)
         pprint(api_response)
     except fastly.ApiException as e:
-        print("Exception when calling ResponseObjectApi->delete_response_object: %s\n" % e)
-```
-
-
-### Parameters
-
-Name | Type | Description  | Notes
-------------- | ------------- | ------------- | -------------
- **service_id** | **str**| Alphanumeric string identifying the service. |
- **version_id** | **int**| Integer identifying a service version. |
- **response_object_name** | **str**| Name for the request settings. |
-
-### Return type
-
-[**InlineResponse200**](InlineResponse200.md)
-
-### Authorization
-
-[token](../README.md#token)
-
-### HTTP request headers
-
- - **Content-Type**: Not defined
- - **Accept**: application/json
-
-
-### HTTP response details
-
-| Status code | Description | Response headers |
-|-------------|-------------|------------------|
-**200** | OK |  -  |
-
-[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
-
-# **get_response_object**
-> ResponseObjectResponse get_response_object(service_id, version_id, response_object_name)
-
-Get a Response object
-
-Gets the specified Response Object.
-
-### Example
-
-* Api Key Authentication (token):
-
-```python
-import time
-import fastly
-from fastly.api import response_object_api
-from fastly.model.response_object_response import ResponseObjectResponse
-from pprint import pprint
-# Defining the host is optional and defaults to https://api.fastly.com
-# See configuration.py for a list of all supported configuration parameters.
-configuration = fastly.Configuration(
-    host = "https://api.fastly.com"
-)
-
-# The client must configure the authentication and authorization parameters
-# in accordance with the API server security policy.
-# Examples for each auth method are provided below, use the example that
-# satisfies your auth use case.
-
-# Configure API key authorization: token
-configuration.api_key['token'] = 'YOUR_API_KEY'
-
-# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
-# configuration.api_key_prefix['token'] = 'Bearer'
-
-# Enter a context with an instance of the API client
-with fastly.ApiClient(configuration) as api_client:
-    # Create an instance of the API class
-    api_instance = response_object_api.ResponseObjectApi(api_client)
-    service_id = "SU1Z0isxPaozGVKXdv0eY" # str | Alphanumeric string identifying the service.
-    version_id = 1 # int | Integer identifying a service version.
-    response_object_name = "test-response" # str | Name for the request settings.
+        print("Exception when calling WafRuleRevisionsApi->get_waf_rule_revision: %s\n" % e)
 
     # example passing only required values which don't have defaults set
+    # and optional values
     try:
-        # Get a Response object
-        api_response = api_instance.get_response_object(service_id, version_id, response_object_name)
+        # Get a revision of a rule
+        api_response = api_instance.get_waf_rule_revision(waf_rule_id, waf_rule_revision_number, include=include)
         pprint(api_response)
     except fastly.ApiException as e:
-        print("Exception when calling ResponseObjectApi->get_response_object: %s\n" % e)
+        print("Exception when calling WafRuleRevisionsApi->get_waf_rule_revision: %s\n" % e)
 ```
 
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
- **service_id** | **str**| Alphanumeric string identifying the service. |
- **version_id** | **int**| Integer identifying a service version. |
- **response_object_name** | **str**| Name for the request settings. |
+ **waf_rule_id** | **str**| Alphanumeric string identifying a WAF rule. |
+ **waf_rule_revision_number** | **int**| Revision number. |
+ **include** | **str**| Include relationships. Optional, comma-separated values. Permitted values: `waf_rule`, `vcl`, and `source`. The `vcl` and `source` relationships show the WAF VCL and corresponding ModSecurity source. These fields are blank unless the relationship is included.  | [optional]
 
 ### Return type
 
-[**ResponseObjectResponse**](ResponseObjectResponse.md)
+[**WafRuleRevisionResponse**](WafRuleRevisionResponse.md)
 
 ### Authorization
 
 [token](../README.md#token)
 
 ### HTTP request headers
 
  - **Content-Type**: Not defined
- - **Accept**: application/json
+ - **Accept**: application/vnd.api+json
 
 
 ### HTTP response details
 
 | Status code | Description | Response headers |
 |-------------|-------------|------------------|
 **200** | OK |  -  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
-# **list_response_objects**
-> [ResponseObjectResponse] list_response_objects(service_id, version_id)
+# **list_waf_rule_revisions**
+> WafRuleRevisionsResponse list_waf_rule_revisions(waf_rule_id)
 
-List Response objects
+List revisions for a rule
 
-Returns all Response Objects for the specified service and version.
+List all revisions for a specific rule. The `rule_id` provided can be the ModSecurity Rule ID or the Fastly generated rule ID.
 
 ### Example
 
 * Api Key Authentication (token):
 
 ```python
 import time
 import fastly
-from fastly.api import response_object_api
-from fastly.model.response_object_response import ResponseObjectResponse
+from fastly.api import waf_rule_revisions_api
+from fastly.model.waf_rule_revisions_response import WafRuleRevisionsResponse
 from pprint import pprint
 # Defining the host is optional and defaults to https://api.fastly.com
 # See configuration.py for a list of all supported configuration parameters.
 configuration = fastly.Configuration(
     host = "https://api.fastly.com"
 )
 
@@ -206,47 +132,60 @@
 
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['token'] = 'Bearer'
 
 # Enter a context with an instance of the API client
 with fastly.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = response_object_api.ResponseObjectApi(api_client)
-    service_id = "SU1Z0isxPaozGVKXdv0eY" # str | Alphanumeric string identifying the service.
-    version_id = 1 # int | Integer identifying a service version.
+    api_instance = waf_rule_revisions_api.WafRuleRevisionsApi(api_client)
+    waf_rule_id = "3krg2uUGZzb2W9Euo4moOR" # str | Alphanumeric string identifying a WAF rule.
+    page_number = 1 # int | Current page. (optional)
+    page_size = 20 # int | Number of records per page. (optional) if omitted the server will use the default value of 20
+    include = "waf_rule" # str | Include relationships. Optional. (optional) if omitted the server will use the default value of "waf_rule"
+
+    # example passing only required values which don't have defaults set
+    try:
+        # List revisions for a rule
+        api_response = api_instance.list_waf_rule_revisions(waf_rule_id)
+        pprint(api_response)
+    except fastly.ApiException as e:
+        print("Exception when calling WafRuleRevisionsApi->list_waf_rule_revisions: %s\n" % e)
 
     # example passing only required values which don't have defaults set
+    # and optional values
     try:
-        # List Response objects
-        api_response = api_instance.list_response_objects(service_id, version_id)
+        # List revisions for a rule
+        api_response = api_instance.list_waf_rule_revisions(waf_rule_id, page_number=page_number, page_size=page_size, include=include)
         pprint(api_response)
     except fastly.ApiException as e:
-        print("Exception when calling ResponseObjectApi->list_response_objects: %s\n" % e)
+        print("Exception when calling WafRuleRevisionsApi->list_waf_rule_revisions: %s\n" % e)
 ```
 
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
- **service_id** | **str**| Alphanumeric string identifying the service. |
- **version_id** | **int**| Integer identifying a service version. |
+ **waf_rule_id** | **str**| Alphanumeric string identifying a WAF rule. |
+ **page_number** | **int**| Current page. | [optional]
+ **page_size** | **int**| Number of records per page. | [optional] if omitted the server will use the default value of 20
+ **include** | **str**| Include relationships. Optional. | [optional] if omitted the server will use the default value of "waf_rule"
 
 ### Return type
 
-[**[ResponseObjectResponse]**](ResponseObjectResponse.md)
+[**WafRuleRevisionsResponse**](WafRuleRevisionsResponse.md)
 
 ### Authorization
 
 [token](../README.md#token)
 
 ### HTTP request headers
 
  - **Content-Type**: Not defined
- - **Accept**: application/json
+ - **Accept**: application/vnd.api+json
 
 
 ### HTTP response details
 
 | Status code | Description | Response headers |
 |-------------|-------------|------------------|
 **200** | OK |  -  |
```

### Comparing `fastly-2.2.2/docs/ResponseObjectResponse.md` & `fastly-2.3.0/docs/ResponseObjectResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Results.md` & `fastly-2.3.0/docs/Results.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/RoleUser.md` & `fastly-2.3.0/docs/RoleUser.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/SchemasContactResponse.md` & `fastly-2.3.0/docs/SchemasContactResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/SchemasSnippetResponse.md` & `fastly-2.3.0/docs/SchemasSnippetResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/SchemasUserResponse.md` & `fastly-2.3.0/docs/SchemasUserResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/SchemasVclResponse.md` & `fastly-2.3.0/docs/SchemasVclResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/SchemasVersion.md` & `fastly-2.3.0/docs/SchemasVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/SchemasVersionResponse.md` & `fastly-2.3.0/docs/SchemasVersionResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/SchemasWafFirewallVersion.md` & `fastly-2.3.0/docs/SchemasWafFirewallVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/SchemasWafFirewallVersionData.md` & `fastly-2.3.0/docs/SchemasWafFirewallVersionData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Server.md` & `fastly-2.3.0/docs/Server.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServerApi.md` & `fastly-2.3.0/docs/ServerApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServerResponse.md` & `fastly-2.3.0/docs/ServerResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServerResponseAllOf.md` & `fastly-2.3.0/docs/ServerResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Service.md` & `fastly-2.3.0/docs/WafTag.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# Service
+# WafTag
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**comment** | **str, none_type** | A freeform descriptive note. | [optional] 
-**name** | **str** | The name of the service. | [optional] 
-**customer_id** | **str** | Alphanumeric string identifying the customer. | [optional] 
+**type** | [**TypeWafTag**](TypeWafTag.md) |  | [optional] 
+**id** | **str** | Alphanumeric string identifying a WAF tag. | [optional] [readonly] 
+**attributes** | [**WafTagAttributes**](WafTagAttributes.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-2.2.2/docs/ServiceApi.md` & `fastly-2.3.0/docs/ServiceApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceAuthorization.md` & `fastly-2.3.0/docs/ServiceAuthorization.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceAuthorizationData.md` & `fastly-2.3.0/docs/ServiceAuthorizationData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceAuthorizationDataAttributes.md` & `fastly-2.3.0/docs/ServiceAuthorizationDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceAuthorizationDataRelationships.md` & `fastly-2.3.0/docs/ServiceAuthorizationDataRelationships.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceAuthorizationDataRelationshipsUser.md` & `fastly-2.3.0/docs/ServiceAuthorizationDataRelationshipsUser.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceAuthorizationDataRelationshipsUserData.md` & `fastly-2.3.0/docs/ServiceAuthorizationDataRelationshipsUserData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceAuthorizationResponse.md` & `fastly-2.3.0/docs/ServiceAuthorizationResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceAuthorizationResponseData.md` & `fastly-2.3.0/docs/ServiceAuthorizationResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceAuthorizationResponseDataAllOf.md` & `fastly-2.3.0/docs/ServiceAuthorizationResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceAuthorizationsApi.md` & `fastly-2.3.0/docs/ServiceAuthorizationsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceAuthorizationsResponse.md` & `fastly-2.3.0/docs/ServiceAuthorizationsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceAuthorizationsResponseAllOf.md` & `fastly-2.3.0/docs/ServiceAuthorizationsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceCreate.md` & `fastly-2.3.0/docs/ServiceCreate.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceCreateAllOf.md` & `fastly-2.3.0/docs/ServiceCreateAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceDetail.md` & `fastly-2.3.0/docs/ServiceDetail.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceDetailAllOf.md` & `fastly-2.3.0/docs/ServiceDetailAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceIdAndVersion.md` & `fastly-2.3.0/docs/ServiceIdAndVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceInvitation.md` & `fastly-2.3.0/docs/ServiceInvitation.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceInvitationData.md` & `fastly-2.3.0/docs/ServiceInvitationData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceInvitationDataAttributes.md` & `fastly-2.3.0/docs/ServiceInvitationDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceInvitationDataRelationships.md` & `fastly-2.3.0/docs/ServiceInvitationDataRelationships.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceInvitationResponse.md` & `fastly-2.3.0/docs/ServiceInvitationResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceInvitationResponseAllOf.md` & `fastly-2.3.0/docs/ServiceInvitationResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceInvitationResponseAllOfData.md` & `fastly-2.3.0/docs/ServiceInvitationResponseAllOfData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceListResponse.md` & `fastly-2.3.0/docs/ServiceListResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceListResponseAllOf.md` & `fastly-2.3.0/docs/ServiceListResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceResponse.md` & `fastly-2.3.0/docs/ServiceResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceResponseAllOf.md` & `fastly-2.3.0/docs/ServiceResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceVersionDetail.md` & `fastly-2.3.0/docs/ServiceVersionDetail.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ServiceVersionDetailOrNull.md` & `fastly-2.3.0/docs/ServiceVersionDetailOrNull.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Settings.md` & `fastly-2.3.0/docs/Settings.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/SettingsApi.md` & `fastly-2.3.0/docs/SettingsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/SettingsResponse.md` & `fastly-2.3.0/docs/SettingsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Snippet.md` & `fastly-2.3.0/docs/Snippet.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/SnippetApi.md` & `fastly-2.3.0/docs/SnippetApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/SnippetResponse.md` & `fastly-2.3.0/docs/SnippetResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/SnippetResponseAllOf.md` & `fastly-2.3.0/docs/SnippetResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/StarApi.md` & `fastly-2.3.0/docs/StarApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/StarData.md` & `fastly-2.3.0/docs/StarData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/StarResponse.md` & `fastly-2.3.0/docs/StarResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/StarResponseAllOf.md` & `fastly-2.3.0/docs/StarResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Stats.md` & `fastly-2.3.0/docs/Stats.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/StatsApi.md` & `fastly-2.3.0/docs/StatsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Store.md` & `fastly-2.3.0/docs/Store.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/StoreResponse.md` & `fastly-2.3.0/docs/StoreResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Timestamps.md` & `fastly-2.3.0/docs/Timestamps.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TimestampsNoDelete.md` & `fastly-2.3.0/docs/TimestampsNoDelete.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsActivation.md` & `fastly-2.3.0/docs/TlsActivation.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsActivationData.md` & `fastly-2.3.0/docs/TlsActivationData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsActivationResponse.md` & `fastly-2.3.0/docs/TlsActivationResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsActivationResponseData.md` & `fastly-2.3.0/docs/TlsActivationResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsActivationResponseDataAllOf.md` & `fastly-2.3.0/docs/TlsActivationsResponseAllOf.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# TlsActivationResponseDataAllOf
+# TlsActivationsResponseAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**id** | **str** |  | [optional] [readonly] 
-**attributes** | [**Timestamps**](Timestamps.md) |  | [optional] 
+**data** | [**[TlsActivationResponseData]**](TlsActivationResponseData.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-2.2.2/docs/TlsActivationsApi.md` & `fastly-2.3.0/docs/TlsActivationsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsActivationsResponse.md` & `fastly-2.3.0/docs/TlsActivationsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsActivationsResponseAllOf.md` & `fastly-2.3.0/docs/TlsCertificatesResponseAllOf.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# TlsActivationsResponseAllOf
+# TlsCertificatesResponseAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**[TlsActivationResponseData]**](TlsActivationResponseData.md) |  | [optional] 
+**data** | [**[TlsCertificateResponseData]**](TlsCertificateResponseData.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-2.2.2/docs/TlsBulkCertificate.md` & `fastly-2.3.0/docs/TlsBulkCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsBulkCertificateData.md` & `fastly-2.3.0/docs/TlsBulkCertificateData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsBulkCertificateDataAttributes.md` & `fastly-2.3.0/docs/TlsBulkCertificateDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsBulkCertificateResponse.md` & `fastly-2.3.0/docs/TlsBulkCertificateResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsBulkCertificateResponseAttributes.md` & `fastly-2.3.0/docs/TlsBulkCertificateResponseAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsBulkCertificateResponseAttributesAllOf.md` & `fastly-2.3.0/docs/TlsBulkCertificateResponseAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsBulkCertificateResponseData.md` & `fastly-2.3.0/docs/TlsBulkCertificateResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsBulkCertificateResponseDataAllOf.md` & `fastly-2.3.0/docs/TlsBulkCertificateResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsBulkCertificatesApi.md` & `fastly-2.3.0/docs/TlsBulkCertificatesApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsBulkCertificatesResponse.md` & `fastly-2.3.0/docs/TlsBulkCertificatesResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsBulkCertificatesResponseAllOf.md` & `fastly-2.3.0/docs/TlsBulkCertificatesResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsCertificate.md` & `fastly-2.3.0/docs/TlsCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsCertificateData.md` & `fastly-2.3.0/docs/TlsCertificateData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsCertificateDataAttributes.md` & `fastly-2.3.0/docs/TlsCertificateDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsCertificateResponse.md` & `fastly-2.3.0/docs/TlsCertificateResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsCertificateResponseAttributes.md` & `fastly-2.3.0/docs/TlsCertificateResponseAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsCertificateResponseAttributesAllOf.md` & `fastly-2.3.0/docs/TlsCertificateResponseAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsCertificateResponseData.md` & `fastly-2.3.0/docs/TlsCertificateResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsCertificateResponseDataAllOf.md` & `fastly-2.3.0/docs/TlsCertificateResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsCertificatesApi.md` & `fastly-2.3.0/docs/TlsCertificatesApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsCertificatesResponse.md` & `fastly-2.3.0/docs/TlsCertificatesResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsCertificatesResponseAllOf.md` & `fastly-2.3.0/docs/TlsPrivateKeysResponseAllOf.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# TlsCertificatesResponseAllOf
+# TlsPrivateKeysResponseAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**[TlsCertificateResponseData]**](TlsCertificateResponseData.md) |  | [optional] 
+**data** | [**[TlsPrivateKeyResponseData]**](TlsPrivateKeyResponseData.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-2.2.2/docs/TlsCommon.md` & `fastly-2.3.0/docs/TlsCommon.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsConfiguration.md` & `fastly-2.3.0/docs/TlsConfiguration.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsConfigurationData.md` & `fastly-2.3.0/docs/TlsConfigurationData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsConfigurationDataAttributes.md` & `fastly-2.3.0/docs/TlsConfigurationDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsConfigurationResponse.md` & `fastly-2.3.0/docs/TlsConfigurationResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsConfigurationResponseAttributes.md` & `fastly-2.3.0/docs/TlsConfigurationResponseAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsConfigurationResponseAttributesAllOf.md` & `fastly-2.3.0/docs/TlsConfigurationResponseAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsConfigurationResponseData.md` & `fastly-2.3.0/docs/TlsConfigurationResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsConfigurationResponseDataAllOf.md` & `fastly-2.3.0/docs/TlsConfigurationResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsConfigurationsApi.md` & `fastly-2.3.0/docs/TlsConfigurationsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsConfigurationsResponse.md` & `fastly-2.3.0/docs/TlsConfigurationsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsConfigurationsResponseAllOf.md` & `fastly-2.3.0/docs/TlsConfigurationsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsDnsRecord.md` & `fastly-2.3.0/docs/TlsDnsRecord.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsDomainData.md` & `fastly-2.3.0/docs/TlsDomainData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsDomainsApi.md` & `fastly-2.3.0/docs/TlsDomainsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsDomainsResponse.md` & `fastly-2.3.0/docs/TlsDomainsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsDomainsResponseAllOf.md` & `fastly-2.3.0/docs/TlsDomainsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsPrivateKey.md` & `fastly-2.3.0/docs/TlsPrivateKey.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsPrivateKeyData.md` & `fastly-2.3.0/docs/TlsPrivateKeyData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsPrivateKeyDataAttributes.md` & `fastly-2.3.0/docs/TlsPrivateKeyDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsPrivateKeyResponse.md` & `fastly-2.3.0/docs/TlsPrivateKeyResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsPrivateKeyResponseAttributes.md` & `fastly-2.3.0/docs/TlsPrivateKeyResponseAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsPrivateKeyResponseAttributesAllOf.md` & `fastly-2.3.0/docs/TlsPrivateKeyResponseAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsPrivateKeyResponseData.md` & `fastly-2.3.0/docs/TlsPrivateKeyResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsPrivateKeysApi.md` & `fastly-2.3.0/docs/TlsPrivateKeysApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsPrivateKeysResponse.md` & `fastly-2.3.0/docs/TlsPrivateKeysResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsPrivateKeysResponseAllOf.md` & `fastly-2.3.0/docs/WafTagsResponseAllOf.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# TlsPrivateKeysResponseAllOf
+# WafTagsResponseAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**[TlsPrivateKeyResponseData]**](TlsPrivateKeyResponseData.md) |  | [optional] 
+**data** | [**[WafTagsResponseDataItem]**](WafTagsResponseDataItem.md) |  | [optional] 
+**included** | [**[WafRule]**](WafRule.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-2.2.2/docs/TlsSubscription.md` & `fastly-2.3.0/docs/TlsSubscription.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsSubscriptionData.md` & `fastly-2.3.0/docs/TlsSubscriptionData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsSubscriptionDataAttributes.md` & `fastly-2.3.0/docs/TlsSubscriptionDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsSubscriptionResponse.md` & `fastly-2.3.0/docs/TlsSubscriptionResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsSubscriptionResponseAttributes.md` & `fastly-2.3.0/docs/TlsSubscriptionResponseAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsSubscriptionResponseAttributesAllOf.md` & `fastly-2.3.0/docs/TlsSubscriptionResponseAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsSubscriptionResponseData.md` & `fastly-2.3.0/docs/TlsSubscriptionResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsSubscriptionResponseDataAllOf.md` & `fastly-2.3.0/docs/TlsSubscriptionResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsSubscriptionsApi.md` & `fastly-2.3.0/docs/TlsSubscriptionsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsSubscriptionsResponse.md` & `fastly-2.3.0/docs/TlsSubscriptionsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TlsSubscriptionsResponseAllOf.md` & `fastly-2.3.0/docs/TlsSubscriptionsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Token.md` & `fastly-2.3.0/docs/Token.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TokenCreatedResponse.md` & `fastly-2.3.0/docs/TokenCreatedResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TokenCreatedResponseAllOf.md` & `fastly-2.3.0/docs/TokenCreatedResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TokenResponse.md` & `fastly-2.3.0/docs/TokenResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TokenResponseAllOf.md` & `fastly-2.3.0/docs/TokenResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/TokensApi.md` & `fastly-2.3.0/docs/TokensApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/UpdateBillingAddressRequest.md` & `fastly-2.3.0/docs/UpdateBillingAddressRequest.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/UpdateBillingAddressRequestData.md` & `fastly-2.3.0/docs/UpdateBillingAddressRequestData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/User.md` & `fastly-2.3.0/docs/User.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/UserApi.md` & `fastly-2.3.0/docs/UserApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/UserResponse.md` & `fastly-2.3.0/docs/UserResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/UserResponseAllOf.md` & `fastly-2.3.0/docs/UserResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ValidatorResult.md` & `fastly-2.3.0/docs/ValidatorResult.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/ValidatorResultMessages.md` & `fastly-2.3.0/docs/ValidatorResultMessages.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Vcl.md` & `fastly-2.3.0/docs/Vcl.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/VclApi.md` & `fastly-2.3.0/docs/VclApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/VclDiff.md` & `fastly-2.3.0/docs/VclDiff.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/VclDiffApi.md` & `fastly-2.3.0/docs/VclDiffApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/VclResponse.md` & `fastly-2.3.0/docs/VclResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/Version.md` & `fastly-2.3.0/docs/Version.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/VersionApi.md` & `fastly-2.3.0/docs/VersionApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/VersionCreateResponse.md` & `fastly-2.3.0/docs/VersionCreateResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/VersionDetail.md` & `fastly-2.3.0/docs/VersionDetail.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/VersionDetailSettings.md` & `fastly-2.3.0/docs/VersionDetailSettings.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/VersionResponse.md` & `fastly-2.3.0/docs/VersionResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/VersionResponseAllOf.md` & `fastly-2.3.0/docs/VersionResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafActiveRule.md` & `fastly-2.3.0/docs/WafActiveRule.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafActiveRuleCreationResponse.md` & `fastly-2.3.0/docs/WafActiveRuleCreationResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafActiveRuleData.md` & `fastly-2.3.0/docs/WafActiveRuleData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafActiveRuleDataAttributes.md` & `fastly-2.3.0/docs/WafActiveRuleDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafActiveRuleResponse.md` & `fastly-2.3.0/docs/WafActiveRuleResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafActiveRuleResponseData.md` & `fastly-2.3.0/docs/WafActiveRuleResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafActiveRuleResponseDataAllOf.md` & `fastly-2.3.0/docs/WafActiveRuleResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafActiveRuleResponseDataAttributes.md` & `fastly-2.3.0/docs/WafActiveRuleResponseDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafActiveRuleResponseDataAttributesAllOf.md` & `fastly-2.3.0/docs/WafActiveRuleResponseDataAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafActiveRuleResponseDataRelationships.md` & `fastly-2.3.0/docs/WafActiveRuleResponseDataRelationships.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafActiveRulesApi.md` & `fastly-2.3.0/docs/WafActiveRulesApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafActiveRulesResponse.md` & `fastly-2.3.0/docs/WafActiveRulesResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafActiveRulesResponseAllOf.md` & `fastly-2.3.0/docs/WafActiveRulesResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafExclusion.md` & `fastly-2.3.0/docs/WafExclusion.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafExclusionData.md` & `fastly-2.3.0/docs/WafExclusionData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafExclusionDataAttributes.md` & `fastly-2.3.0/docs/WafExclusionDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafExclusionResponse.md` & `fastly-2.3.0/docs/WafExclusionResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafExclusionResponseData.md` & `fastly-2.3.0/docs/WafExclusionResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafExclusionResponseDataAllOf.md` & `fastly-2.3.0/docs/WafExclusionResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafExclusionResponseDataAttributes.md` & `fastly-2.3.0/docs/WafExclusionResponseDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafExclusionResponseDataAttributesAllOf.md` & `fastly-2.3.0/docs/WafExclusionResponseDataAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafExclusionResponseDataRelationships.md` & `fastly-2.3.0/docs/WafExclusionResponseDataRelationships.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafExclusionsApi.md` & `fastly-2.3.0/docs/WafExclusionsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafExclusionsResponse.md` & `fastly-2.3.0/docs/WafExclusionsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafExclusionsResponseAllOf.md` & `fastly-2.3.0/docs/WafExclusionsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewall.md` & `fastly-2.3.0/docs/WafFirewall.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewallData.md` & `fastly-2.3.0/docs/WafFirewallData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewallDataAttributes.md` & `fastly-2.3.0/docs/WafFirewallDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewallResponse.md` & `fastly-2.3.0/docs/WafFirewallResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewallResponseData.md` & `fastly-2.3.0/docs/WafFirewallResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewallResponseDataAllOf.md` & `fastly-2.3.0/docs/WafFirewallResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewallResponseDataAttributes.md` & `fastly-2.3.0/docs/WafFirewallResponseDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewallResponseDataAttributesAllOf.md` & `fastly-2.3.0/docs/WafFirewallResponseDataAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewallVersion.md` & `fastly-2.3.0/docs/WafFirewallVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewallVersionData.md` & `fastly-2.3.0/docs/WafFirewallVersionData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewallVersionDataAttributes.md` & `fastly-2.3.0/docs/WafFirewallVersionDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewallVersionResponse.md` & `fastly-2.3.0/docs/WafFirewallVersionResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewallVersionResponseData.md` & `fastly-2.3.0/docs/WafFirewallVersionResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewallVersionResponseDataAllOf.md` & `fastly-2.3.0/docs/WafFirewallVersionResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewallVersionResponseDataAttributes.md` & `fastly-2.3.0/docs/WafFirewallVersionResponseDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewallVersionResponseDataAttributesAllOf.md` & `fastly-2.3.0/docs/WafFirewallVersionResponseDataAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewallVersionsApi.md` & `fastly-2.3.0/docs/WafFirewallVersionsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewallVersionsResponse.md` & `fastly-2.3.0/docs/WafFirewallVersionsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewallVersionsResponseAllOf.md` & `fastly-2.3.0/docs/WafFirewallVersionsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewallsApi.md` & `fastly-2.3.0/docs/WafFirewallsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewallsResponse.md` & `fastly-2.3.0/docs/WafFirewallsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafFirewallsResponseAllOf.md` & `fastly-2.3.0/docs/WafFirewallsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafRule.md` & `fastly-2.3.0/docs/WafRule.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafRuleAttributes.md` & `fastly-2.3.0/docs/WafRuleAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafRuleResponse.md` & `fastly-2.3.0/docs/WafRuleResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafRuleResponseData.md` & `fastly-2.3.0/docs/WafRuleResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafRuleResponseDataAllOf.md` & `fastly-2.3.0/docs/WafRuleResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafRuleRevision.md` & `fastly-2.3.0/docs/WafRuleRevision.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafRuleRevisionAttributes.md` & `fastly-2.3.0/docs/WafRuleRevisionAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafRuleRevisionResponse.md` & `fastly-2.3.0/docs/WafRuleRevisionResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafRuleRevisionResponseData.md` & `fastly-2.3.0/docs/WafRuleRevisionResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafRuleRevisionResponseDataAllOf.md` & `fastly-2.3.0/docs/WafRuleRevisionResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafRuleRevisionsApi.md` & `fastly-2.3.0/docs/WafRulesApi.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# fastly.WafRuleRevisionsApi
+# fastly.WafRulesApi
 
 All URIs are relative to *https://api.fastly.com*
 
 Method | HTTP request | Description
 ------------- | ------------- | -------------
-[**get_waf_rule_revision**](WafRuleRevisionsApi.md#get_waf_rule_revision) | **GET** /waf/rules/{waf_rule_id}/revisions/{waf_rule_revision_number} | Get a revision of a rule
-[**list_waf_rule_revisions**](WafRuleRevisionsApi.md#list_waf_rule_revisions) | **GET** /waf/rules/{waf_rule_id}/revisions | List revisions for a rule
+[**get_waf_rule**](WafRulesApi.md#get_waf_rule) | **GET** /waf/rules/{waf_rule_id} | Get a rule
+[**list_waf_rules**](WafRulesApi.md#list_waf_rules) | **GET** /waf/rules | List available WAF rules
 
 
-# **get_waf_rule_revision**
-> WafRuleRevisionResponse get_waf_rule_revision(waf_rule_id, waf_rule_revision_number)
+# **get_waf_rule**
+> WafRuleResponse get_waf_rule(waf_rule_id)
 
-Get a revision of a rule
+Get a rule
 
-Get a specific rule revision.
+Get a specific rule. The `id` provided can be the ModSecurity Rule ID or the Fastly generated rule ID.
 
 ### Example
 
 * Api Key Authentication (token):
 
 ```python
 import time
 import fastly
-from fastly.api import waf_rule_revisions_api
-from fastly.model.waf_rule_revision_response import WafRuleRevisionResponse
+from fastly.api import waf_rules_api
+from fastly.model.waf_rule_response import WafRuleResponse
 from pprint import pprint
 # Defining the host is optional and defaults to https://api.fastly.com
 # See configuration.py for a list of all supported configuration parameters.
 configuration = fastly.Configuration(
     host = "https://api.fastly.com"
 )
 
@@ -41,49 +41,47 @@
 
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['token'] = 'Bearer'
 
 # Enter a context with an instance of the API client
 with fastly.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = waf_rule_revisions_api.WafRuleRevisionsApi(api_client)
+    api_instance = waf_rules_api.WafRulesApi(api_client)
     waf_rule_id = "3krg2uUGZzb2W9Euo4moOR" # str | Alphanumeric string identifying a WAF rule.
-    waf_rule_revision_number = 2 # int | Revision number.
-    include = "source,vcl,waf_rule" # str | Include relationships. Optional, comma-separated values. Permitted values: `waf_rule`, `vcl`, and `source`. The `vcl` and `source` relationships show the WAF VCL and corresponding ModSecurity source. These fields are blank unless the relationship is included.  (optional)
+    include = "waf_tags,waf_rule_revisions" # str | Include relationships. Optional, comma-separated values. Permitted values: `waf_tags` and `waf_rule_revisions`.  (optional)
 
     # example passing only required values which don't have defaults set
     try:
-        # Get a revision of a rule
-        api_response = api_instance.get_waf_rule_revision(waf_rule_id, waf_rule_revision_number)
+        # Get a rule
+        api_response = api_instance.get_waf_rule(waf_rule_id)
         pprint(api_response)
     except fastly.ApiException as e:
-        print("Exception when calling WafRuleRevisionsApi->get_waf_rule_revision: %s\n" % e)
+        print("Exception when calling WafRulesApi->get_waf_rule: %s\n" % e)
 
     # example passing only required values which don't have defaults set
     # and optional values
     try:
-        # Get a revision of a rule
-        api_response = api_instance.get_waf_rule_revision(waf_rule_id, waf_rule_revision_number, include=include)
+        # Get a rule
+        api_response = api_instance.get_waf_rule(waf_rule_id, include=include)
         pprint(api_response)
     except fastly.ApiException as e:
-        print("Exception when calling WafRuleRevisionsApi->get_waf_rule_revision: %s\n" % e)
+        print("Exception when calling WafRulesApi->get_waf_rule: %s\n" % e)
 ```
 
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **waf_rule_id** | **str**| Alphanumeric string identifying a WAF rule. |
- **waf_rule_revision_number** | **int**| Revision number. |
- **include** | **str**| Include relationships. Optional, comma-separated values. Permitted values: `waf_rule`, `vcl`, and `source`. The `vcl` and `source` relationships show the WAF VCL and corresponding ModSecurity source. These fields are blank unless the relationship is included.  | [optional]
+ **include** | **str**| Include relationships. Optional, comma-separated values. Permitted values: `waf_tags` and `waf_rule_revisions`.  | [optional]
 
 ### Return type
 
-[**WafRuleRevisionResponse**](WafRuleRevisionResponse.md)
+[**WafRuleResponse**](WafRuleResponse.md)
 
 ### Authorization
 
 [token](../README.md#token)
 
 ### HTTP request headers
 
@@ -95,30 +93,30 @@
 
 | Status code | Description | Response headers |
 |-------------|-------------|------------------|
 **200** | OK |  -  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
-# **list_waf_rule_revisions**
-> WafRuleRevisionsResponse list_waf_rule_revisions(waf_rule_id)
+# **list_waf_rules**
+> WafRulesResponse list_waf_rules()
 
-List revisions for a rule
+List available WAF rules
 
-List all revisions for a specific rule. The `rule_id` provided can be the ModSecurity Rule ID or the Fastly generated rule ID.
+List all available WAF rules.
 
 ### Example
 
 * Api Key Authentication (token):
 
 ```python
 import time
 import fastly
-from fastly.api import waf_rule_revisions_api
-from fastly.model.waf_rule_revisions_response import WafRuleRevisionsResponse
+from fastly.api import waf_rules_api
+from fastly.model.waf_rules_response import WafRulesResponse
 from pprint import pprint
 # Defining the host is optional and defaults to https://api.fastly.com
 # See configuration.py for a list of all supported configuration parameters.
 configuration = fastly.Configuration(
     host = "https://api.fastly.com"
 )
 
@@ -132,51 +130,49 @@
 
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['token'] = 'Bearer'
 
 # Enter a context with an instance of the API client
 with fastly.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = waf_rule_revisions_api.WafRuleRevisionsApi(api_client)
-    waf_rule_id = "3krg2uUGZzb2W9Euo4moOR" # str | Alphanumeric string identifying a WAF rule.
+    api_instance = waf_rules_api.WafRulesApi(api_client)
+    filter_modsec_rule_id = "filter[modsec_rule_id]_example" # str | Limit the returned rules to a specific ModSecurity rule ID. (optional)
+    filter_waf_tags_name = "filter[waf_tags][name]_example" # str | Limit the returned rules to a set linked to a tag by name. (optional)
+    filter_waf_rule_revisions_source = "filter[waf_rule_revisions][source]_example" # str | Limit the returned rules to a set linked to a source. (optional)
+    filter_waf_firewall_id_not_match = "filter[waf_firewall.id][not][match]_example" # str | Limit the returned rules to a set not included in the active firewall version for a firewall. (optional)
     page_number = 1 # int | Current page. (optional)
     page_size = 20 # int | Number of records per page. (optional) if omitted the server will use the default value of 20
-    include = "waf_rule" # str | Include relationships. Optional. (optional) if omitted the server will use the default value of "waf_rule"
-
-    # example passing only required values which don't have defaults set
-    try:
-        # List revisions for a rule
-        api_response = api_instance.list_waf_rule_revisions(waf_rule_id)
-        pprint(api_response)
-    except fastly.ApiException as e:
-        print("Exception when calling WafRuleRevisionsApi->list_waf_rule_revisions: %s\n" % e)
+    include = "waf_tags,waf_rule_revisions" # str | Include relationships. Optional, comma-separated values. Permitted values: `waf_tags` and `waf_rule_revisions`.  (optional)
 
     # example passing only required values which don't have defaults set
     # and optional values
     try:
-        # List revisions for a rule
-        api_response = api_instance.list_waf_rule_revisions(waf_rule_id, page_number=page_number, page_size=page_size, include=include)
+        # List available WAF rules
+        api_response = api_instance.list_waf_rules(filter_modsec_rule_id=filter_modsec_rule_id, filter_waf_tags_name=filter_waf_tags_name, filter_waf_rule_revisions_source=filter_waf_rule_revisions_source, filter_waf_firewall_id_not_match=filter_waf_firewall_id_not_match, page_number=page_number, page_size=page_size, include=include)
         pprint(api_response)
     except fastly.ApiException as e:
-        print("Exception when calling WafRuleRevisionsApi->list_waf_rule_revisions: %s\n" % e)
+        print("Exception when calling WafRulesApi->list_waf_rules: %s\n" % e)
 ```
 
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
- **waf_rule_id** | **str**| Alphanumeric string identifying a WAF rule. |
+ **filter_modsec_rule_id** | **str**| Limit the returned rules to a specific ModSecurity rule ID. | [optional]
+ **filter_waf_tags_name** | **str**| Limit the returned rules to a set linked to a tag by name. | [optional]
+ **filter_waf_rule_revisions_source** | **str**| Limit the returned rules to a set linked to a source. | [optional]
+ **filter_waf_firewall_id_not_match** | **str**| Limit the returned rules to a set not included in the active firewall version for a firewall. | [optional]
  **page_number** | **int**| Current page. | [optional]
  **page_size** | **int**| Number of records per page. | [optional] if omitted the server will use the default value of 20
- **include** | **str**| Include relationships. Optional. | [optional] if omitted the server will use the default value of "waf_rule"
+ **include** | **str**| Include relationships. Optional, comma-separated values. Permitted values: `waf_tags` and `waf_rule_revisions`.  | [optional]
 
 ### Return type
 
-[**WafRuleRevisionsResponse**](WafRuleRevisionsResponse.md)
+[**WafRulesResponse**](WafRulesResponse.md)
 
 ### Authorization
 
 [token](../README.md#token)
 
 ### HTTP request headers
```

### Comparing `fastly-2.2.2/docs/WafRuleRevisionsResponse.md` & `fastly-2.3.0/docs/WafRuleRevisionsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafRuleRevisionsResponseAllOf.md` & `fastly-2.3.0/docs/WafRuleRevisionsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafRulesResponse.md` & `fastly-2.3.0/docs/WafRulesResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafRulesResponseAllOf.md` & `fastly-2.3.0/docs/WafRulesResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafTag.md` & `fastly-2.3.0/docs/WafTagsResponseDataItem.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# WafTag
+# WafTagsResponseDataItem
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **type** | [**TypeWafTag**](TypeWafTag.md) |  | [optional] 
 **id** | **str** | Alphanumeric string identifying a WAF tag. | [optional] [readonly] 
 **attributes** | [**WafTagAttributes**](WafTagAttributes.md) |  | [optional] 
+**relationships** | [**RelationshipWafRule**](RelationshipWafRule.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-2.2.2/docs/WafTagsApi.md` & `fastly-2.3.0/docs/WafTagsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WafTagsResponse.md` & `fastly-2.3.0/docs/WafTagsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/docs/WsMessageFormat.md` & `fastly-2.3.0/docs/WsMessageFormat.md`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/__init__.py` & `fastly-2.3.0/fastly/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Via the Fastly API you can perform any of the operations that are possible within the management console,  including creating services, domains, and backends, configuring rules or uploading your own application code, as well as account operations such as user administration and billing reports. The API is organized into collections of endpoints that allow manipulation of objects related to Fastly services and accounts. For the most accurate and up-to-date API reference content, visit our [Developer Hub](https://developer.fastly.com/reference/api/)   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: oss@fastly.com
 """
 
 
-__version__ = "2.2.2"
+__version__ = "2.3.0"
 
 # import ApiClient
 from fastly.api_client import ApiClient
 
 # import Configuration
 from fastly.configuration import Configuration
```

### Comparing `fastly-2.2.2/fastly/api_client.py` & `fastly-2.3.0/fastly/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'fastly-py/2.2.2'
+        self.user_agent = 'fastly-py/2.3.0'
 
         # The last observed value of http header Fastly-RateLimit-Remaining
         self.rate_limit_remaining = DEFAULT_RATELIMIT
 
         # The last observed value of http header Fastly-RateLimit-Reset
         self.rate_limit_reset = 0
```

### Comparing `fastly-2.2.2/fastly/configuration.py` & `fastly-2.3.0/fastly/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,15 +442,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 2.2.2".\
+               "SDK Package Version: 2.3.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `fastly-2.2.2/fastly/exceptions.py` & `fastly-2.3.0/fastly/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model_utils.py` & `fastly-2.3.0/fastly/model_utils.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/rest.py` & `fastly-2.3.0/fastly/rest.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/acl_api.py` & `fastly-2.3.0/fastly/api/acl_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/acl_entry_api.py` & `fastly-2.3.0/fastly/api/acl_entry_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/apex_redirect_api.py` & `fastly-2.3.0/fastly/api/apex_redirect_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/backend_api.py` & `fastly-2.3.0/fastly/api/backend_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/billing_address_api.py` & `fastly-2.3.0/fastly/api/billing_address_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/billing_api.py` & `fastly-2.3.0/fastly/api/billing_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/cache_settings_api.py` & `fastly-2.3.0/fastly/api/cache_settings_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/condition_api.py` & `fastly-2.3.0/fastly/api/condition_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/config_store_api.py` & `fastly-2.3.0/fastly/api/config_store_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/config_store_item_api.py` & `fastly-2.3.0/fastly/api/config_store_item_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/contact_api.py` & `fastly-2.3.0/fastly/api/contact_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/content_api.py` & `fastly-2.3.0/fastly/api/content_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/customer_api.py` & `fastly-2.3.0/fastly/api/customer_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/dictionary_api.py` & `fastly-2.3.0/fastly/api/dictionary_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/dictionary_info_api.py` & `fastly-2.3.0/fastly/api/dictionary_info_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/dictionary_item_api.py` & `fastly-2.3.0/fastly/api/dictionary_item_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/diff_api.py` & `fastly-2.3.0/fastly/api/diff_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/director_api.py` & `fastly-2.3.0/fastly/api/director_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/director_backend_api.py` & `fastly-2.3.0/fastly/api/director_backend_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/domain_api.py` & `fastly-2.3.0/fastly/api/domain_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/domain_ownerships_api.py` & `fastly-2.3.0/fastly/api/domain_ownerships_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/enabled_products_api.py` & `fastly-2.3.0/fastly/api/enabled_products_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/events_api.py` & `fastly-2.3.0/fastly/api/events_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/gzip_api.py` & `fastly-2.3.0/fastly/api/gzip_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/header_api.py` & `fastly-2.3.0/fastly/api/header_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/healthcheck_api.py` & `fastly-2.3.0/fastly/api/healthcheck_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/historical_api.py` & `fastly-2.3.0/fastly/api/historical_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/http3_api.py` & `fastly-2.3.0/fastly/api/http3_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/iam_permissions_api.py` & `fastly-2.3.0/fastly/api/iam_permissions_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/iam_roles_api.py` & `fastly-2.3.0/fastly/api/iam_roles_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/iam_service_groups_api.py` & `fastly-2.3.0/fastly/api/iam_service_groups_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/iam_user_groups_api.py` & `fastly-2.3.0/fastly/api/iam_user_groups_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/invitations_api.py` & `fastly-2.3.0/fastly/api/invitations_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/kv_store_api.py` & `fastly-2.3.0/fastly/api/kv_store_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/kv_store_item_api.py` & `fastly-2.3.0/fastly/api/kv_store_item_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_azureblob_api.py` & `fastly-2.3.0/fastly/api/logging_azureblob_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_bigquery_api.py` & `fastly-2.3.0/fastly/api/logging_bigquery_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_cloudfiles_api.py` & `fastly-2.3.0/fastly/api/logging_cloudfiles_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_datadog_api.py` & `fastly-2.3.0/fastly/api/logging_datadog_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_digitalocean_api.py` & `fastly-2.3.0/fastly/api/logging_digitalocean_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_elasticsearch_api.py` & `fastly-2.3.0/fastly/api/logging_elasticsearch_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_ftp_api.py` & `fastly-2.3.0/fastly/api/logging_ftp_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_gcs_api.py` & `fastly-2.3.0/fastly/api/logging_gcs_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_heroku_api.py` & `fastly-2.3.0/fastly/api/logging_heroku_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_honeycomb_api.py` & `fastly-2.3.0/fastly/api/logging_honeycomb_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_https_api.py` & `fastly-2.3.0/fastly/api/logging_https_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_kafka_api.py` & `fastly-2.3.0/fastly/api/logging_kafka_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_kinesis_api.py` & `fastly-2.3.0/fastly/api/logging_kinesis_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_logentries_api.py` & `fastly-2.3.0/fastly/api/logging_logentries_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_loggly_api.py` & `fastly-2.3.0/fastly/api/logging_loggly_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_logshuttle_api.py` & `fastly-2.3.0/fastly/api/logging_logshuttle_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_newrelic_api.py` & `fastly-2.3.0/fastly/api/logging_newrelic_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_openstack_api.py` & `fastly-2.3.0/fastly/api/logging_openstack_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_papertrail_api.py` & `fastly-2.3.0/fastly/api/logging_papertrail_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_pubsub_api.py` & `fastly-2.3.0/fastly/api/logging_pubsub_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_s3_api.py` & `fastly-2.3.0/fastly/api/logging_s3_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_scalyr_api.py` & `fastly-2.3.0/fastly/api/logging_scalyr_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_sftp_api.py` & `fastly-2.3.0/fastly/api/logging_sftp_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_splunk_api.py` & `fastly-2.3.0/fastly/api/logging_splunk_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_sumologic_api.py` & `fastly-2.3.0/fastly/api/logging_sumologic_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/logging_syslog_api.py` & `fastly-2.3.0/fastly/api/logging_syslog_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/mutual_authentication_api.py` & `fastly-2.3.0/fastly/api/mutual_authentication_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/package_api.py` & `fastly-2.3.0/fastly/api/package_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/pool_api.py` & `fastly-2.3.0/fastly/api/pool_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/pop_api.py` & `fastly-2.3.0/fastly/api/pop_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/public_ip_list_api.py` & `fastly-2.3.0/fastly/api/public_ip_list_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/publish_api.py` & `fastly-2.3.0/fastly/api/publish_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/purge_api.py` & `fastly-2.3.0/fastly/api/purge_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/rate_limiter_api.py` & `fastly-2.3.0/fastly/api/realtime_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,167 +17,172 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from fastly.model.inline_response200 import InlineResponse200
-from fastly.model.rate_limiter_response import RateLimiterResponse
+from fastly.model.realtime import Realtime
 
 
-class RateLimiterApi(object):
+class RealtimeApi(object):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.delete_rate_limiter_endpoint = _Endpoint(
+        self.get_stats_last120_seconds_endpoint = _Endpoint(
             settings={
-                'response_type': (InlineResponse200,),
+                'response_type': (Realtime,),
                 'auth': [
                     'token'
                 ],
-                'endpoint_path': '/rate-limiters/{rate_limiter_id}',
-                'operation_id': 'delete_rate_limiter',
-                'http_method': 'DELETE',
+                'endpoint_path': '/v1/channel/{service_id}/ts/h',
+                'operation_id': 'get_stats_last120_seconds',
+                'http_method': 'GET',
                 'servers': [
                     {
-                        'url': "https://api.fastly.com",
+                        'url': "https://rt.fastly.com",
                         'description': "No description provided",
                     },
                 ]
             },
             params_map={
                 'all': [
-                    'rate_limiter_id',
+                    'service_id',
                 ],
                 'required': [
-                    'rate_limiter_id',
+                    'service_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'rate_limiter_id':
+                    'service_id':
                         (str,),
                 },
                 'attribute_map': {
-                    'rate_limiter_id': 'rate_limiter_id',
+                    'service_id': 'service_id',
                 },
                 'location_map': {
-                    'rate_limiter_id': 'path',
+                    'service_id': 'path',
                 },
                 'path_params_allow_reserved_map': {
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_rate_limiter_endpoint = _Endpoint(
+        self.get_stats_last120_seconds_limit_entries_endpoint = _Endpoint(
             settings={
-                'response_type': (RateLimiterResponse,),
+                'response_type': (Realtime,),
                 'auth': [
                     'token'
                 ],
-                'endpoint_path': '/rate-limiters/{rate_limiter_id}',
-                'operation_id': 'get_rate_limiter',
+                'endpoint_path': '/v1/channel/{service_id}/ts/h/limit/{max_entries}',
+                'operation_id': 'get_stats_last120_seconds_limit_entries',
                 'http_method': 'GET',
                 'servers': [
                     {
-                        'url': "https://api.fastly.com",
+                        'url': "https://rt.fastly.com",
                         'description': "No description provided",
                     },
                 ]
             },
             params_map={
                 'all': [
-                    'rate_limiter_id',
+                    'service_id',
+                    'max_entries',
                 ],
                 'required': [
-                    'rate_limiter_id',
+                    'service_id',
+                    'max_entries',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'rate_limiter_id':
+                    'service_id':
                         (str,),
+                    'max_entries':
+                        (int,),
                 },
                 'attribute_map': {
-                    'rate_limiter_id': 'rate_limiter_id',
+                    'service_id': 'service_id',
+                    'max_entries': 'max_entries',
                 },
                 'location_map': {
-                    'rate_limiter_id': 'path',
+                    'service_id': 'path',
+                    'max_entries': 'path',
                 },
                 'path_params_allow_reserved_map': {
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.list_rate_limiters_endpoint = _Endpoint(
+        self.get_stats_last_second_endpoint = _Endpoint(
             settings={
-                'response_type': ([RateLimiterResponse],),
+                'response_type': (Realtime,),
                 'auth': [
                     'token'
                 ],
-                'endpoint_path': '/service/{service_id}/version/{version_id}/rate-limiters',
-                'operation_id': 'list_rate_limiters',
+                'endpoint_path': '/v1/channel/{service_id}/ts/{timestamp_in_seconds}',
+                'operation_id': 'get_stats_last_second',
                 'http_method': 'GET',
                 'servers': [
                     {
-                        'url': "https://api.fastly.com",
+                        'url': "https://rt.fastly.com",
                         'description': "No description provided",
                     },
                 ]
             },
             params_map={
                 'all': [
                     'service_id',
-                    'version_id',
+                    'timestamp_in_seconds',
                 ],
                 'required': [
                     'service_id',
-                    'version_id',
+                    'timestamp_in_seconds',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -186,24 +191,24 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'service_id':
                         (str,),
-                    'version_id':
+                    'timestamp_in_seconds':
                         (int,),
                 },
                 'attribute_map': {
                     'service_id': 'service_id',
-                    'version_id': 'version_id',
+                    'timestamp_in_seconds': 'timestamp_in_seconds',
                 },
                 'location_map': {
                     'service_id': 'path',
-                    'version_id': 'path',
+                    'timestamp_in_seconds': 'path',
                 },
                 'path_params_allow_reserved_map': {
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
@@ -211,30 +216,30 @@
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
 
-    def delete_rate_limiter(
+    def get_stats_last120_seconds(
         self,
-        rate_limiter_id,
+        service_id,
         **kwargs
     ):
-        """Delete a rate limiter  # noqa: E501
+        """Get real-time data for the last 120 seconds  # noqa: E501
 
-        Delete a rate limiter by its ID.  # noqa: E501
+        Get data for the 120 seconds preceding the latest timestamp available for a service.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_rate_limiter(rate_limiter_id, async_req=True)
+        >>> thread = api.get_stats_last120_seconds(service_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            rate_limiter_id (str): Alphanumeric string identifying the rate limiter.
+            service_id (str): Alphanumeric string identifying the service.
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -257,15 +262,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            InlineResponse200
+            Realtime
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -285,34 +290,36 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['rate_limiter_id'] = \
-            rate_limiter_id
-        return self.delete_rate_limiter_endpoint.call_with_http_info(**kwargs)
+        kwargs['service_id'] = \
+            service_id
+        return self.get_stats_last120_seconds_endpoint.call_with_http_info(**kwargs)
 
-    def get_rate_limiter(
+    def get_stats_last120_seconds_limit_entries(
         self,
-        rate_limiter_id,
+        service_id,
+        max_entries,
         **kwargs
     ):
-        """Get a rate limiter  # noqa: E501
+        """Get a limited number of real-time data entries  # noqa: E501
 
-        Get a rate limiter by its ID.  # noqa: E501
+        Get data for the 120 seconds preceding the latest timestamp available for a service, up to a maximum of `max_entries` entries.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_rate_limiter(rate_limiter_id, async_req=True)
+        >>> thread = api.get_stats_last120_seconds_limit_entries(service_id, max_entries, async_req=True)
         >>> result = thread.get()
 
         Args:
-            rate_limiter_id (str): Alphanumeric string identifying the rate limiter.
+            service_id (str): Alphanumeric string identifying the service.
+            max_entries (int): Maximum number of results to show.
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -335,15 +342,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            RateLimiterResponse
+            Realtime
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -363,36 +370,38 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['rate_limiter_id'] = \
-            rate_limiter_id
-        return self.get_rate_limiter_endpoint.call_with_http_info(**kwargs)
+        kwargs['service_id'] = \
+            service_id
+        kwargs['max_entries'] = \
+            max_entries
+        return self.get_stats_last120_seconds_limit_entries_endpoint.call_with_http_info(**kwargs)
 
-    def list_rate_limiters(
+    def get_stats_last_second(
         self,
         service_id,
-        version_id,
+        timestamp_in_seconds,
         **kwargs
     ):
-        """List rate limiters  # noqa: E501
+        """Get real-time data from specified time  # noqa: E501
 
-        List all rate limiters for a particular service and version.  # noqa: E501
+        Get real-time data for the specified reporting period. Specify `0` to get a single entry for the last complete second. The `Timestamp` field included in the response provides the time index of the latest entry in the dataset and can be provided as the `start_timestamp` of the next request for a seamless continuation of the dataset from one request to the next.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_rate_limiters(service_id, version_id, async_req=True)
+        >>> thread = api.get_stats_last_second(service_id, timestamp_in_seconds, async_req=True)
         >>> result = thread.get()
 
         Args:
             service_id (str): Alphanumeric string identifying the service.
-            version_id (int): Integer identifying a service version.
+            timestamp_in_seconds (int): Timestamp in seconds (Unix epoch time).
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -415,15 +424,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            [RateLimiterResponse]
+            Realtime
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -445,11 +454,11 @@
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['service_id'] = \
             service_id
-        kwargs['version_id'] = \
-            version_id
-        return self.list_rate_limiters_endpoint.call_with_http_info(**kwargs)
+        kwargs['timestamp_in_seconds'] = \
+            timestamp_in_seconds
+        return self.get_stats_last_second_endpoint.call_with_http_info(**kwargs)
```

### Comparing `fastly-2.2.2/fastly/api/realtime_api.py` & `fastly-2.3.0/fastly/api/star_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,231 +17,267 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from fastly.model.realtime import Realtime
+from fastly.model.pagination import Pagination
+from fastly.model.star import Star
+from fastly.model.star_response import StarResponse
 
 
-class RealtimeApi(object):
+class StarApi(object):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.get_stats_last120_seconds_endpoint = _Endpoint(
+        self.create_service_star_endpoint = _Endpoint(
             settings={
-                'response_type': (Realtime,),
+                'response_type': (StarResponse,),
                 'auth': [
                     'token'
                 ],
-                'endpoint_path': '/v1/channel/{service_id}/ts/h',
-                'operation_id': 'get_stats_last120_seconds',
-                'http_method': 'GET',
+                'endpoint_path': '/stars',
+                'operation_id': 'create_service_star',
+                'http_method': 'POST',
                 'servers': [
                     {
-                        'url': "https://rt.fastly.com",
+                        'url': "https://api.fastly.com",
                         'description': "No description provided",
                     },
                 ]
             },
             params_map={
                 'all': [
-                    'service_id',
+                    'star',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'star':
+                        (Star,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'star': 'body',
+                },
+                'path_params_allow_reserved_map': {
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/vnd.api+json'
+                ],
+                'content_type': [
+                    'application/vnd.api+json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.delete_service_star_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'token'
+                ],
+                'endpoint_path': '/stars/{star_id}',
+                'operation_id': 'delete_service_star',
+                'http_method': 'DELETE',
+                'servers': [
+                    {
+                        'url': "https://api.fastly.com",
+                        'description': "No description provided",
+                    },
+                ]
+            },
+            params_map={
+                'all': [
+                    'star_id',
                 ],
                 'required': [
-                    'service_id',
+                    'star_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'service_id':
+                    'star_id':
                         (str,),
                 },
                 'attribute_map': {
-                    'service_id': 'service_id',
+                    'star_id': 'star_id',
                 },
                 'location_map': {
-                    'service_id': 'path',
+                    'star_id': 'path',
                 },
                 'path_params_allow_reserved_map': {
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [
-                    'application/json'
-                ],
+                'accept': [],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_stats_last120_seconds_limit_entries_endpoint = _Endpoint(
+        self.get_service_star_endpoint = _Endpoint(
             settings={
-                'response_type': (Realtime,),
+                'response_type': (StarResponse,),
                 'auth': [
                     'token'
                 ],
-                'endpoint_path': '/v1/channel/{service_id}/ts/h/limit/{max_entries}',
-                'operation_id': 'get_stats_last120_seconds_limit_entries',
+                'endpoint_path': '/stars/{star_id}',
+                'operation_id': 'get_service_star',
                 'http_method': 'GET',
                 'servers': [
                     {
-                        'url': "https://rt.fastly.com",
+                        'url': "https://api.fastly.com",
                         'description': "No description provided",
                     },
                 ]
             },
             params_map={
                 'all': [
-                    'service_id',
-                    'max_entries',
+                    'star_id',
                 ],
                 'required': [
-                    'service_id',
-                    'max_entries',
+                    'star_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'service_id':
+                    'star_id':
                         (str,),
-                    'max_entries':
-                        (int,),
                 },
                 'attribute_map': {
-                    'service_id': 'service_id',
-                    'max_entries': 'max_entries',
+                    'star_id': 'star_id',
                 },
                 'location_map': {
-                    'service_id': 'path',
-                    'max_entries': 'path',
+                    'star_id': 'path',
                 },
                 'path_params_allow_reserved_map': {
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
-                    'application/json'
+                    'application/vnd.api+json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_stats_last_second_endpoint = _Endpoint(
+        self.list_service_stars_endpoint = _Endpoint(
             settings={
-                'response_type': (Realtime,),
+                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
                     'token'
                 ],
-                'endpoint_path': '/v1/channel/{service_id}/ts/{timestamp_in_seconds}',
-                'operation_id': 'get_stats_last_second',
+                'endpoint_path': '/stars',
+                'operation_id': 'list_service_stars',
                 'http_method': 'GET',
                 'servers': [
                     {
-                        'url': "https://rt.fastly.com",
+                        'url': "https://api.fastly.com",
                         'description': "No description provided",
                     },
                 ]
             },
             params_map={
                 'all': [
-                    'service_id',
-                    'timestamp_in_seconds',
-                ],
-                'required': [
-                    'service_id',
-                    'timestamp_in_seconds',
                 ],
+                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'service_id':
-                        (str,),
-                    'timestamp_in_seconds':
-                        (int,),
                 },
                 'attribute_map': {
-                    'service_id': 'service_id',
-                    'timestamp_in_seconds': 'timestamp_in_seconds',
                 },
                 'location_map': {
-                    'service_id': 'path',
-                    'timestamp_in_seconds': 'path',
                 },
                 'path_params_allow_reserved_map': {
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
-                    'application/json'
+                    'application/vnd.api+json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
 
-    def get_stats_last120_seconds(
+    def create_service_star(
         self,
-        service_id,
         **kwargs
     ):
-        """Get real-time data for the last 120 seconds  # noqa: E501
+        """Create a star  # noqa: E501
 
-        Get data for the 120 seconds preceding the latest timestamp available for a service.  # noqa: E501
+        Create star.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_stats_last120_seconds(service_id, async_req=True)
+        >>> thread = api.create_service_star(async_req=True)
         >>> result = thread.get()
 
-        Args:
-            service_id (str): Alphanumeric string identifying the service.
 
         Keyword Args:
+            star (Star): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -262,15 +298,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            Realtime
+            StarResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -290,36 +326,32 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['service_id'] = \
-            service_id
-        return self.get_stats_last120_seconds_endpoint.call_with_http_info(**kwargs)
+        return self.create_service_star_endpoint.call_with_http_info(**kwargs)
 
-    def get_stats_last120_seconds_limit_entries(
+    def delete_service_star(
         self,
-        service_id,
-        max_entries,
+        star_id,
         **kwargs
     ):
-        """Get a limited number of real-time data entries  # noqa: E501
+        """Delete a star  # noqa: E501
 
-        Get data for the 120 seconds preceding the latest timestamp available for a service, up to a maximum of `max_entries` entries.  # noqa: E501
+        Delete star.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_stats_last120_seconds_limit_entries(service_id, max_entries, async_req=True)
+        >>> thread = api.delete_service_star(star_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            service_id (str): Alphanumeric string identifying the service.
-            max_entries (int): Maximum number of results to show.
+            star_id (str): Alphanumeric string identifying a star.
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -342,15 +374,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            Realtime
+            None
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -370,38 +402,109 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['service_id'] = \
-            service_id
-        kwargs['max_entries'] = \
-            max_entries
-        return self.get_stats_last120_seconds_limit_entries_endpoint.call_with_http_info(**kwargs)
+        kwargs['star_id'] = \
+            star_id
+        return self.delete_service_star_endpoint.call_with_http_info(**kwargs)
 
-    def get_stats_last_second(
+    def get_service_star(
         self,
-        service_id,
-        timestamp_in_seconds,
+        star_id,
         **kwargs
     ):
-        """Get real-time data from specified time  # noqa: E501
+        """Get a star  # noqa: E501
 
-        Get real-time data for the specified reporting period. Specify `0` to get a single entry for the last complete second. The `Timestamp` field included in the response provides the time index of the latest entry in the dataset and can be provided as the `start_timestamp` of the next request for a seamless continuation of the dataset from one request to the next.  # noqa: E501
+        Show star.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_stats_last_second(service_id, timestamp_in_seconds, async_req=True)
+        >>> thread = api.get_service_star(star_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            service_id (str): Alphanumeric string identifying the service.
-            timestamp_in_seconds (int): Timestamp in seconds (Unix epoch time).
+            star_id (str): Alphanumeric string identifying a star.
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            StarResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['star_id'] = \
+            star_id
+        return self.get_service_star_endpoint.call_with_http_info(**kwargs)
+
+    def list_service_stars(
+        self,
+        **kwargs
+    ):
+        """List stars  # noqa: E501
+
+        List stars.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.list_service_stars(async_req=True)
+        >>> result = thread.get()
+
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -424,15 +527,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            Realtime
+            bool, date, datetime, dict, float, int, list, str, none_type
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -452,13 +555,9 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['service_id'] = \
-            service_id
-        kwargs['timestamp_in_seconds'] = \
-            timestamp_in_seconds
-        return self.get_stats_last_second_endpoint.call_with_http_info(**kwargs)
+        return self.list_service_stars_endpoint.call_with_http_info(**kwargs)
```

### Comparing `fastly-2.2.2/fastly/api/request_settings_api.py` & `fastly-2.3.0/fastly/api/request_settings_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/resource_api.py` & `fastly-2.3.0/fastly/api/resource_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/response_object_api.py` & `fastly-2.3.0/fastly/api/response_object_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/server_api.py` & `fastly-2.3.0/fastly/api/server_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/service_api.py` & `fastly-2.3.0/fastly/api/service_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/service_authorizations_api.py` & `fastly-2.3.0/fastly/api/service_authorizations_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/settings_api.py` & `fastly-2.3.0/fastly/api/settings_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/snippet_api.py` & `fastly-2.3.0/fastly/api/snippet_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/star_api.py` & `fastly-2.3.0/fastly/api/tls_private_keys_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,47 +17,47 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from fastly.model.pagination import Pagination
-from fastly.model.star import Star
-from fastly.model.star_response import StarResponse
+from fastly.model.tls_private_key import TlsPrivateKey
+from fastly.model.tls_private_key_response import TlsPrivateKeyResponse
+from fastly.model.tls_private_keys_response import TlsPrivateKeysResponse
 
 
-class StarApi(object):
+class TlsPrivateKeysApi(object):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.create_service_star_endpoint = _Endpoint(
+        self.create_tls_key_endpoint = _Endpoint(
             settings={
-                'response_type': (StarResponse,),
+                'response_type': (TlsPrivateKeyResponse,),
                 'auth': [
                     'token'
                 ],
-                'endpoint_path': '/stars',
-                'operation_id': 'create_service_star',
+                'endpoint_path': '/tls/private_keys',
+                'operation_id': 'create_tls_key',
                 'http_method': 'POST',
                 'servers': [
                     {
                         'url': "https://api.fastly.com",
                         'description': "No description provided",
                     },
                 ]
             },
             params_map={
                 'all': [
-                    'star',
+                    'tls_private_key',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -65,21 +65,21 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'star':
-                        (Star,),
+                    'tls_private_key':
+                        (TlsPrivateKey,),
                 },
                 'attribute_map': {
                 },
                 'location_map': {
-                    'star': 'body',
+                    'tls_private_key': 'body',
                 },
                 'path_params_allow_reserved_map': {
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
@@ -88,165 +88,186 @@
                 ],
                 'content_type': [
                     'application/vnd.api+json'
                 ]
             },
             api_client=api_client
         )
-        self.delete_service_star_endpoint = _Endpoint(
+        self.delete_tls_key_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'token'
                 ],
-                'endpoint_path': '/stars/{star_id}',
-                'operation_id': 'delete_service_star',
+                'endpoint_path': '/tls/private_keys/{tls_private_key_id}',
+                'operation_id': 'delete_tls_key',
                 'http_method': 'DELETE',
                 'servers': [
                     {
                         'url': "https://api.fastly.com",
                         'description': "No description provided",
                     },
                 ]
             },
             params_map={
                 'all': [
-                    'star_id',
+                    'tls_private_key_id',
                 ],
                 'required': [
-                    'star_id',
+                    'tls_private_key_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'star_id':
+                    'tls_private_key_id':
                         (str,),
                 },
                 'attribute_map': {
-                    'star_id': 'star_id',
+                    'tls_private_key_id': 'tls_private_key_id',
                 },
                 'location_map': {
-                    'star_id': 'path',
+                    'tls_private_key_id': 'path',
                 },
                 'path_params_allow_reserved_map': {
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_service_star_endpoint = _Endpoint(
+        self.get_tls_key_endpoint = _Endpoint(
             settings={
-                'response_type': (StarResponse,),
+                'response_type': (TlsPrivateKeyResponse,),
                 'auth': [
                     'token'
                 ],
-                'endpoint_path': '/stars/{star_id}',
-                'operation_id': 'get_service_star',
+                'endpoint_path': '/tls/private_keys/{tls_private_key_id}',
+                'operation_id': 'get_tls_key',
                 'http_method': 'GET',
                 'servers': [
                     {
                         'url': "https://api.fastly.com",
                         'description': "No description provided",
                     },
                 ]
             },
             params_map={
                 'all': [
-                    'star_id',
+                    'tls_private_key_id',
                 ],
                 'required': [
-                    'star_id',
+                    'tls_private_key_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'star_id':
+                    'tls_private_key_id':
                         (str,),
                 },
                 'attribute_map': {
-                    'star_id': 'star_id',
+                    'tls_private_key_id': 'tls_private_key_id',
                 },
                 'location_map': {
-                    'star_id': 'path',
+                    'tls_private_key_id': 'path',
                 },
                 'path_params_allow_reserved_map': {
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.api+json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.list_service_stars_endpoint = _Endpoint(
+        self.list_tls_keys_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': (TlsPrivateKeysResponse,),
                 'auth': [
                     'token'
                 ],
-                'endpoint_path': '/stars',
-                'operation_id': 'list_service_stars',
+                'endpoint_path': '/tls/private_keys',
+                'operation_id': 'list_tls_keys',
                 'http_method': 'GET',
                 'servers': [
                     {
                         'url': "https://api.fastly.com",
                         'description': "No description provided",
                     },
                 ]
             },
             params_map={
                 'all': [
+                    'filter_in_use',
+                    'page_number',
+                    'page_size',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
+                    'page_size',
                 ]
             },
             root_map={
                 'validations': {
+                    ('page_size',): {
+
+                        'inclusive_maximum': 100,
+                        'inclusive_minimum': 1,
+                    },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
+                    'filter_in_use':
+                        (str,),
+                    'page_number':
+                        (int,),
+                    'page_size':
+                        (int,),
                 },
                 'attribute_map': {
+                    'filter_in_use': 'filter[in_use]',
+                    'page_number': 'page[number]',
+                    'page_size': 'page[size]',
                 },
                 'location_map': {
+                    'filter_in_use': 'query',
+                    'page_number': 'query',
+                    'page_size': 'query',
                 },
                 'path_params_allow_reserved_map': {
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
@@ -254,30 +275,30 @@
                     'application/vnd.api+json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
 
-    def create_service_star(
+    def create_tls_key(
         self,
         **kwargs
     ):
-        """Create a star  # noqa: E501
+        """Create a TLS private key  # noqa: E501
 
-        Create star.  # noqa: E501
+        Create a TLS private key.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_service_star(async_req=True)
+        >>> thread = api.create_tls_key(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            star (Star): [optional]
+            tls_private_key (TlsPrivateKey): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -298,15 +319,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            StarResponse
+            TlsPrivateKeyResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -326,32 +347,32 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.create_service_star_endpoint.call_with_http_info(**kwargs)
+        return self.create_tls_key_endpoint.call_with_http_info(**kwargs)
 
-    def delete_service_star(
+    def delete_tls_key(
         self,
-        star_id,
+        tls_private_key_id,
         **kwargs
     ):
-        """Delete a star  # noqa: E501
+        """Delete a TLS private key  # noqa: E501
 
-        Delete star.  # noqa: E501
+        Destroy a TLS private key. Only private keys not already matched to any certificates can be deleted.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_service_star(star_id, async_req=True)
+        >>> thread = api.delete_tls_key(tls_private_key_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            star_id (str): Alphanumeric string identifying a star.
+            tls_private_key_id (str): Alphanumeric string identifying a private Key.
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -402,34 +423,34 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['star_id'] = \
-            star_id
-        return self.delete_service_star_endpoint.call_with_http_info(**kwargs)
+        kwargs['tls_private_key_id'] = \
+            tls_private_key_id
+        return self.delete_tls_key_endpoint.call_with_http_info(**kwargs)
 
-    def get_service_star(
+    def get_tls_key(
         self,
-        star_id,
+        tls_private_key_id,
         **kwargs
     ):
-        """Get a star  # noqa: E501
+        """Get a TLS private key  # noqa: E501
 
-        Show star.  # noqa: E501
+        Show a TLS private key.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_service_star(star_id, async_req=True)
+        >>> thread = api.get_tls_key(tls_private_key_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            star_id (str): Alphanumeric string identifying a star.
+            tls_private_key_id (str): Alphanumeric string identifying a private Key.
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -452,15 +473,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            StarResponse
+            TlsPrivateKeyResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -480,33 +501,36 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['star_id'] = \
-            star_id
-        return self.get_service_star_endpoint.call_with_http_info(**kwargs)
+        kwargs['tls_private_key_id'] = \
+            tls_private_key_id
+        return self.get_tls_key_endpoint.call_with_http_info(**kwargs)
 
-    def list_service_stars(
+    def list_tls_keys(
         self,
         **kwargs
     ):
-        """List stars  # noqa: E501
+        """List TLS private keys  # noqa: E501
 
-        List stars.  # noqa: E501
+        List all TLS private keys.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_service_stars(async_req=True)
+        >>> thread = api.list_tls_keys(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
+            filter_in_use (str): Limit the returned keys to those without any matching TLS certificates. The only valid value is false.. [optional]
+            page_number (int): Current page.. [optional]
+            page_size (int): Number of records per page.. [optional] if omitted the server will use the default value of 20
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -527,15 +551,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            TlsPrivateKeysResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -555,9 +579,9 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.list_service_stars_endpoint.call_with_http_info(**kwargs)
+        return self.list_tls_keys_endpoint.call_with_http_info(**kwargs)
```

### Comparing `fastly-2.2.2/fastly/api/stats_api.py` & `fastly-2.3.0/fastly/api/stats_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/tls_activations_api.py` & `fastly-2.3.0/fastly/api/tls_activations_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/tls_bulk_certificates_api.py` & `fastly-2.3.0/fastly/api/tls_bulk_certificates_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/tls_certificates_api.py` & `fastly-2.3.0/fastly/api/tls_certificates_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/tls_configurations_api.py` & `fastly-2.3.0/fastly/api/tls_configurations_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/tls_domains_api.py` & `fastly-2.3.0/fastly/api/tls_domains_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/tls_private_keys_api.py` & `fastly-2.3.0/fastly/api/tokens_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,288 +17,373 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from fastly.model.tls_private_key import TlsPrivateKey
-from fastly.model.tls_private_key_response import TlsPrivateKeyResponse
-from fastly.model.tls_private_keys_response import TlsPrivateKeysResponse
+from fastly.model.generic_token_error import GenericTokenError
+from fastly.model.token_response import TokenResponse
 
 
-class TlsPrivateKeysApi(object):
+class TokensApi(object):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.create_tls_key_endpoint = _Endpoint(
+        self.get_token_endpoint = _Endpoint(
             settings={
-                'response_type': (TlsPrivateKeyResponse,),
+                'response_type': (TokenResponse,),
                 'auth': [
                     'token'
                 ],
-                'endpoint_path': '/tls/private_keys',
-                'operation_id': 'create_tls_key',
-                'http_method': 'POST',
+                'endpoint_path': '/tokens/{token_id}',
+                'operation_id': 'get_token',
+                'http_method': 'GET',
                 'servers': [
                     {
                         'url': "https://api.fastly.com",
                         'description': "No description provided",
                     },
                 ]
             },
             params_map={
                 'all': [
-                    'tls_private_key',
+                    'token_id',
+                ],
+                'required': [
+                    'token_id',
                 ],
-                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'tls_private_key':
-                        (TlsPrivateKey,),
+                    'token_id':
+                        (str,),
                 },
                 'attribute_map': {
+                    'token_id': 'token_id',
                 },
                 'location_map': {
-                    'tls_private_key': 'body',
+                    'token_id': 'path',
                 },
                 'path_params_allow_reserved_map': {
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
-                    'application/vnd.api+json'
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.get_token_current_endpoint = _Endpoint(
+            settings={
+                'response_type': (TokenResponse,),
+                'auth': [
+                    'token'
                 ],
-                'content_type': [
-                    'application/vnd.api+json'
+                'endpoint_path': '/tokens/self',
+                'operation_id': 'get_token_current',
+                'http_method': 'GET',
+                'servers': [
+                    {
+                        'url': "https://api.fastly.com",
+                        'description': "No description provided",
+                    },
                 ]
             },
+            params_map={
+                'all': [
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                },
+                'path_params_allow_reserved_map': {
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
             api_client=api_client
         )
-        self.delete_tls_key_endpoint = _Endpoint(
+        self.list_tokens_customer_endpoint = _Endpoint(
             settings={
-                'response_type': None,
+                'response_type': ([TokenResponse],),
                 'auth': [
                     'token'
                 ],
-                'endpoint_path': '/tls/private_keys/{tls_private_key_id}',
-                'operation_id': 'delete_tls_key',
-                'http_method': 'DELETE',
+                'endpoint_path': '/customer/{customer_id}/tokens',
+                'operation_id': 'list_tokens_customer',
+                'http_method': 'GET',
                 'servers': [
                     {
                         'url': "https://api.fastly.com",
                         'description': "No description provided",
                     },
                 ]
             },
             params_map={
                 'all': [
-                    'tls_private_key_id',
+                    'customer_id',
                 ],
                 'required': [
-                    'tls_private_key_id',
+                    'customer_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'tls_private_key_id':
+                    'customer_id':
                         (str,),
                 },
                 'attribute_map': {
-                    'tls_private_key_id': 'tls_private_key_id',
+                    'customer_id': 'customer_id',
                 },
                 'location_map': {
-                    'tls_private_key_id': 'path',
+                    'customer_id': 'path',
                 },
                 'path_params_allow_reserved_map': {
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [],
+                'accept': [
+                    'application/json'
+                ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_tls_key_endpoint = _Endpoint(
+        self.list_tokens_user_endpoint = _Endpoint(
             settings={
-                'response_type': (TlsPrivateKeyResponse,),
+                'response_type': ([TokenResponse],),
                 'auth': [
                     'token'
                 ],
-                'endpoint_path': '/tls/private_keys/{tls_private_key_id}',
-                'operation_id': 'get_tls_key',
+                'endpoint_path': '/tokens',
+                'operation_id': 'list_tokens_user',
                 'http_method': 'GET',
                 'servers': [
                     {
                         'url': "https://api.fastly.com",
                         'description': "No description provided",
                     },
                 ]
             },
             params_map={
                 'all': [
-                    'tls_private_key_id',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                },
+                'path_params_allow_reserved_map': {
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.revoke_token_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'token'
+                ],
+                'endpoint_path': '/tokens/{token_id}',
+                'operation_id': 'revoke_token',
+                'http_method': 'DELETE',
+                'servers': [
+                    {
+                        'url': "https://api.fastly.com",
+                        'description': "No description provided",
+                    },
+                ]
+            },
+            params_map={
+                'all': [
+                    'token_id',
                 ],
                 'required': [
-                    'tls_private_key_id',
+                    'token_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'tls_private_key_id':
+                    'token_id':
                         (str,),
                 },
                 'attribute_map': {
-                    'tls_private_key_id': 'tls_private_key_id',
+                    'token_id': 'token_id',
                 },
                 'location_map': {
-                    'tls_private_key_id': 'path',
+                    'token_id': 'path',
                 },
                 'path_params_allow_reserved_map': {
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
-                    'application/vnd.api+json'
+                    'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.list_tls_keys_endpoint = _Endpoint(
+        self.revoke_token_current_endpoint = _Endpoint(
             settings={
-                'response_type': (TlsPrivateKeysResponse,),
+                'response_type': None,
                 'auth': [
                     'token'
                 ],
-                'endpoint_path': '/tls/private_keys',
-                'operation_id': 'list_tls_keys',
-                'http_method': 'GET',
+                'endpoint_path': '/tokens/self',
+                'operation_id': 'revoke_token_current',
+                'http_method': 'DELETE',
                 'servers': [
                     {
                         'url': "https://api.fastly.com",
                         'description': "No description provided",
                     },
                 ]
             },
             params_map={
                 'all': [
-                    'filter_in_use',
-                    'page_number',
-                    'page_size',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
-                    'page_size',
                 ]
             },
             root_map={
                 'validations': {
-                    ('page_size',): {
-
-                        'inclusive_maximum': 100,
-                        'inclusive_minimum': 1,
-                    },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'filter_in_use':
-                        (str,),
-                    'page_number':
-                        (int,),
-                    'page_size':
-                        (int,),
                 },
                 'attribute_map': {
-                    'filter_in_use': 'filter[in_use]',
-                    'page_number': 'page[number]',
-                    'page_size': 'page[size]',
                 },
                 'location_map': {
-                    'filter_in_use': 'query',
-                    'page_number': 'query',
-                    'page_size': 'query',
                 },
                 'path_params_allow_reserved_map': {
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
-                    'application/vnd.api+json'
+                    'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
 
-    def create_tls_key(
+    def get_token(
         self,
+        token_id,
         **kwargs
     ):
-        """Create a TLS private key  # noqa: E501
+        """Get a token  # noqa: E501
 
-        Create a TLS private key.  # noqa: E501
+        Get a single token by its id.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_tls_key(async_req=True)
+        >>> thread = api.get_token(token_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            token_id (str): Alphanumeric string identifying a token.
 
         Keyword Args:
-            tls_private_key (TlsPrivateKey): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -319,15 +404,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            TlsPrivateKeyResponse
+            TokenResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -347,32 +432,107 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.create_tls_key_endpoint.call_with_http_info(**kwargs)
+        kwargs['token_id'] = \
+            token_id
+        return self.get_token_endpoint.call_with_http_info(**kwargs)
 
-    def delete_tls_key(
+    def get_token_current(
         self,
-        tls_private_key_id,
         **kwargs
     ):
-        """Delete a TLS private key  # noqa: E501
+        """Get the current token  # noqa: E501
 
-        Destroy a TLS private key. Only private keys not already matched to any certificates can be deleted.  # noqa: E501
+        Get a single token based on the access_token used in the request.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_tls_key(tls_private_key_id, async_req=True)
+        >>> thread = api.get_token_current(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            TokenResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        return self.get_token_current_endpoint.call_with_http_info(**kwargs)
+
+    def list_tokens_customer(
+        self,
+        customer_id,
+        **kwargs
+    ):
+        """List tokens for a customer  # noqa: E501
+
+        List all tokens belonging to a specific customer.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.list_tokens_customer(customer_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            tls_private_key_id (str): Alphanumeric string identifying a private Key.
+            customer_id (str): Alphanumeric string identifying the customer.
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -395,15 +555,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            None
+            [TokenResponse]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -423,34 +583,107 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['tls_private_key_id'] = \
-            tls_private_key_id
-        return self.delete_tls_key_endpoint.call_with_http_info(**kwargs)
+        kwargs['customer_id'] = \
+            customer_id
+        return self.list_tokens_customer_endpoint.call_with_http_info(**kwargs)
 
-    def get_tls_key(
+    def list_tokens_user(
         self,
-        tls_private_key_id,
         **kwargs
     ):
-        """Get a TLS private key  # noqa: E501
+        """List tokens for the authenticated user  # noqa: E501
 
-        Show a TLS private key.  # noqa: E501
+        List all tokens belonging to the authenticated user.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_tls_key(tls_private_key_id, async_req=True)
+        >>> thread = api.list_tokens_user(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            [TokenResponse]
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        return self.list_tokens_user_endpoint.call_with_http_info(**kwargs)
+
+    def revoke_token(
+        self,
+        token_id,
+        **kwargs
+    ):
+        """Revoke a token  # noqa: E501
+
+        Revoke a specific token by its id.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.revoke_token(token_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            tls_private_key_id (str): Alphanumeric string identifying a private Key.
+            token_id (str): Alphanumeric string identifying a token.
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -473,15 +706,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            TlsPrivateKeyResponse
+            None
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -501,36 +734,33 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['tls_private_key_id'] = \
-            tls_private_key_id
-        return self.get_tls_key_endpoint.call_with_http_info(**kwargs)
+        kwargs['token_id'] = \
+            token_id
+        return self.revoke_token_endpoint.call_with_http_info(**kwargs)
 
-    def list_tls_keys(
+    def revoke_token_current(
         self,
         **kwargs
     ):
-        """List TLS private keys  # noqa: E501
+        """Revoke the current token  # noqa: E501
 
-        List all TLS private keys.  # noqa: E501
+        Revoke a token that is used to authenticate the request.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_tls_keys(async_req=True)
+        >>> thread = api.revoke_token_current(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            filter_in_use (str): Limit the returned keys to those without any matching TLS certificates. The only valid value is false.. [optional]
-            page_number (int): Current page.. [optional]
-            page_size (int): Number of records per page.. [optional] if omitted the server will use the default value of 20
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -551,15 +781,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            TlsPrivateKeysResponse
+            None
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -579,9 +809,9 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.list_tls_keys_endpoint.call_with_http_info(**kwargs)
+        return self.revoke_token_current_endpoint.call_with_http_info(**kwargs)
```

### Comparing `fastly-2.2.2/fastly/api/tls_subscriptions_api.py` & `fastly-2.3.0/fastly/api/tls_subscriptions_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/tokens_api.py` & `fastly-2.3.0/fastly/api/waf_firewalls_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,373 +17,388 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from fastly.model.generic_token_error import GenericTokenError
-from fastly.model.token_response import TokenResponse
+from fastly.model.waf_firewall import WafFirewall
+from fastly.model.waf_firewall_response import WafFirewallResponse
+from fastly.model.waf_firewalls_response import WafFirewallsResponse
 
 
-class TokensApi(object):
+class WafFirewallsApi(object):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.get_token_endpoint = _Endpoint(
+        self.create_waf_firewall_endpoint = _Endpoint(
             settings={
-                'response_type': (TokenResponse,),
+                'response_type': (WafFirewallResponse,),
                 'auth': [
                     'token'
                 ],
-                'endpoint_path': '/tokens/{token_id}',
-                'operation_id': 'get_token',
-                'http_method': 'GET',
+                'endpoint_path': '/waf/firewalls',
+                'operation_id': 'create_waf_firewall',
+                'http_method': 'POST',
                 'servers': [
                     {
                         'url': "https://api.fastly.com",
                         'description': "No description provided",
                     },
                 ]
             },
             params_map={
                 'all': [
-                    'token_id',
-                ],
-                'required': [
-                    'token_id',
+                    'waf_firewall',
                 ],
+                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'token_id':
-                        (str,),
+                    'waf_firewall':
+                        (WafFirewall,),
                 },
                 'attribute_map': {
-                    'token_id': 'token_id',
                 },
                 'location_map': {
-                    'token_id': 'path',
+                    'waf_firewall': 'body',
                 },
                 'path_params_allow_reserved_map': {
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
-                    'application/json'
+                    'application/vnd.api+json'
                 ],
-                'content_type': [],
+                'content_type': [
+                    'application/vnd.api+json'
+                ]
             },
             api_client=api_client
         )
-        self.get_token_current_endpoint = _Endpoint(
+        self.delete_waf_firewall_endpoint = _Endpoint(
             settings={
-                'response_type': (TokenResponse,),
+                'response_type': None,
                 'auth': [
                     'token'
                 ],
-                'endpoint_path': '/tokens/self',
-                'operation_id': 'get_token_current',
-                'http_method': 'GET',
+                'endpoint_path': '/waf/firewalls/{firewall_id}',
+                'operation_id': 'delete_waf_firewall',
+                'http_method': 'DELETE',
                 'servers': [
                     {
                         'url': "https://api.fastly.com",
                         'description': "No description provided",
                     },
                 ]
             },
             params_map={
                 'all': [
+                    'firewall_id',
+                    'waf_firewall',
+                ],
+                'required': [
+                    'firewall_id',
                 ],
-                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
+                    'firewall_id':
+                        (str,),
+                    'waf_firewall':
+                        (WafFirewall,),
                 },
                 'attribute_map': {
+                    'firewall_id': 'firewall_id',
                 },
                 'location_map': {
+                    'firewall_id': 'path',
+                    'waf_firewall': 'body',
                 },
                 'path_params_allow_reserved_map': {
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [
+                'accept': [],
+                'content_type': [
                     'application/json'
-                ],
-                'content_type': [],
+                ]
             },
             api_client=api_client
         )
-        self.list_tokens_customer_endpoint = _Endpoint(
+        self.get_waf_firewall_endpoint = _Endpoint(
             settings={
-                'response_type': ([TokenResponse],),
+                'response_type': (WafFirewallResponse,),
                 'auth': [
                     'token'
                 ],
-                'endpoint_path': '/customer/{customer_id}/tokens',
-                'operation_id': 'list_tokens_customer',
+                'endpoint_path': '/waf/firewalls/{firewall_id}',
+                'operation_id': 'get_waf_firewall',
                 'http_method': 'GET',
                 'servers': [
                     {
                         'url': "https://api.fastly.com",
                         'description': "No description provided",
                     },
                 ]
             },
             params_map={
                 'all': [
-                    'customer_id',
+                    'firewall_id',
+                    'filter_service_version_number',
+                    'include',
                 ],
                 'required': [
-                    'customer_id',
+                    'firewall_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
+                    'include',
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
+                    ('include',): {
+
+                        "WAF_FIREWALL_VERSIONS": "waf_firewall_versions"
+                    },
                 },
                 'openapi_types': {
-                    'customer_id':
+                    'firewall_id':
+                        (str,),
+                    'filter_service_version_number':
+                        (str,),
+                    'include':
                         (str,),
                 },
                 'attribute_map': {
-                    'customer_id': 'customer_id',
+                    'firewall_id': 'firewall_id',
+                    'filter_service_version_number': 'filter[service_version_number]',
+                    'include': 'include',
                 },
                 'location_map': {
-                    'customer_id': 'path',
+                    'firewall_id': 'path',
+                    'filter_service_version_number': 'query',
+                    'include': 'query',
                 },
                 'path_params_allow_reserved_map': {
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
-                    'application/json'
+                    'application/vnd.api+json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.list_tokens_user_endpoint = _Endpoint(
+        self.list_waf_firewalls_endpoint = _Endpoint(
             settings={
-                'response_type': ([TokenResponse],),
+                'response_type': (WafFirewallsResponse,),
                 'auth': [
                     'token'
                 ],
-                'endpoint_path': '/tokens',
-                'operation_id': 'list_tokens_user',
+                'endpoint_path': '/waf/firewalls',
+                'operation_id': 'list_waf_firewalls',
                 'http_method': 'GET',
                 'servers': [
                     {
                         'url': "https://api.fastly.com",
                         'description': "No description provided",
                     },
                 ]
             },
             params_map={
                 'all': [
+                    'page_number',
+                    'page_size',
+                    'filter_service_id',
+                    'filter_service_version_number',
+                    'include',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
+                    'include',
                 ],
                 'validation': [
+                    'page_size',
                 ]
             },
             root_map={
                 'validations': {
+                    ('page_size',): {
+
+                        'inclusive_maximum': 100,
+                        'inclusive_minimum': 1,
+                    },
                 },
                 'allowed_values': {
+                    ('include',): {
+
+                        "WAF_FIREWALL_VERSIONS": "waf_firewall_versions"
+                    },
                 },
                 'openapi_types': {
+                    'page_number':
+                        (int,),
+                    'page_size':
+                        (int,),
+                    'filter_service_id':
+                        (str,),
+                    'filter_service_version_number':
+                        (str,),
+                    'include':
+                        (str,),
                 },
                 'attribute_map': {
+                    'page_number': 'page[number]',
+                    'page_size': 'page[size]',
+                    'filter_service_id': 'filter[service_id]',
+                    'filter_service_version_number': 'filter[service_version_number]',
+                    'include': 'include',
                 },
                 'location_map': {
+                    'page_number': 'query',
+                    'page_size': 'query',
+                    'filter_service_id': 'query',
+                    'filter_service_version_number': 'query',
+                    'include': 'query',
                 },
                 'path_params_allow_reserved_map': {
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
-                    'application/json'
+                    'application/vnd.api+json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.revoke_token_endpoint = _Endpoint(
+        self.update_waf_firewall_endpoint = _Endpoint(
             settings={
-                'response_type': None,
+                'response_type': (WafFirewallResponse,),
                 'auth': [
                     'token'
                 ],
-                'endpoint_path': '/tokens/{token_id}',
-                'operation_id': 'revoke_token',
-                'http_method': 'DELETE',
+                'endpoint_path': '/waf/firewalls/{firewall_id}',
+                'operation_id': 'update_waf_firewall',
+                'http_method': 'PATCH',
                 'servers': [
                     {
                         'url': "https://api.fastly.com",
                         'description': "No description provided",
                     },
                 ]
             },
             params_map={
                 'all': [
-                    'token_id',
+                    'firewall_id',
+                    'waf_firewall',
                 ],
                 'required': [
-                    'token_id',
+                    'firewall_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'token_id':
+                    'firewall_id':
                         (str,),
+                    'waf_firewall':
+                        (WafFirewall,),
                 },
                 'attribute_map': {
-                    'token_id': 'token_id',
+                    'firewall_id': 'firewall_id',
                 },
                 'location_map': {
-                    'token_id': 'path',
+                    'firewall_id': 'path',
+                    'waf_firewall': 'body',
                 },
                 'path_params_allow_reserved_map': {
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-        self.revoke_token_current_endpoint = _Endpoint(
-            settings={
-                'response_type': None,
-                'auth': [
-                    'token'
+                    'application/vnd.api+json'
                 ],
-                'endpoint_path': '/tokens/self',
-                'operation_id': 'revoke_token_current',
-                'http_method': 'DELETE',
-                'servers': [
-                    {
-                        'url': "https://api.fastly.com",
-                        'description': "No description provided",
-                    },
+                'content_type': [
+                    'application/vnd.api+json'
                 ]
             },
-            params_map={
-                'all': [
-                ],
-                'required': [],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                },
-                'attribute_map': {
-                },
-                'location_map': {
-                },
-                'path_params_allow_reserved_map': {
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
             api_client=api_client
         )
 
-    def get_token(
+    def create_waf_firewall(
         self,
-        token_id,
         **kwargs
     ):
-        """Get a token  # noqa: E501
+        """Create a firewall  # noqa: E501
 
-        Get a single token by its id.  # noqa: E501
+        Create a firewall object for a particular service and service version using a defined `prefetch_condition` and `response`. If the `prefetch_condition` or the `response` is missing from the request body, Fastly will generate a default object on your service.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_token(token_id, async_req=True)
+        >>> thread = api.create_waf_firewall(async_req=True)
         >>> result = thread.get()
 
-        Args:
-            token_id (str): Alphanumeric string identifying a token.
 
         Keyword Args:
+            waf_firewall (WafFirewall): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -404,15 +419,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            TokenResponse
+            WafFirewallResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -432,33 +447,35 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['token_id'] = \
-            token_id
-        return self.get_token_endpoint.call_with_http_info(**kwargs)
+        return self.create_waf_firewall_endpoint.call_with_http_info(**kwargs)
 
-    def get_token_current(
+    def delete_waf_firewall(
         self,
+        firewall_id,
         **kwargs
     ):
-        """Get the current token  # noqa: E501
+        """Delete a firewall  # noqa: E501
 
-        Get a single token based on the access_token used in the request.  # noqa: E501
+        Delete the firewall object for a particular service and service version.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_token_current(async_req=True)
+        >>> thread = api.delete_waf_firewall(firewall_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            firewall_id (str): Alphanumeric string identifying a WAF Firewall.
 
         Keyword Args:
+            waf_firewall (WafFirewall): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -479,15 +496,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            TokenResponse
+            None
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -507,34 +524,38 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.get_token_current_endpoint.call_with_http_info(**kwargs)
+        kwargs['firewall_id'] = \
+            firewall_id
+        return self.delete_waf_firewall_endpoint.call_with_http_info(**kwargs)
 
-    def list_tokens_customer(
+    def get_waf_firewall(
         self,
-        customer_id,
+        firewall_id,
         **kwargs
     ):
-        """List tokens for a customer  # noqa: E501
+        """Get a firewall  # noqa: E501
 
-        List all tokens belonging to a specific customer.  # noqa: E501
+        Get a specific firewall object.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_tokens_customer(customer_id, async_req=True)
+        >>> thread = api.get_waf_firewall(firewall_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            customer_id (str): Alphanumeric string identifying the customer.
+            firewall_id (str): Alphanumeric string identifying a WAF Firewall.
 
         Keyword Args:
+            filter_service_version_number (str): Limit the results returned to a specific service version.. [optional]
+            include (str): Include related objects. Optional.. [optional] if omitted the server will use the default value of "waf_firewall_versions"
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -555,15 +576,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            [TokenResponse]
+            WafFirewallResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -583,33 +604,38 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['customer_id'] = \
-            customer_id
-        return self.list_tokens_customer_endpoint.call_with_http_info(**kwargs)
+        kwargs['firewall_id'] = \
+            firewall_id
+        return self.get_waf_firewall_endpoint.call_with_http_info(**kwargs)
 
-    def list_tokens_user(
+    def list_waf_firewalls(
         self,
         **kwargs
     ):
-        """List tokens for the authenticated user  # noqa: E501
+        """List firewalls  # noqa: E501
 
-        List all tokens belonging to the authenticated user.  # noqa: E501
+        List all firewall objects.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_tokens_user(async_req=True)
+        >>> thread = api.list_waf_firewalls(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
+            page_number (int): Current page.. [optional]
+            page_size (int): Number of records per page.. [optional] if omitted the server will use the default value of 20
+            filter_service_id (str): Limit the results returned to a specific service.. [optional]
+            filter_service_version_number (str): Limit the results returned to a specific service version.. [optional]
+            include (str): Include related objects. Optional.. [optional] if omitted the server will use the default value of "waf_firewall_versions"
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -630,15 +656,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            [TokenResponse]
+            WafFirewallsResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -658,34 +684,35 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.list_tokens_user_endpoint.call_with_http_info(**kwargs)
+        return self.list_waf_firewalls_endpoint.call_with_http_info(**kwargs)
 
-    def revoke_token(
+    def update_waf_firewall(
         self,
-        token_id,
+        firewall_id,
         **kwargs
     ):
-        """Revoke a token  # noqa: E501
+        """Update a firewall  # noqa: E501
 
-        Revoke a specific token by its id.  # noqa: E501
+        Update a firewall object for a particular service and service version. Specifying a `service_version_number` is required.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.revoke_token(token_id, async_req=True)
+        >>> thread = api.update_waf_firewall(firewall_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            token_id (str): Alphanumeric string identifying a token.
+            firewall_id (str): Alphanumeric string identifying a WAF Firewall.
 
         Keyword Args:
+            waf_firewall (WafFirewall): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -706,90 +733,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            None
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['token_id'] = \
-            token_id
-        return self.revoke_token_endpoint.call_with_http_info(**kwargs)
-
-    def revoke_token_current(
-        self,
-        **kwargs
-    ):
-        """Revoke the current token  # noqa: E501
-
-        Revoke a token that is used to authenticate the request.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.revoke_token_current(async_req=True)
-        >>> result = thread.get()
-
-
-        Keyword Args:
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            None
+            WafFirewallResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -809,9 +761,11 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.revoke_token_current_endpoint.call_with_http_info(**kwargs)
+        kwargs['firewall_id'] = \
+            firewall_id
+        return self.update_waf_firewall_endpoint.call_with_http_info(**kwargs)
```

### Comparing `fastly-2.2.2/fastly/api/user_api.py` & `fastly-2.3.0/fastly/api/user_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/vcl_api.py` & `fastly-2.3.0/fastly/api/vcl_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/vcl_diff_api.py` & `fastly-2.3.0/fastly/api/vcl_diff_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/version_api.py` & `fastly-2.3.0/fastly/api/version_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/waf_active_rules_api.py` & `fastly-2.3.0/fastly/api/waf_active_rules_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/waf_exclusions_api.py` & `fastly-2.3.0/fastly/api/waf_exclusions_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/waf_firewall_versions_api.py` & `fastly-2.3.0/fastly/api/waf_firewall_versions_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/waf_rule_revisions_api.py` & `fastly-2.3.0/fastly/api/waf_rule_revisions_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/waf_rules_api.py` & `fastly-2.3.0/fastly/api/waf_rules_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/api/waf_tags_api.py` & `fastly-2.3.0/fastly/api/waf_tags_api.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/apis/__init__.py` & `fastly-2.3.0/fastly/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/acl.py` & `fastly-2.3.0/fastly/model/acl.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/acl_entry.py` & `fastly-2.3.0/fastly/model/acl_entry.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/acl_entry_response.py` & `fastly-2.3.0/fastly/model/acl_entry_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/acl_entry_response_all_of.py` & `fastly-2.3.0/fastly/model/acl_entry_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/acl_response.py` & `fastly-2.3.0/fastly/model/acl_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/acl_response_all_of.py` & `fastly-2.3.0/fastly/model/acl_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/apex_redirect.py` & `fastly-2.3.0/fastly/model/apex_redirect.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/apex_redirect_all_of.py` & `fastly-2.3.0/fastly/model/apex_redirect_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/aws_region.py` & `fastly-2.3.0/fastly/model/aws_region.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/backend.py` & `fastly-2.3.0/fastly/model/backend.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/backend_response.py` & `fastly-2.3.0/fastly/model/backend_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/backend_response_all_of.py` & `fastly-2.3.0/fastly/model/backend_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/billing.py` & `fastly-2.3.0/fastly/model/billing.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/billing_address_attributes.py` & `fastly-2.3.0/fastly/model/billing_address_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/billing_address_request.py` & `fastly-2.3.0/fastly/model/billing_address_request.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/billing_address_request_data.py` & `fastly-2.3.0/fastly/model/billing_address_request_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/billing_address_response.py` & `fastly-2.3.0/fastly/model/billing_address_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/billing_address_response_data.py` & `fastly-2.3.0/fastly/model/billing_address_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/billing_address_verification_error_response.py` & `fastly-2.3.0/fastly/model/billing_address_verification_error_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/billing_address_verification_error_response_errors.py` & `fastly-2.3.0/fastly/model/billing_address_verification_error_response_errors.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/billing_estimate_response.py` & `fastly-2.3.0/fastly/model/billing_estimate_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/billing_estimate_response_all_of.py` & `fastly-2.3.0/fastly/model/billing_estimate_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/billing_estimate_response_all_of_line.py` & `fastly-2.3.0/fastly/model/billing_estimate_response_all_of_line.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/billing_estimate_response_all_of_lines.py` & `fastly-2.3.0/fastly/model/billing_estimate_response_all_of_lines.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/billing_response.py` & `fastly-2.3.0/fastly/model/billing_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/billing_response_all_of.py` & `fastly-2.3.0/fastly/model/billing_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/billing_response_line_item.py` & `fastly-2.3.0/fastly/model/billing_response_line_item.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/billing_response_line_item_all_of.py` & `fastly-2.3.0/fastly/model/billing_response_line_item_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/billing_status.py` & `fastly-2.3.0/fastly/model/billing_status.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/billing_total.py` & `fastly-2.3.0/fastly/model/billing_total.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/billing_total_extras.py` & `fastly-2.3.0/fastly/model/billing_total_extras.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/bulk_update_acl_entries_request.py` & `fastly-2.3.0/fastly/model/bulk_update_acl_entries_request.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/bulk_update_acl_entry.py` & `fastly-2.3.0/fastly/model/bulk_update_acl_entry.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/bulk_update_acl_entry_all_of.py` & `fastly-2.3.0/fastly/model/bulk_update_acl_entry_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/bulk_update_config_store_item.py` & `fastly-2.3.0/fastly/model/bulk_update_config_store_item.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/bulk_update_config_store_item_all_of.py` & `fastly-2.3.0/fastly/model/bulk_update_config_store_item_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/bulk_update_config_store_list_request.py` & `fastly-2.3.0/fastly/model/bulk_update_config_store_list_request.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/bulk_update_dictionary_item.py` & `fastly-2.3.0/fastly/model/bulk_update_dictionary_item.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/bulk_update_dictionary_list_request.py` & `fastly-2.3.0/fastly/model/bulk_update_dictionary_list_request.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/bulk_waf_active_rule.py` & `fastly-2.3.0/fastly/model/bulk_waf_active_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/bulk_waf_active_rules.py` & `fastly-2.3.0/fastly/model/bulk_waf_active_rules.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/cache_setting.py` & `fastly-2.3.0/fastly/model/cache_setting.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/cache_setting_response.py` & `fastly-2.3.0/fastly/model/cache_setting_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/condition.py` & `fastly-2.3.0/fastly/model/condition.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/condition_response.py` & `fastly-2.3.0/fastly/model/condition_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/conditions_response.py` & `fastly-2.3.0/fastly/model/conditions_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/config_store.py` & `fastly-2.3.0/fastly/model/config_store.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/config_store_info_response.py` & `fastly-2.3.0/fastly/model/config_store_info_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/config_store_item.py` & `fastly-2.3.0/fastly/model/config_store_item.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/config_store_item_response.py` & `fastly-2.3.0/fastly/model/config_store_item_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/config_store_item_response_all_of.py` & `fastly-2.3.0/fastly/model/config_store_item_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/config_store_response.py` & `fastly-2.3.0/fastly/model/config_store_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/config_store_response_all_of.py` & `fastly-2.3.0/fastly/model/config_store_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/contact.py` & `fastly-2.3.0/fastly/model/contact.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/contact_response.py` & `fastly-2.3.0/fastly/model/contact_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/contact_response_all_of.py` & `fastly-2.3.0/fastly/model/contact_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/content.py` & `fastly-2.3.0/fastly/model/content.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/customer.py` & `fastly-2.3.0/fastly/model/customer.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/customer_response.py` & `fastly-2.3.0/fastly/model/customer_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/customer_response_all_of.py` & `fastly-2.3.0/fastly/model/customer_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/dictionary.py` & `fastly-2.3.0/fastly/model/dictionary.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/dictionary_info_response.py` & `fastly-2.3.0/fastly/model/dictionary_info_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/dictionary_item.py` & `fastly-2.3.0/fastly/model/dictionary_item.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/dictionary_item_response.py` & `fastly-2.3.0/fastly/model/dictionary_item_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/dictionary_item_response_all_of.py` & `fastly-2.3.0/fastly/model/dictionary_item_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/dictionary_response.py` & `fastly-2.3.0/fastly/model/dictionary_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/dictionary_response_all_of.py` & `fastly-2.3.0/fastly/model/dictionary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/diff_response.py` & `fastly-2.3.0/fastly/model/diff_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/director.py` & `fastly-2.3.0/fastly/model/director.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/director_backend.py` & `fastly-2.3.0/fastly/model/director_backend.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/director_backend_all_of.py` & `fastly-2.3.0/fastly/model/director_backend_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/director_response.py` & `fastly-2.3.0/fastly/model/director_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/domain.py` & `fastly-2.3.0/fastly/model/domain.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/domain_check_item.py` & `fastly-2.3.0/fastly/model/domain_check_item.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/domain_check_response.py` & `fastly-2.3.0/fastly/model/domain_check_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/domain_check_response_list.py` & `fastly-2.3.0/fastly/model/domain_check_response_list.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/domain_response.py` & `fastly-2.3.0/fastly/model/domain_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/domains_response.py` & `fastly-2.3.0/fastly/model/domains_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/enabled_product_response.py` & `fastly-2.3.0/fastly/model/enabled_product_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/enabled_product_response_links.py` & `fastly-2.3.0/fastly/model/enabled_product_response_links.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/enabled_product_response_product.py` & `fastly-2.3.0/fastly/model/enabled_product_response_product.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/enabled_product_response_service.py` & `fastly-2.3.0/fastly/model/enabled_product_response_service.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/event.py` & `fastly-2.3.0/fastly/model/event.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/event_attributes.py` & `fastly-2.3.0/fastly/model/event_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/event_response.py` & `fastly-2.3.0/fastly/model/event_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/events_response.py` & `fastly-2.3.0/fastly/model/events_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/events_response_all_of.py` & `fastly-2.3.0/fastly/model/events_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/generic_token_error.py` & `fastly-2.3.0/fastly/model/generic_token_error.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/gzip.py` & `fastly-2.3.0/fastly/model/gzip.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/gzip_response.py` & `fastly-2.3.0/fastly/model/gzip_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/header.py` & `fastly-2.3.0/fastly/model/header.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/header_response.py` & `fastly-2.3.0/fastly/model/header_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/healthcheck.py` & `fastly-2.3.0/fastly/model/healthcheck.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/healthcheck_response.py` & `fastly-2.3.0/fastly/model/healthcheck_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical.py` & `fastly-2.3.0/fastly/model/historical.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_aggregate_response.py` & `fastly-2.3.0/fastly/model/historical_aggregate_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_aggregate_response_all_of.py` & `fastly-2.3.0/fastly/model/historical_aggregate_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_field_aggregate_response.py` & `fastly-2.3.0/fastly/model/historical_field_aggregate_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_field_aggregate_response_all_of.py` & `fastly-2.3.0/fastly/model/historical_field_aggregate_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_field_response.py` & `fastly-2.3.0/fastly/model/historical_field_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_field_response_data_field.py` & `fastly-2.3.0/fastly/model/historical_field_response_data_field.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_field_results.py` & `fastly-2.3.0/fastly/model/historical_field_results.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_field_results_attributes.py` & `fastly-2.3.0/fastly/model/historical_field_results_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,18 @@
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from fastly.model.historical_field_results_attributes_all_of import HistoricalFieldResultsAttributesAllOf
+    from fastly.model.read_only_id_service import ReadOnlyIdService
     from fastly.model.results import Results
     globals()['HistoricalFieldResultsAttributesAllOf'] = HistoricalFieldResultsAttributesAllOf
+    globals()['ReadOnlyIdService'] = ReadOnlyIdService
     globals()['Results'] = Results
 
 
 class HistoricalFieldResultsAttributes(ModelComposed):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
@@ -299,15 +301,15 @@
             'fanout_conn_time_ms': (int,),  # noqa: E501
             'ddos_action_limit_streams_connections': (int,),  # noqa: E501
             'ddos_action_limit_streams_requests': (int,),  # noqa: E501
             'ddos_action_tarpit_accept': (int,),  # noqa: E501
             'ddos_action_tarpit': (int,),  # noqa: E501
             'ddos_action_close': (int,),  # noqa: E501
             'ddos_action_blackhole': (int,),  # noqa: E501
-            'service_id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'service_id': (ReadOnlyIdService,),  # noqa: E501
             'start_time': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -530,15 +532,14 @@
         'ddos_action_close': 'ddos_action_close',  # noqa: E501
         'ddos_action_blackhole': 'ddos_action_blackhole',  # noqa: E501
         'service_id': 'service_id',  # noqa: E501
         'start_time': 'start_time',  # noqa: E501
     }
 
     read_only_vars = {
-        'service_id',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """HistoricalFieldResultsAttributes - a model defined in OpenAPI
 
@@ -785,15 +786,15 @@
             fanout_conn_time_ms (int): Total duration of Fanout connections with end users.. [optional]  # noqa: E501
             ddos_action_limit_streams_connections (int): For HTTP/2, the number of connections the limit-streams action was applied to. The limit-streams action caps the allowed number of concurrent streams in a connection.. [optional]  # noqa: E501
             ddos_action_limit_streams_requests (int): For HTTP/2, the number of requests made on a connection for which the limit-streams action was taken. The limit-streams action caps the allowed number of concurrent streams in a connection.. [optional]  # noqa: E501
             ddos_action_tarpit_accept (int): The number of times the tarpit-accept action was taken. The tarpit-accept action adds a delay when accepting future connections.. [optional]  # noqa: E501
             ddos_action_tarpit (int): The number of times the tarpit action was taken. The tarpit action delays writing the response to the client.. [optional]  # noqa: E501
             ddos_action_close (int): The number of times the close action was taken. The close action aborts the connection as soon as possible. The close action takes effect either right after accept, right after the client hello, or right after the response was sent.. [optional]  # noqa: E501
             ddos_action_blackhole (int): The number of times the blackhole action was taken. The blackhole action quietly closes a TCP connection without sending a reset. The blackhole action quietly closes a TCP connection without notifying its peer (all TCP state is dropped).. [optional]  # noqa: E501
-            service_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            service_id (ReadOnlyIdService): [optional]  # noqa: E501
             start_time (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -1102,15 +1103,15 @@
             fanout_conn_time_ms (int): Total duration of Fanout connections with end users.. [optional]  # noqa: E501
             ddos_action_limit_streams_connections (int): For HTTP/2, the number of connections the limit-streams action was applied to. The limit-streams action caps the allowed number of concurrent streams in a connection.. [optional]  # noqa: E501
             ddos_action_limit_streams_requests (int): For HTTP/2, the number of requests made on a connection for which the limit-streams action was taken. The limit-streams action caps the allowed number of concurrent streams in a connection.. [optional]  # noqa: E501
             ddos_action_tarpit_accept (int): The number of times the tarpit-accept action was taken. The tarpit-accept action adds a delay when accepting future connections.. [optional]  # noqa: E501
             ddos_action_tarpit (int): The number of times the tarpit action was taken. The tarpit action delays writing the response to the client.. [optional]  # noqa: E501
             ddos_action_close (int): The number of times the close action was taken. The close action aborts the connection as soon as possible. The close action takes effect either right after accept, right after the client hello, or right after the response was sent.. [optional]  # noqa: E501
             ddos_action_blackhole (int): The number of times the blackhole action was taken. The blackhole action quietly closes a TCP connection without sending a reset. The blackhole action quietly closes a TCP connection without notifying its peer (all TCP state is dropped).. [optional]  # noqa: E501
-            service_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            service_id (ReadOnlyIdService): [optional]  # noqa: E501
             start_time (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `fastly-2.2.2/fastly/model/historical_field_results_attributes_all_of.py` & `fastly-2.3.0/fastly/model/server_response_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class HistoricalFieldResultsAttributesAllOf(ModelNormal):
+class ServerResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -75,38 +75,42 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'service_id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'start_time': (int,),  # noqa: E501
+            'service_id': (str,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'pool_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'service_id': 'service_id',  # noqa: E501
-        'start_time': 'start_time',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'pool_id': 'pool_id',  # noqa: E501
     }
 
     read_only_vars = {
         'service_id',  # noqa: E501
+        'id',  # noqa: E501
+        'pool_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """HistoricalFieldResultsAttributesAllOf - a model defined in OpenAPI
+        """ServerResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -131,16 +135,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            service_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            start_time (int): [optional]  # noqa: E501
+            service_id (str): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            pool_id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -181,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """HistoricalFieldResultsAttributesAllOf - a model defined in OpenAPI
+        """ServerResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -214,16 +219,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            service_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            start_time (int): [optional]  # noqa: E501
+            service_id (str): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            pool_id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-2.2.2/fastly/model/historical_meta.py` & `fastly-2.3.0/fastly/model/historical_meta.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_regions_response.py` & `fastly-2.3.0/fastly/model/historical_regions_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_regions_response_all_of.py` & `fastly-2.3.0/fastly/model/historical_regions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_response.py` & `fastly-2.3.0/fastly/model/historical_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_response_data_field.py` & `fastly-2.3.0/fastly/model/historical_response_data_field.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_results.py` & `fastly-2.3.0/fastly/model/historical_results.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_service.py` & `fastly-2.3.0/fastly/model/historical_service.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_services.py` & `fastly-2.3.0/fastly/model/historical_services.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_usage_aggregate_response.py` & `fastly-2.3.0/fastly/model/historical_usage_aggregate_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_usage_month_response.py` & `fastly-2.3.0/fastly/model/historical_usage_month_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_usage_month_response_all_of.py` & `fastly-2.3.0/fastly/model/historical_usage_month_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_usage_month_response_data.py` & `fastly-2.3.0/fastly/model/historical_usage_month_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_usage_results.py` & `fastly-2.3.0/fastly/model/historical_usage_results.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_usage_service_response.py` & `fastly-2.3.0/fastly/model/historical_usage_service_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/historical_usage_service_response_all_of.py` & `fastly-2.3.0/fastly/model/historical_usage_service_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/http3.py` & `fastly-2.3.0/fastly/model/http3.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/http3_all_of.py` & `fastly-2.3.0/fastly/model/http3_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/http_response_format.py` & `fastly-2.3.0/fastly/model/http_response_format.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/http_stream_format.py` & `fastly-2.3.0/fastly/model/http_stream_format.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/iam_permission.py` & `fastly-2.3.0/fastly/model/iam_permission.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/iam_role.py` & `fastly-2.3.0/fastly/model/iam_role.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/iam_role_all_of.py` & `fastly-2.3.0/fastly/model/iam_role_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/iam_service_group.py` & `fastly-2.3.0/fastly/model/iam_service_group.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/iam_service_group_all_of.py` & `fastly-2.3.0/fastly/model/iam_service_group_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/iam_user_group.py` & `fastly-2.3.0/fastly/model/iam_user_group.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/iam_user_group_all_of.py` & `fastly-2.3.0/fastly/model/iam_user_group_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/included_with_waf_active_rule.py` & `fastly-2.3.0/fastly/model/included_with_waf_active_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/included_with_waf_active_rule_item.py` & `fastly-2.3.0/fastly/model/included_with_waf_active_rule_item.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/included_with_waf_exclusion.py` & `fastly-2.3.0/fastly/model/included_with_waf_exclusion.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/included_with_waf_exclusion_item.py` & `fastly-2.3.0/fastly/model/included_with_waf_exclusion_item.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/included_with_waf_firewall.py` & `fastly-2.3.0/fastly/model/included_with_waf_firewall.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/included_with_waf_firewall_version.py` & `fastly-2.3.0/fastly/model/included_with_waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/included_with_waf_firewall_version_item.py` & `fastly-2.3.0/fastly/model/included_with_waf_firewall_version_item.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/included_with_waf_rule.py` & `fastly-2.3.0/fastly/model/included_with_waf_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/included_with_waf_rule_item.py` & `fastly-2.3.0/fastly/model/included_with_waf_rule_item.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/included_with_waf_rule_revision.py` & `fastly-2.3.0/fastly/model/included_with_waf_rule_revision.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/inline_object.py` & `fastly-2.3.0/fastly/model/inline_object.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/inline_object1.py` & `fastly-2.3.0/fastly/model/inline_object1.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/inline_response200.py` & `fastly-2.3.0/fastly/model/inline_response200.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/inline_response2001.py` & `fastly-2.3.0/fastly/model/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/inline_response2002.py` & `fastly-2.3.0/fastly/model/inline_response2002.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/inline_response2002_meta.py` & `fastly-2.3.0/fastly/model/inline_response2002_meta.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/inline_response2003.py` & `fastly-2.3.0/fastly/model/inline_response2003.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/inline_response2003_meta.py` & `fastly-2.3.0/fastly/model/inline_response2003_meta.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/invitation.py` & `fastly-2.3.0/fastly/model/invitation.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/invitation_data.py` & `fastly-2.3.0/fastly/model/invitation_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/invitation_data_attributes.py` & `fastly-2.3.0/fastly/model/invitation_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/invitation_response.py` & `fastly-2.3.0/fastly/model/invitation_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/invitation_response_all_of.py` & `fastly-2.3.0/fastly/model/invitation_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/invitation_response_data.py` & `fastly-2.3.0/fastly/model/invitation_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/invitation_response_data_all_of.py` & `fastly-2.3.0/fastly/model/invitation_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/invitations_response.py` & `fastly-2.3.0/fastly/model/invitations_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/invitations_response_all_of.py` & `fastly-2.3.0/fastly/model/invitations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_address_and_port.py` & `fastly-2.3.0/fastly/model/logging_address_and_port.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_azureblob.py` & `fastly-2.3.0/fastly/model/logging_azureblob.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_azureblob_all_of.py` & `fastly-2.3.0/fastly/model/logging_azureblob_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_azureblob_response.py` & `fastly-2.3.0/fastly/model/logging_azureblob_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_bigquery.py` & `fastly-2.3.0/fastly/model/logging_bigquery.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_bigquery_all_of.py` & `fastly-2.3.0/fastly/model/logging_bigquery_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_bigquery_response.py` & `fastly-2.3.0/fastly/model/logging_bigquery_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_cloudfiles.py` & `fastly-2.3.0/fastly/model/logging_cloudfiles.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_cloudfiles_all_of.py` & `fastly-2.3.0/fastly/model/logging_cloudfiles_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_cloudfiles_response.py` & `fastly-2.3.0/fastly/model/logging_cloudfiles_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_common.py` & `fastly-2.3.0/fastly/model/logging_common.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_datadog.py` & `fastly-2.3.0/fastly/model/logging_datadog.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_datadog_all_of.py` & `fastly-2.3.0/fastly/model/logging_datadog_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_datadog_response.py` & `fastly-2.3.0/fastly/model/logging_datadog_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_digitalocean.py` & `fastly-2.3.0/fastly/model/logging_digitalocean.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_digitalocean_all_of.py` & `fastly-2.3.0/fastly/model/logging_digitalocean_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_digitalocean_response.py` & `fastly-2.3.0/fastly/model/logging_digitalocean_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_elasticsearch.py` & `fastly-2.3.0/fastly/model/logging_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_elasticsearch_all_of.py` & `fastly-2.3.0/fastly/model/logging_elasticsearch_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_elasticsearch_response.py` & `fastly-2.3.0/fastly/model/logging_elasticsearch_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_format_version.py` & `fastly-2.3.0/fastly/model/logging_format_version.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_ftp.py` & `fastly-2.3.0/fastly/model/logging_ftp.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_ftp_all_of.py` & `fastly-2.3.0/fastly/model/logging_ftp_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_ftp_response.py` & `fastly-2.3.0/fastly/model/logging_ftp_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_gcs.py` & `fastly-2.3.0/fastly/model/logging_gcs.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_gcs_all_of.py` & `fastly-2.3.0/fastly/model/logging_gcs_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_gcs_common.py` & `fastly-2.3.0/fastly/model/logging_gcs_common.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_gcs_response.py` & `fastly-2.3.0/fastly/model/logging_gcs_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_generic_common.py` & `fastly-2.3.0/fastly/model/logging_generic_common.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_google_pubsub.py` & `fastly-2.3.0/fastly/model/logging_google_pubsub.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_google_pubsub_all_of.py` & `fastly-2.3.0/fastly/model/logging_google_pubsub_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_google_pubsub_response.py` & `fastly-2.3.0/fastly/model/logging_google_pubsub_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_heroku.py` & `fastly-2.3.0/fastly/model/logging_heroku.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_heroku_all_of.py` & `fastly-2.3.0/fastly/model/logging_heroku_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_heroku_response.py` & `fastly-2.3.0/fastly/model/logging_heroku_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_honeycomb.py` & `fastly-2.3.0/fastly/model/logging_honeycomb.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_honeycomb_all_of.py` & `fastly-2.3.0/fastly/model/logging_honeycomb_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_honeycomb_response.py` & `fastly-2.3.0/fastly/model/logging_honeycomb_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_https.py` & `fastly-2.3.0/fastly/model/logging_https.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_https_all_of.py` & `fastly-2.3.0/fastly/model/logging_https_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_https_response.py` & `fastly-2.3.0/fastly/model/logging_https_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_kafka.py` & `fastly-2.3.0/fastly/model/logging_kafka.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_kafka_all_of.py` & `fastly-2.3.0/fastly/model/logging_kafka_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_kafka_response.py` & `fastly-2.3.0/fastly/model/logging_kafka_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_kinesis.py` & `fastly-2.3.0/fastly/model/logging_kinesis.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_kinesis_response.py` & `fastly-2.3.0/fastly/model/logging_kinesis_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_logentries.py` & `fastly-2.3.0/fastly/model/logging_logentries.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_logentries_all_of.py` & `fastly-2.3.0/fastly/model/logging_logentries_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_logentries_response.py` & `fastly-2.3.0/fastly/model/logging_logentries_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_loggly.py` & `fastly-2.3.0/fastly/model/logging_loggly.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_loggly_all_of.py` & `fastly-2.3.0/fastly/model/logging_loggly_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_loggly_response.py` & `fastly-2.3.0/fastly/model/logging_loggly_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_logshuttle.py` & `fastly-2.3.0/fastly/model/logging_logshuttle.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_logshuttle_all_of.py` & `fastly-2.3.0/fastly/model/logging_logshuttle_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_logshuttle_response.py` & `fastly-2.3.0/fastly/model/logging_logshuttle_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_message_type.py` & `fastly-2.3.0/fastly/model/logging_message_type.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_newrelic.py` & `fastly-2.3.0/fastly/model/logging_newrelic.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_newrelic_all_of.py` & `fastly-2.3.0/fastly/model/logging_newrelic_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_newrelic_response.py` & `fastly-2.3.0/fastly/model/logging_newrelic_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_openstack.py` & `fastly-2.3.0/fastly/model/logging_openstack.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_openstack_all_of.py` & `fastly-2.3.0/fastly/model/logging_openstack_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_openstack_response.py` & `fastly-2.3.0/fastly/model/logging_openstack_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_papertrail.py` & `fastly-2.3.0/fastly/model/logging_papertrail.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_papertrail_response.py` & `fastly-2.3.0/fastly/model/logging_papertrail_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_placement.py` & `fastly-2.3.0/fastly/model/logging_placement.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_request_caps_common.py` & `fastly-2.3.0/fastly/model/logging_request_caps_common.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_s3.py` & `fastly-2.3.0/fastly/model/logging_s3.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_s3_all_of.py` & `fastly-2.3.0/fastly/model/logging_s3_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_s3_response.py` & `fastly-2.3.0/fastly/model/logging_s3_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_scalyr.py` & `fastly-2.3.0/fastly/model/logging_scalyr.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_scalyr_all_of.py` & `fastly-2.3.0/fastly/model/logging_scalyr_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_scalyr_response.py` & `fastly-2.3.0/fastly/model/logging_scalyr_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_sftp.py` & `fastly-2.3.0/fastly/model/logging_sftp.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_sftp_all_of.py` & `fastly-2.3.0/fastly/model/logging_sftp_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_sftp_response.py` & `fastly-2.3.0/fastly/model/logging_sftp_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_splunk.py` & `fastly-2.3.0/fastly/model/logging_splunk.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_splunk_all_of.py` & `fastly-2.3.0/fastly/model/logging_splunk_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_splunk_response.py` & `fastly-2.3.0/fastly/model/logging_splunk_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_sumologic.py` & `fastly-2.3.0/fastly/model/logging_sumologic.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_sumologic_all_of.py` & `fastly-2.3.0/fastly/model/logging_sumologic_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_sumologic_response.py` & `fastly-2.3.0/fastly/model/logging_sumologic_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_syslog.py` & `fastly-2.3.0/fastly/model/logging_syslog.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_syslog_all_of.py` & `fastly-2.3.0/fastly/model/logging_syslog_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_syslog_response.py` & `fastly-2.3.0/fastly/model/logging_syslog_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_tls_common.py` & `fastly-2.3.0/fastly/model/logging_tls_common.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/logging_use_tls.py` & `fastly-2.3.0/fastly/model/logging_use_tls.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/mutual_authentication.py` & `fastly-2.3.0/fastly/model/mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/mutual_authentication_data.py` & `fastly-2.3.0/fastly/model/mutual_authentication_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/mutual_authentication_data_attributes.py` & `fastly-2.3.0/fastly/model/mutual_authentication_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/mutual_authentication_response.py` & `fastly-2.3.0/fastly/model/mutual_authentication_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/mutual_authentication_response_attributes.py` & `fastly-2.3.0/fastly/model/mutual_authentication_response_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/mutual_authentication_response_attributes_all_of.py` & `fastly-2.3.0/fastly/model/mutual_authentication_response_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/mutual_authentication_response_data.py` & `fastly-2.3.0/fastly/model/mutual_authentication_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/mutual_authentication_response_data_all_of.py` & `fastly-2.3.0/fastly/model/mutual_authentication_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/mutual_authentications_response.py` & `fastly-2.3.0/fastly/model/mutual_authentications_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/mutual_authentications_response_all_of.py` & `fastly-2.3.0/fastly/model/mutual_authentications_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/number_version.py` & `fastly-2.3.0/fastly/model/number_version.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/package.py` & `fastly-2.3.0/fastly/model/package.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/package_metadata.py` & `fastly-2.3.0/fastly/model/package_metadata.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/package_response.py` & `fastly-2.3.0/fastly/model/package_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/package_response_all_of.py` & `fastly-2.3.0/fastly/model/package_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/pagination.py` & `fastly-2.3.0/fastly/model/pagination.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/pagination_links.py` & `fastly-2.3.0/fastly/model/pagination_links.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/pagination_meta.py` & `fastly-2.3.0/fastly/model/pagination_meta.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/permission.py` & `fastly-2.3.0/fastly/model/permission.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/pool.py` & `fastly-2.3.0/fastly/model/pool.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/pool_all_of.py` & `fastly-2.3.0/fastly/model/pool_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/pool_response.py` & `fastly-2.3.0/fastly/model/pool_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/pool_response_all_of.py` & `fastly-2.3.0/fastly/model/pool_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/pop.py` & `fastly-2.3.0/fastly/model/pop.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/pop_coordinates.py` & `fastly-2.3.0/fastly/model/pop_coordinates.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/public_ip_list.py` & `fastly-2.3.0/fastly/model/public_ip_list.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/publish_item.py` & `fastly-2.3.0/fastly/model/publish_item.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/publish_item_formats.py` & `fastly-2.3.0/fastly/model/publish_item_formats.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/publish_request.py` & `fastly-2.3.0/fastly/model/publish_request.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/purge_keys.py` & `fastly-2.3.0/fastly/model/purge_keys.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/purge_keys_response.py` & `fastly-2.3.0/fastly/model/purge_keys_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/purge_response.py` & `fastly-2.3.0/fastly/model/purge_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/rate_limiter.py` & `fastly-2.3.0/fastly/model/rate_limiter.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,14 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from fastly.model.rate_limiter_response1 import RateLimiterResponse1
-    globals()['RateLimiterResponse1'] = RateLimiterResponse1
-
 
 class RateLimiter(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -144,40 +140,38 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'uri_dictionary_name': (str, none_type,),  # noqa: E501
             'http_methods': ([str],),  # noqa: E501
             'rps_limit': (int,),  # noqa: E501
             'window_size': (int,),  # noqa: E501
             'client_key': ([str],),  # noqa: E501
             'penalty_box_duration': (int,),  # noqa: E501
             'action': (str,),  # noqa: E501
-            'response': (RateLimiterResponse1,),  # noqa: E501
+            'response': ({str: (str,)}, none_type,),  # noqa: E501
             'response_object_name': (str, none_type,),  # noqa: E501
             'logger_type': (str,),  # noqa: E501
             'feature_revision': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
@@ -244,15 +238,15 @@
             uri_dictionary_name (str, none_type): The name of an Edge Dictionary containing URIs as keys. If not defined or `null`, all origin URIs will be rate limited.. [optional]  # noqa: E501
             http_methods ([str]): Array of HTTP methods to apply rate limiting to.. [optional]  # noqa: E501
             rps_limit (int): Upper limit of requests per second allowed by the rate limiter.. [optional]  # noqa: E501
             window_size (int): Number of seconds during which the RPS limit must be exceeded in order to trigger a violation.. [optional]  # noqa: E501
             client_key ([str]): Array of VCL variables used to generate a counter key to identify a client. Example variables include `req.http.Fastly-Client-IP`, `req.http.User-Agent`, or a custom header like `req.http.API-Key`.. [optional]  # noqa: E501
             penalty_box_duration (int): Length of time in minutes that the rate limiter is in effect after the initial violation is detected.. [optional]  # noqa: E501
             action (str): The action to take when a rate limiter violation is detected.. [optional]  # noqa: E501
-            response (RateLimiterResponse1): [optional]  # noqa: E501
+            response ({str: (str,)}, none_type): Custom response to be sent when the rate limit is exceeded. Required if `action` is `response`.. [optional]  # noqa: E501
             response_object_name (str, none_type): Name of existing response object. Required if `action` is `response_object`. Note that the rate limiter response is only updated to reflect the response object content when saving the rate limiter configuration.. [optional]  # noqa: E501
             logger_type (str): Name of the type of logging endpoint to be used when action is `log_only`. The logging endpoint type is used to determine the appropriate log format to use when emitting log entries.. [optional]  # noqa: E501
             feature_revision (int): Revision number of the rate limiting feature implementation. Defaults to the most recent revision.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -337,15 +331,15 @@
             uri_dictionary_name (str, none_type): The name of an Edge Dictionary containing URIs as keys. If not defined or `null`, all origin URIs will be rate limited.. [optional]  # noqa: E501
             http_methods ([str]): Array of HTTP methods to apply rate limiting to.. [optional]  # noqa: E501
             rps_limit (int): Upper limit of requests per second allowed by the rate limiter.. [optional]  # noqa: E501
             window_size (int): Number of seconds during which the RPS limit must be exceeded in order to trigger a violation.. [optional]  # noqa: E501
             client_key ([str]): Array of VCL variables used to generate a counter key to identify a client. Example variables include `req.http.Fastly-Client-IP`, `req.http.User-Agent`, or a custom header like `req.http.API-Key`.. [optional]  # noqa: E501
             penalty_box_duration (int): Length of time in minutes that the rate limiter is in effect after the initial violation is detected.. [optional]  # noqa: E501
             action (str): The action to take when a rate limiter violation is detected.. [optional]  # noqa: E501
-            response (RateLimiterResponse1): [optional]  # noqa: E501
+            response ({str: (str,)}, none_type): Custom response to be sent when the rate limit is exceeded. Required if `action` is `response`.. [optional]  # noqa: E501
             response_object_name (str, none_type): Name of existing response object. Required if `action` is `response_object`. Note that the rate limiter response is only updated to reflect the response object content when saving the rate limiter configuration.. [optional]  # noqa: E501
             logger_type (str): Name of the type of logging endpoint to be used when action is `log_only`. The logging endpoint type is used to determine the appropriate log format to use when emitting log entries.. [optional]  # noqa: E501
             feature_revision (int): Revision number of the rate limiting feature implementation. Defaults to the most recent revision.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `fastly-2.2.2/fastly/model/rate_limiter_response.py` & `fastly-2.3.0/fastly/model/rate_limiter_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,20 +27,18 @@
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from fastly.model.rate_limiter import RateLimiter
-    from fastly.model.rate_limiter_response1 import RateLimiterResponse1
     from fastly.model.rate_limiter_response_all_of import RateLimiterResponseAllOf
     from fastly.model.service_id_and_version import ServiceIdAndVersion
     from fastly.model.timestamps import Timestamps
     globals()['RateLimiter'] = RateLimiter
-    globals()['RateLimiterResponse1'] = RateLimiterResponse1
     globals()['RateLimiterResponseAllOf'] = RateLimiterResponseAllOf
     globals()['ServiceIdAndVersion'] = ServiceIdAndVersion
     globals()['Timestamps'] = Timestamps
 
 
 class RateLimiterResponse(ModelComposed):
     """NOTE: This class is auto generated.
@@ -177,15 +175,15 @@
             'uri_dictionary_name': (str, none_type,),  # noqa: E501
             'http_methods': ([str],),  # noqa: E501
             'rps_limit': (int,),  # noqa: E501
             'window_size': (int,),  # noqa: E501
             'client_key': ([str],),  # noqa: E501
             'penalty_box_duration': (int,),  # noqa: E501
             'action': (str,),  # noqa: E501
-            'response': (RateLimiterResponse1,),  # noqa: E501
+            'response': ({str: (str,)}, none_type,),  # noqa: E501
             'response_object_name': (str, none_type,),  # noqa: E501
             'logger_type': (str,),  # noqa: E501
             'feature_revision': (int,),  # noqa: E501
             'service_id': (str,),  # noqa: E501
             'version': (int,),  # noqa: E501
             'created_at': (datetime, none_type,),  # noqa: E501
             'deleted_at': (datetime, none_type,),  # noqa: E501
@@ -267,15 +265,15 @@
             uri_dictionary_name (str, none_type): The name of an Edge Dictionary containing URIs as keys. If not defined or `null`, all origin URIs will be rate limited.. [optional]  # noqa: E501
             http_methods ([str]): Array of HTTP methods to apply rate limiting to.. [optional]  # noqa: E501
             rps_limit (int): Upper limit of requests per second allowed by the rate limiter.. [optional]  # noqa: E501
             window_size (int): Number of seconds during which the RPS limit must be exceeded in order to trigger a violation.. [optional]  # noqa: E501
             client_key ([str]): Array of VCL variables used to generate a counter key to identify a client. Example variables include `req.http.Fastly-Client-IP`, `req.http.User-Agent`, or a custom header like `req.http.API-Key`.. [optional]  # noqa: E501
             penalty_box_duration (int): Length of time in minutes that the rate limiter is in effect after the initial violation is detected.. [optional]  # noqa: E501
             action (str): The action to take when a rate limiter violation is detected.. [optional]  # noqa: E501
-            response (RateLimiterResponse1): [optional]  # noqa: E501
+            response ({str: (str,)}, none_type): Custom response to be sent when the rate limit is exceeded. Required if `action` is `response`.. [optional]  # noqa: E501
             response_object_name (str, none_type): Name of existing response object. Required if `action` is `response_object`. Note that the rate limiter response is only updated to reflect the response object content when saving the rate limiter configuration.. [optional]  # noqa: E501
             logger_type (str): Name of the type of logging endpoint to be used when action is `log_only`. The logging endpoint type is used to determine the appropriate log format to use when emitting log entries.. [optional]  # noqa: E501
             feature_revision (int): Revision number of the rate limiting feature implementation. Defaults to the most recent revision.. [optional]  # noqa: E501
             service_id (str): [optional]  # noqa: E501
             version (int): [optional]  # noqa: E501
             created_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             deleted_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
@@ -384,15 +382,15 @@
             uri_dictionary_name (str, none_type): The name of an Edge Dictionary containing URIs as keys. If not defined or `null`, all origin URIs will be rate limited.. [optional]  # noqa: E501
             http_methods ([str]): Array of HTTP methods to apply rate limiting to.. [optional]  # noqa: E501
             rps_limit (int): Upper limit of requests per second allowed by the rate limiter.. [optional]  # noqa: E501
             window_size (int): Number of seconds during which the RPS limit must be exceeded in order to trigger a violation.. [optional]  # noqa: E501
             client_key ([str]): Array of VCL variables used to generate a counter key to identify a client. Example variables include `req.http.Fastly-Client-IP`, `req.http.User-Agent`, or a custom header like `req.http.API-Key`.. [optional]  # noqa: E501
             penalty_box_duration (int): Length of time in minutes that the rate limiter is in effect after the initial violation is detected.. [optional]  # noqa: E501
             action (str): The action to take when a rate limiter violation is detected.. [optional]  # noqa: E501
-            response (RateLimiterResponse1): [optional]  # noqa: E501
+            response ({str: (str,)}, none_type): Custom response to be sent when the rate limit is exceeded. Required if `action` is `response`.. [optional]  # noqa: E501
             response_object_name (str, none_type): Name of existing response object. Required if `action` is `response_object`. Note that the rate limiter response is only updated to reflect the response object content when saving the rate limiter configuration.. [optional]  # noqa: E501
             logger_type (str): Name of the type of logging endpoint to be used when action is `log_only`. The logging endpoint type is used to determine the appropriate log format to use when emitting log entries.. [optional]  # noqa: E501
             feature_revision (int): Revision number of the rate limiting feature implementation. Defaults to the most recent revision.. [optional]  # noqa: E501
             service_id (str): [optional]  # noqa: E501
             version (int): [optional]  # noqa: E501
             created_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             deleted_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
```

### Comparing `fastly-2.2.2/fastly/model/rate_limiter_response1.py` & `fastly-2.3.0/fastly/model/store_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class RateLimiterResponse1(ModelNormal):
+class StoreResponse(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -52,72 +52,60 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('status',): {
-            'inclusive_maximum': 999,
-            'inclusive_minimum': 100,
-        },
-        ('content_type',): {
-            'min_length': 1,
-        },
-        ('content',): {
-            'min_length': 1,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
-    _nullable = True
+    _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'status': (int,),  # noqa: E501
-            'content_type': (str,),  # noqa: E501
-            'content': (str,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'status': 'status',  # noqa: E501
-        'content_type': 'content_type',  # noqa: E501
-        'content': 'content',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RateLimiterResponse1 - a model defined in OpenAPI
+        """StoreResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,17 +130,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            status (int): HTTP status code for custom limit enforcement response.. [optional]  # noqa: E501
-            content_type (str): MIME type for custom limit enforcement response.. [optional]  # noqa: E501
-            content (str): Response body for custom limit enforcement response.. [optional]  # noqa: E501
+            id (str): ID of the store.. [optional]  # noqa: E501
+            name (str): A human-readable name for the store.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -193,15 +180,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """RateLimiterResponse1 - a model defined in OpenAPI
+        """StoreResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,17 +213,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            status (int): HTTP status code for custom limit enforcement response.. [optional]  # noqa: E501
-            content_type (str): MIME type for custom limit enforcement response.. [optional]  # noqa: E501
-            content (str): Response body for custom limit enforcement response.. [optional]  # noqa: E501
+            id (str): ID of the store.. [optional]  # noqa: E501
+            name (str): A human-readable name for the store.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-2.2.2/fastly/model/rate_limiter_response_all_of.py` & `fastly-2.3.0/fastly/model/rate_limiter_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/realtime.py` & `fastly-2.3.0/fastly/model/realtime.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/realtime_entry.py` & `fastly-2.3.0/fastly/model/realtime_entry.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/realtime_measurements.py` & `fastly-2.3.0/fastly/model/realtime_measurements.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_common_name.py` & `fastly-2.3.0/fastly/model/relationship_common_name.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_customer.py` & `fastly-2.3.0/fastly/model/relationship_customer.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_customer_customer.py` & `fastly-2.3.0/fastly/model/relationship_customer_customer.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_member_customer.py` & `fastly-2.3.0/fastly/model/relationship_member_customer.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_member_mutual_authentication.py` & `fastly-2.3.0/fastly/model/relationship_member_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_member_service.py` & `fastly-2.3.0/fastly/model/relationship_member_service.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_member_service_invitation.py` & `fastly-2.3.0/fastly/model/relationship_member_service_invitation.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_member_tls_activation.py` & `fastly-2.3.0/fastly/model/relationship_member_tls_activation.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_member_tls_bulk_certificate.py` & `fastly-2.3.0/fastly/model/relationship_member_tls_bulk_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_member_tls_certificate.py` & `fastly-2.3.0/fastly/model/relationship_member_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_member_tls_configuration.py` & `fastly-2.3.0/fastly/model/relationship_member_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_member_tls_dns_record.py` & `fastly-2.3.0/fastly/model/relationship_member_tls_dns_record.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_member_tls_domain.py` & `fastly-2.3.0/fastly/model/relationship_member_tls_domain.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_member_tls_private_key.py` & `fastly-2.3.0/fastly/model/relationship_member_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_member_tls_subscription.py` & `fastly-2.3.0/fastly/model/relationship_member_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_member_waf_active_rule.py` & `fastly-2.3.0/fastly/model/relationship_member_waf_active_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_member_waf_firewall.py` & `fastly-2.3.0/fastly/model/relationship_member_waf_firewall.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_member_waf_firewall_version.py` & `fastly-2.3.0/fastly/model/relationship_member_waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_member_waf_rule.py` & `fastly-2.3.0/fastly/model/relationship_member_waf_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_member_waf_rule_revision.py` & `fastly-2.3.0/fastly/model/relationship_member_waf_rule_revision.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_member_waf_tag.py` & `fastly-2.3.0/fastly/model/relationship_member_waf_tag.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_mutual_authentication.py` & `fastly-2.3.0/fastly/model/relationship_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_mutual_authentication_mutual_authentication.py` & `fastly-2.3.0/fastly/model/relationship_mutual_authentication_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_mutual_authentications.py` & `fastly-2.3.0/fastly/model/relationship_mutual_authentications.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_mutual_authentications_mutual_authentications.py` & `fastly-2.3.0/fastly/model/relationship_mutual_authentications_mutual_authentications.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_service.py` & `fastly-2.3.0/fastly/model/relationship_service.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_service_invitations.py` & `fastly-2.3.0/fastly/model/relationship_service_invitations.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_service_invitations_create.py` & `fastly-2.3.0/fastly/model/relationship_service_invitations_create.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_service_invitations_create_service_invitations.py` & `fastly-2.3.0/fastly/model/relationship_service_invitations_create_service_invitations.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_service_invitations_service_invitations.py` & `fastly-2.3.0/fastly/model/relationship_service_invitations_service_invitations.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_services.py` & `fastly-2.3.0/fastly/model/relationship_services.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_services_services.py` & `fastly-2.3.0/fastly/model/relationship_services_services.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_activation.py` & `fastly-2.3.0/fastly/model/relationship_tls_activation.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_activation_tls_activation.py` & `fastly-2.3.0/fastly/model/relationship_tls_activation_tls_activation.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_activations.py` & `fastly-2.3.0/fastly/model/relationship_tls_activations.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_bulk_certificate.py` & `fastly-2.3.0/fastly/model/relationship_tls_bulk_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_bulk_certificate_tls_bulk_certificate.py` & `fastly-2.3.0/fastly/model/relationship_tls_bulk_certificate_tls_bulk_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_bulk_certificates.py` & `fastly-2.3.0/fastly/model/relationship_tls_bulk_certificates.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_certificate.py` & `fastly-2.3.0/fastly/model/relationship_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_certificate_tls_certificate.py` & `fastly-2.3.0/fastly/model/relationship_tls_certificate_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_certificates.py` & `fastly-2.3.0/fastly/model/relationship_tls_certificates.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_certificates_tls_certificates.py` & `fastly-2.3.0/fastly/model/relationship_tls_certificates_tls_certificates.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_configuration.py` & `fastly-2.3.0/fastly/model/relationship_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_configuration_for_tls_subscription.py` & `fastly-2.3.0/fastly/model/relationship_tls_configuration_for_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_configuration_tls_configuration.py` & `fastly-2.3.0/fastly/model/relationship_tls_configuration_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_configurations.py` & `fastly-2.3.0/fastly/model/relationship_tls_configurations.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_configurations_tls_configurations.py` & `fastly-2.3.0/fastly/model/relationship_tls_configurations_tls_configurations.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_dns_record.py` & `fastly-2.3.0/fastly/model/relationship_tls_dns_record.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_dns_record_dns_record.py` & `fastly-2.3.0/fastly/model/relationship_tls_dns_record_dns_record.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_dns_records.py` & `fastly-2.3.0/fastly/model/relationship_tls_dns_records.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_domain.py` & `fastly-2.3.0/fastly/model/relationship_tls_domain.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_domain_tls_domain.py` & `fastly-2.3.0/fastly/model/relationship_tls_domain_tls_domain.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_domains.py` & `fastly-2.3.0/fastly/model/relationship_tls_domains.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_domains_tls_domains.py` & `fastly-2.3.0/fastly/model/relationship_tls_domains_tls_domains.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_private_key.py` & `fastly-2.3.0/fastly/model/relationship_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_private_key_tls_private_key.py` & `fastly-2.3.0/fastly/model/relationship_tls_private_key_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_private_keys.py` & `fastly-2.3.0/fastly/model/relationship_tls_private_keys.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_private_keys_tls_private_keys.py` & `fastly-2.3.0/fastly/model/relationship_tls_private_keys_tls_private_keys.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_subscription.py` & `fastly-2.3.0/fastly/model/relationship_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_subscription_tls_subscription.py` & `fastly-2.3.0/fastly/model/relationship_tls_subscription_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_tls_subscriptions.py` & `fastly-2.3.0/fastly/model/relationship_tls_subscriptions.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_user.py` & `fastly-2.3.0/fastly/model/relationship_user.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_user_user.py` & `fastly-2.3.0/fastly/model/relationship_user_user.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_waf_active_rules.py` & `fastly-2.3.0/fastly/model/relationship_waf_active_rules.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_waf_active_rules_waf_active_rules.py` & `fastly-2.3.0/fastly/model/relationship_waf_active_rules_waf_active_rules.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_waf_firewall.py` & `fastly-2.3.0/fastly/model/relationship_waf_firewall.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_waf_firewall_version.py` & `fastly-2.3.0/fastly/model/relationship_waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_waf_firewall_version_waf_firewall_version.py` & `fastly-2.3.0/fastly/model/relationship_waf_firewall_version_waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_waf_firewall_versions.py` & `fastly-2.3.0/fastly/model/relationship_waf_firewall_versions.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_waf_firewall_waf_firewall.py` & `fastly-2.3.0/fastly/model/relationship_waf_firewall_waf_firewall.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_waf_rule.py` & `fastly-2.3.0/fastly/model/relationship_waf_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_waf_rule_revision.py` & `fastly-2.3.0/fastly/model/relationship_waf_rule_revision.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_waf_rule_revision_waf_rule_revisions.py` & `fastly-2.3.0/fastly/model/relationship_waf_rule_revision_waf_rule_revisions.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_waf_rule_revisions.py` & `fastly-2.3.0/fastly/model/relationship_waf_rule_revisions.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_waf_rule_waf_rule.py` & `fastly-2.3.0/fastly/model/relationship_waf_rule_waf_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_waf_rules.py` & `fastly-2.3.0/fastly/model/relationship_waf_rules.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_waf_tags.py` & `fastly-2.3.0/fastly/model/relationship_waf_tags.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationship_waf_tags_waf_tags.py` & `fastly-2.3.0/fastly/model/relationship_waf_tags_waf_tags.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationships_for_invitation.py` & `fastly-2.3.0/fastly/model/relationships_for_invitation.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationships_for_mutual_authentication.py` & `fastly-2.3.0/fastly/model/relationships_for_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationships_for_star.py` & `fastly-2.3.0/fastly/model/relationships_for_star.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationships_for_tls_activation.py` & `fastly-2.3.0/fastly/model/relationships_for_tls_activation.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationships_for_tls_bulk_certificate.py` & `fastly-2.3.0/fastly/model/relationships_for_tls_bulk_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationships_for_tls_configuration.py` & `fastly-2.3.0/fastly/model/relationships_for_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationships_for_tls_domain.py` & `fastly-2.3.0/fastly/model/relationships_for_tls_domain.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationships_for_tls_private_key.py` & `fastly-2.3.0/fastly/model/relationships_for_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationships_for_tls_subscription.py` & `fastly-2.3.0/fastly/model/relationships_for_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationships_for_waf_active_rule.py` & `fastly-2.3.0/fastly/model/relationships_for_waf_active_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationships_for_waf_exclusion.py` & `fastly-2.3.0/fastly/model/relationships_for_waf_exclusion.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationships_for_waf_firewall_version.py` & `fastly-2.3.0/fastly/model/relationships_for_waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/relationships_for_waf_rule.py` & `fastly-2.3.0/fastly/model/relationships_for_waf_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/request_settings.py` & `fastly-2.3.0/fastly/model/request_settings.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/request_settings_response.py` & `fastly-2.3.0/fastly/model/request_settings_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/resource.py` & `fastly-2.3.0/fastly/model/resource.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/resource_response.py` & `fastly-2.3.0/fastly/model/resource_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/resource_response_all_of.py` & `fastly-2.3.0/fastly/model/resource_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/response_object.py` & `fastly-2.3.0/fastly/model/response_object.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/response_object_response.py` & `fastly-2.3.0/fastly/model/response_object_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/results.py` & `fastly-2.3.0/fastly/model/results.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/role_user.py` & `fastly-2.3.0/fastly/model/role_user.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/schemas_contact_response.py` & `fastly-2.3.0/fastly/model/schemas_contact_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/schemas_snippet_response.py` & `fastly-2.3.0/fastly/model/schemas_snippet_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/schemas_user_response.py` & `fastly-2.3.0/fastly/model/schemas_user_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/schemas_vcl_response.py` & `fastly-2.3.0/fastly/model/schemas_vcl_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/schemas_version.py` & `fastly-2.3.0/fastly/model/schemas_version.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/schemas_version_response.py` & `fastly-2.3.0/fastly/model/schemas_version_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/schemas_waf_firewall_version.py` & `fastly-2.3.0/fastly/model/schemas_waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/schemas_waf_firewall_version_data.py` & `fastly-2.3.0/fastly/model/schemas_waf_firewall_version_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/server.py` & `fastly-2.3.0/fastly/model/server.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/server_response.py` & `fastly-2.3.0/fastly/model/server_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/server_response_all_of.py` & `fastly-2.3.0/fastly/model/snippet_response_all_of.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class ServerResponseAllOf(ModelNormal):
+class SnippetResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -76,41 +76,41 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'service_id': (str,),  # noqa: E501
+            'version': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
-            'pool_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'service_id': 'service_id',  # noqa: E501
+        'version': 'version',  # noqa: E501
         'id': 'id',  # noqa: E501
-        'pool_id': 'pool_id',  # noqa: E501
     }
 
     read_only_vars = {
         'service_id',  # noqa: E501
+        'version',  # noqa: E501
         'id',  # noqa: E501
-        'pool_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ServerResponseAllOf - a model defined in OpenAPI
+        """SnippetResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,16 +136,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             service_id (str): [optional]  # noqa: E501
+            version (str): String representing the number identifying a version of the service.. [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
-            pool_id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ServerResponseAllOf - a model defined in OpenAPI
+        """SnippetResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -220,16 +220,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             service_id (str): [optional]  # noqa: E501
+            version (str): String representing the number identifying a version of the service.. [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
-            pool_id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-2.2.2/fastly/model/service.py` & `fastly-2.3.0/fastly/model/service.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_authorization.py` & `fastly-2.3.0/fastly/model/service_authorization.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_authorization_data.py` & `fastly-2.3.0/fastly/model/service_authorization_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_authorization_data_attributes.py` & `fastly-2.3.0/fastly/model/service_authorization_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_authorization_data_relationships.py` & `fastly-2.3.0/fastly/model/service_authorization_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_authorization_data_relationships_user.py` & `fastly-2.3.0/fastly/model/service_authorization_data_relationships_user.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_authorization_data_relationships_user_data.py` & `fastly-2.3.0/fastly/model/service_authorization_data_relationships_user_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_authorization_response.py` & `fastly-2.3.0/fastly/model/service_authorization_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_authorization_response_data.py` & `fastly-2.3.0/fastly/model/service_authorization_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_authorization_response_data_all_of.py` & `fastly-2.3.0/fastly/model/service_authorization_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_authorizations_response.py` & `fastly-2.3.0/fastly/model/service_authorizations_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_authorizations_response_all_of.py` & `fastly-2.3.0/fastly/model/service_authorizations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_create.py` & `fastly-2.3.0/fastly/model/service_create.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_create_all_of.py` & `fastly-2.3.0/fastly/model/service_create_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_detail.py` & `fastly-2.3.0/fastly/model/service_detail.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_detail_all_of.py` & `fastly-2.3.0/fastly/model/service_detail_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_id_and_version.py` & `fastly-2.3.0/fastly/model/service_id_and_version.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_invitation.py` & `fastly-2.3.0/fastly/model/service_invitation.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_invitation_data.py` & `fastly-2.3.0/fastly/model/service_invitation_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_invitation_data_attributes.py` & `fastly-2.3.0/fastly/model/service_invitation_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_invitation_data_relationships.py` & `fastly-2.3.0/fastly/model/service_invitation_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_invitation_response.py` & `fastly-2.3.0/fastly/model/service_invitation_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_invitation_response_all_of.py` & `fastly-2.3.0/fastly/model/service_invitation_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_invitation_response_all_of_data.py` & `fastly-2.3.0/fastly/model/service_invitation_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_list_response.py` & `fastly-2.3.0/fastly/model/service_list_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_list_response_all_of.py` & `fastly-2.3.0/fastly/model/service_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_response.py` & `fastly-2.3.0/fastly/model/service_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_response_all_of.py` & `fastly-2.3.0/fastly/model/service_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_version_detail.py` & `fastly-2.3.0/fastly/model/service_version_detail.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/service_version_detail_or_null.py` & `fastly-2.3.0/fastly/model/service_version_detail_or_null.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/settings.py` & `fastly-2.3.0/fastly/model/settings.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/settings_response.py` & `fastly-2.3.0/fastly/model/settings_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/snippet.py` & `fastly-2.3.0/fastly/model/snippet.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/snippet_response.py` & `fastly-2.3.0/fastly/model/snippet_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/snippet_response_all_of.py` & `fastly-2.3.0/fastly/model/tls_certificate_response_data_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fastly.model.tls_certificate_response_attributes import TlsCertificateResponseAttributes
+    globals()['TlsCertificateResponseAttributes'] = TlsCertificateResponseAttributes
 
-class SnippetResponseAllOf(ModelNormal):
+
+class TlsCertificateResponseDataAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -60,57 +64,55 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'service_id': (str,),  # noqa: E501
-            'version': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
+            'attributes': (TlsCertificateResponseAttributes,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'service_id': 'service_id',  # noqa: E501
-        'version': 'version',  # noqa: E501
         'id': 'id',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
-        'service_id',  # noqa: E501
-        'version',  # noqa: E501
         'id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SnippetResponseAllOf - a model defined in OpenAPI
+        """TlsCertificateResponseDataAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,17 +137,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            service_id (str): [optional]  # noqa: E501
-            version (str): String representing the number identifying a version of the service.. [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
+            attributes (TlsCertificateResponseAttributes): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +187,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SnippetResponseAllOf - a model defined in OpenAPI
+        """TlsCertificateResponseDataAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,17 +220,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            service_id (str): [optional]  # noqa: E501
-            version (str): String representing the number identifying a version of the service.. [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
+            attributes (TlsCertificateResponseAttributes): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-2.2.2/fastly/model/star.py` & `fastly-2.3.0/fastly/model/star.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/star_data.py` & `fastly-2.3.0/fastly/model/star_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/star_response.py` & `fastly-2.3.0/fastly/model/star_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/star_response_all_of.py` & `fastly-2.3.0/fastly/model/star_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/stats.py` & `fastly-2.3.0/fastly/model/stats.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/store.py` & `fastly-2.3.0/fastly/model/store.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/store_response.py` & `fastly-2.3.0/fastly/model/vcl.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class StoreResponse(ModelNormal):
+class Vcl(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -75,37 +75,39 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str,),  # noqa: E501
+            'content': (str,),  # noqa: E501
+            'main': (bool,),  # noqa: E501
             'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
+        'content': 'content',  # noqa: E501
+        'main': 'main',  # noqa: E501
         'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """StoreResponse - a model defined in OpenAPI
+        """Vcl - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -130,16 +132,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): ID of the store.. [optional]  # noqa: E501
-            name (str): A human-readable name for the store.. [optional]  # noqa: E501
+            content (str): The VCL code to be included.. [optional]  # noqa: E501
+            main (bool): Set to `true` when this is the main VCL, otherwise `false`.. [optional]  # noqa: E501
+            name (str): The name of this VCL.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -180,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """StoreResponse - a model defined in OpenAPI
+        """Vcl - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -213,16 +216,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): ID of the store.. [optional]  # noqa: E501
-            name (str): A human-readable name for the store.. [optional]  # noqa: E501
+            content (str): The VCL code to be included.. [optional]  # noqa: E501
+            main (bool): Set to `true` when this is the main VCL, otherwise `false`.. [optional]  # noqa: E501
+            name (str): The name of this VCL.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-2.2.2/fastly/model/timestamps.py` & `fastly-2.3.0/fastly/model/timestamps.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/timestamps_no_delete.py` & `fastly-2.3.0/fastly/model/timestamps_no_delete.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_activation.py` & `fastly-2.3.0/fastly/model/tls_activation.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_activation_data.py` & `fastly-2.3.0/fastly/model/tls_activation_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_activation_response.py` & `fastly-2.3.0/fastly/model/tls_activation_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_activation_response_data.py` & `fastly-2.3.0/fastly/model/tls_activation_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_activation_response_data_all_of.py` & `fastly-2.3.0/fastly/model/tls_activation_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_activations_response.py` & `fastly-2.3.0/fastly/model/tls_activations_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_activations_response_all_of.py` & `fastly-2.3.0/fastly/model/tls_activations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_bulk_certificate.py` & `fastly-2.3.0/fastly/model/tls_bulk_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_bulk_certificate_data.py` & `fastly-2.3.0/fastly/model/tls_bulk_certificate_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_bulk_certificate_data_attributes.py` & `fastly-2.3.0/fastly/model/tls_bulk_certificate_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_bulk_certificate_response.py` & `fastly-2.3.0/fastly/model/tls_bulk_certificate_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_bulk_certificate_response_attributes.py` & `fastly-2.3.0/fastly/model/tls_bulk_certificate_response_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_bulk_certificate_response_attributes_all_of.py` & `fastly-2.3.0/fastly/model/tls_bulk_certificate_response_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_bulk_certificate_response_data.py` & `fastly-2.3.0/fastly/model/tls_bulk_certificate_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_bulk_certificate_response_data_all_of.py` & `fastly-2.3.0/fastly/model/tls_bulk_certificate_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_bulk_certificates_response.py` & `fastly-2.3.0/fastly/model/tls_bulk_certificates_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_bulk_certificates_response_all_of.py` & `fastly-2.3.0/fastly/model/tls_bulk_certificates_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_certificate.py` & `fastly-2.3.0/fastly/model/tls_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_certificate_data.py` & `fastly-2.3.0/fastly/model/tls_certificate_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_certificate_data_attributes.py` & `fastly-2.3.0/fastly/model/tls_certificate_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_certificate_response.py` & `fastly-2.3.0/fastly/model/tls_certificate_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_certificate_response_attributes.py` & `fastly-2.3.0/fastly/model/tls_certificate_response_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_certificate_response_attributes_all_of.py` & `fastly-2.3.0/fastly/model/tls_certificate_response_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_certificate_response_data.py` & `fastly-2.3.0/fastly/model/tls_certificate_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_certificate_response_data_all_of.py` & `fastly-2.3.0/fastly/model/tls_certificates_response_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.tls_certificate_response_attributes import TlsCertificateResponseAttributes
-    globals()['TlsCertificateResponseAttributes'] = TlsCertificateResponseAttributes
+    from fastly.model.tls_certificate_response_data import TlsCertificateResponseData
+    globals()['TlsCertificateResponseData'] = TlsCertificateResponseData
 
 
-class TlsCertificateResponseDataAllOf(ModelNormal):
+class TlsCertificatesResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -81,38 +81,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'id': (str,),  # noqa: E501
-            'attributes': (TlsCertificateResponseAttributes,),  # noqa: E501
+            'data': ([TlsCertificateResponseData],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'attributes': 'attributes',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
-        'id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TlsCertificateResponseDataAllOf - a model defined in OpenAPI
+        """TlsCertificatesResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,16 +134,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            attributes (TlsCertificateResponseAttributes): [optional]  # noqa: E501
+            data ([TlsCertificateResponseData]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -187,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TlsCertificateResponseDataAllOf - a model defined in OpenAPI
+        """TlsCertificatesResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -220,16 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            attributes (TlsCertificateResponseAttributes): [optional]  # noqa: E501
+            data ([TlsCertificateResponseData]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-2.2.2/fastly/model/tls_certificates_response.py` & `fastly-2.3.0/fastly/model/tls_certificates_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_certificates_response_all_of.py` & `fastly-2.3.0/fastly/model/tls_private_key_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.tls_certificate_response_data import TlsCertificateResponseData
-    globals()['TlsCertificateResponseData'] = TlsCertificateResponseData
+    from fastly.model.tls_private_key_response_data import TlsPrivateKeyResponseData
+    globals()['TlsPrivateKeyResponseData'] = TlsPrivateKeyResponseData
 
 
-class TlsCertificatesResponseAllOf(ModelNormal):
+class TlsPrivateKeyResponse(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -81,15 +81,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([TlsCertificateResponseData],),  # noqa: E501
+            'data': (TlsPrivateKeyResponseData,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -101,15 +101,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TlsCertificatesResponseAllOf - a model defined in OpenAPI
+        """TlsPrivateKeyResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +134,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([TlsCertificateResponseData]): [optional]  # noqa: E501
+            data (TlsPrivateKeyResponseData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TlsCertificatesResponseAllOf - a model defined in OpenAPI
+        """TlsPrivateKeyResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([TlsCertificateResponseData]): [optional]  # noqa: E501
+            data (TlsPrivateKeyResponseData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-2.2.2/fastly/model/tls_common.py` & `fastly-2.3.0/fastly/model/tls_common.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_configuration.py` & `fastly-2.3.0/fastly/model/tls_configuration.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_configuration_data.py` & `fastly-2.3.0/fastly/model/tls_configuration_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_configuration_data_attributes.py` & `fastly-2.3.0/fastly/model/tls_configuration_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_configuration_response.py` & `fastly-2.3.0/fastly/model/tls_configuration_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_configuration_response_attributes.py` & `fastly-2.3.0/fastly/model/tls_configuration_response_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_configuration_response_attributes_all_of.py` & `fastly-2.3.0/fastly/model/tls_configuration_response_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_configuration_response_data.py` & `fastly-2.3.0/fastly/model/tls_configuration_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_configuration_response_data_all_of.py` & `fastly-2.3.0/fastly/model/tls_configuration_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_configurations_response.py` & `fastly-2.3.0/fastly/model/tls_configurations_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_configurations_response_all_of.py` & `fastly-2.3.0/fastly/model/tls_configurations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_dns_record.py` & `fastly-2.3.0/fastly/model/tls_dns_record.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_domain_data.py` & `fastly-2.3.0/fastly/model/tls_domain_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_domains_response.py` & `fastly-2.3.0/fastly/model/tls_domains_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_domains_response_all_of.py` & `fastly-2.3.0/fastly/model/tls_domains_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_private_key.py` & `fastly-2.3.0/fastly/model/tls_private_key.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_private_key_data.py` & `fastly-2.3.0/fastly/model/tls_private_key_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_private_key_data_attributes.py` & `fastly-2.3.0/fastly/model/tls_private_key_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_private_key_response.py` & `fastly-2.3.0/fastly/model/tls_private_keys_response_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 def lazy_import():
     from fastly.model.tls_private_key_response_data import TlsPrivateKeyResponseData
     globals()['TlsPrivateKeyResponseData'] = TlsPrivateKeyResponseData
 
 
-class TlsPrivateKeyResponse(ModelNormal):
+class TlsPrivateKeysResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -81,15 +81,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (TlsPrivateKeyResponseData,),  # noqa: E501
+            'data': ([TlsPrivateKeyResponseData],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -101,15 +101,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TlsPrivateKeyResponse - a model defined in OpenAPI
+        """TlsPrivateKeysResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +134,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (TlsPrivateKeyResponseData): [optional]  # noqa: E501
+            data ([TlsPrivateKeyResponseData]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TlsPrivateKeyResponse - a model defined in OpenAPI
+        """TlsPrivateKeysResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (TlsPrivateKeyResponseData): [optional]  # noqa: E501
+            data ([TlsPrivateKeyResponseData]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-2.2.2/fastly/model/tls_private_key_response_attributes.py` & `fastly-2.3.0/fastly/model/tls_private_key_response_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_private_key_response_attributes_all_of.py` & `fastly-2.3.0/fastly/model/tls_private_key_response_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_private_key_response_data.py` & `fastly-2.3.0/fastly/model/tls_private_key_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_private_keys_response.py` & `fastly-2.3.0/fastly/model/tls_private_keys_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_private_keys_response_all_of.py` & `fastly-2.3.0/fastly/model/tls_subscription.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.tls_private_key_response_data import TlsPrivateKeyResponseData
-    globals()['TlsPrivateKeyResponseData'] = TlsPrivateKeyResponseData
+    from fastly.model.tls_subscription_data import TlsSubscriptionData
+    globals()['TlsSubscriptionData'] = TlsSubscriptionData
 
 
-class TlsPrivateKeysResponseAllOf(ModelNormal):
+class TlsSubscription(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -81,15 +81,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([TlsPrivateKeyResponseData],),  # noqa: E501
+            'data': (TlsSubscriptionData,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -101,15 +101,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TlsPrivateKeysResponseAllOf - a model defined in OpenAPI
+        """TlsSubscription - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +134,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([TlsPrivateKeyResponseData]): [optional]  # noqa: E501
+            data (TlsSubscriptionData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TlsPrivateKeysResponseAllOf - a model defined in OpenAPI
+        """TlsSubscription - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([TlsPrivateKeyResponseData]): [optional]  # noqa: E501
+            data (TlsSubscriptionData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-2.2.2/fastly/model/tls_subscription.py` & `fastly-2.3.0/fastly/model/tls_subscription_response_attributes_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from fastly.model.tls_subscription_data import TlsSubscriptionData
-    globals()['TlsSubscriptionData'] = TlsSubscriptionData
 
-
-class TlsSubscription(ModelNormal):
+class TlsSubscriptionResponseAttributesAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -53,63 +49,68 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('state',): {
+            'PENDING': "pending",
+            'PROCESSING': "processing",
+            'ISSUED': "issued",
+            'RENEWING': "renewing",
+            'FAILED': "failed",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'data': (TlsSubscriptionData,),  # noqa: E501
+            'state': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'state': 'state',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TlsSubscription - a model defined in OpenAPI
+        """TlsSubscriptionResponseAttributesAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +135,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (TlsSubscriptionData): [optional]  # noqa: E501
+            state (str): The current state of your subscription.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +184,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TlsSubscription - a model defined in OpenAPI
+        """TlsSubscriptionResponseAttributesAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +217,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (TlsSubscriptionData): [optional]  # noqa: E501
+            state (str): The current state of your subscription.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-2.2.2/fastly/model/tls_subscription_data.py` & `fastly-2.3.0/fastly/model/tls_subscription_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_subscription_data_attributes.py` & `fastly-2.3.0/fastly/model/tls_subscription_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_subscription_response.py` & `fastly-2.3.0/fastly/model/tls_subscription_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_subscription_response_attributes.py` & `fastly-2.3.0/fastly/model/tls_subscription_response_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_subscription_response_attributes_all_of.py` & `fastly-2.3.0/fastly/model/version_response_all_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class TlsSubscriptionResponseAttributesAllOf(ModelNormal):
+class VersionResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -49,21 +49,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('state',): {
-            'PENDING': "pending",
-            'PROCESSING': "processing",
-            'ISSUED': "issued",
-            'RENEWING': "renewing",
-            'FAILED': "failed",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -82,35 +75,36 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'state': (str,),  # noqa: E501
+            'service_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'state': 'state',  # noqa: E501
+        'service_id': 'service_id',  # noqa: E501
     }
 
     read_only_vars = {
+        'service_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TlsSubscriptionResponseAttributesAllOf - a model defined in OpenAPI
+        """VersionResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,15 +129,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            state (str): The current state of your subscription.. [optional]  # noqa: E501
+            service_id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -184,15 +178,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TlsSubscriptionResponseAttributesAllOf - a model defined in OpenAPI
+        """VersionResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -217,15 +211,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            state (str): The current state of your subscription.. [optional]  # noqa: E501
+            service_id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-2.2.2/fastly/model/tls_subscription_response_data.py` & `fastly-2.3.0/fastly/model/tls_subscription_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_subscription_response_data_all_of.py` & `fastly-2.3.0/fastly/model/tls_subscription_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_subscriptions_response.py` & `fastly-2.3.0/fastly/model/tls_subscriptions_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/tls_subscriptions_response_all_of.py` & `fastly-2.3.0/fastly/model/tls_subscriptions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/token.py` & `fastly-2.3.0/fastly/model/token.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/token_created_response.py` & `fastly-2.3.0/fastly/model/token_created_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/token_created_response_all_of.py` & `fastly-2.3.0/fastly/model/token_created_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/token_response.py` & `fastly-2.3.0/fastly/model/token_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/token_response_all_of.py` & `fastly-2.3.0/fastly/model/token_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_billing_address.py` & `fastly-2.3.0/fastly/model/type_billing_address.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_contact.py` & `fastly-2.3.0/fastly/model/type_contact.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_customer.py` & `fastly-2.3.0/fastly/model/type_customer.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_event.py` & `fastly-2.3.0/fastly/model/type_event.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_invitation.py` & `fastly-2.3.0/fastly/model/type_invitation.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_mutual_authentication.py` & `fastly-2.3.0/fastly/model/type_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_resource.py` & `fastly-2.3.0/fastly/model/type_resource.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_service.py` & `fastly-2.3.0/fastly/model/type_service.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_service_authorization.py` & `fastly-2.3.0/fastly/model/type_service_authorization.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_service_invitation.py` & `fastly-2.3.0/fastly/model/type_service_invitation.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_star.py` & `fastly-2.3.0/fastly/model/type_star.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_tls_activation.py` & `fastly-2.3.0/fastly/model/type_tls_activation.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_tls_bulk_certificate.py` & `fastly-2.3.0/fastly/model/type_tls_bulk_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_tls_certificate.py` & `fastly-2.3.0/fastly/model/type_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_tls_configuration.py` & `fastly-2.3.0/fastly/model/type_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_tls_dns_record.py` & `fastly-2.3.0/fastly/model/type_tls_dns_record.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_tls_domain.py` & `fastly-2.3.0/fastly/model/type_tls_domain.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_tls_private_key.py` & `fastly-2.3.0/fastly/model/type_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_tls_subscription.py` & `fastly-2.3.0/fastly/model/type_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_user.py` & `fastly-2.3.0/fastly/model/type_user.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_waf_active_rule.py` & `fastly-2.3.0/fastly/model/type_waf_active_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_waf_exclusion.py` & `fastly-2.3.0/fastly/model/type_waf_exclusion.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_waf_firewall.py` & `fastly-2.3.0/fastly/model/type_waf_firewall.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_waf_firewall_version.py` & `fastly-2.3.0/fastly/model/type_waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_waf_rule.py` & `fastly-2.3.0/fastly/model/type_waf_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_waf_rule_revision.py` & `fastly-2.3.0/fastly/model/type_waf_rule_revision.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/type_waf_tag.py` & `fastly-2.3.0/fastly/model/type_waf_tag.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/update_billing_address_request.py` & `fastly-2.3.0/fastly/model/update_billing_address_request.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/update_billing_address_request_data.py` & `fastly-2.3.0/fastly/model/update_billing_address_request_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/user.py` & `fastly-2.3.0/fastly/model/user.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/user_response.py` & `fastly-2.3.0/fastly/model/user_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/user_response_all_of.py` & `fastly-2.3.0/fastly/model/user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/validator_result.py` & `fastly-2.3.0/fastly/model/validator_result.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/validator_result_messages.py` & `fastly-2.3.0/fastly/model/validator_result_messages.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/vcl.py` & `fastly-2.3.0/fastly/model/version_create_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class Vcl(ModelNormal):
+class VersionCreateResponse(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -75,39 +75,39 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'content': (str,),  # noqa: E501
-            'main': (bool,),  # noqa: E501
-            'name': (str,),  # noqa: E501
+            'number': (int,),  # noqa: E501
+            'service_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'content': 'content',  # noqa: E501
-        'main': 'main',  # noqa: E501
-        'name': 'name',  # noqa: E501
+        'number': 'number',  # noqa: E501
+        'service_id': 'service_id',  # noqa: E501
     }
 
     read_only_vars = {
+        'number',  # noqa: E501
+        'service_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Vcl - a model defined in OpenAPI
+        """VersionCreateResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,17 +132,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            content (str): The VCL code to be included.. [optional]  # noqa: E501
-            main (bool): Set to `true` when this is the main VCL, otherwise `false`.. [optional]  # noqa: E501
-            name (str): The name of this VCL.. [optional]  # noqa: E501
+            number (int): [optional]  # noqa: E501
+            service_id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Vcl - a model defined in OpenAPI
+        """VersionCreateResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,17 +215,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            content (str): The VCL code to be included.. [optional]  # noqa: E501
-            main (bool): Set to `true` when this is the main VCL, otherwise `false`.. [optional]  # noqa: E501
-            name (str): The name of this VCL.. [optional]  # noqa: E501
+            number (int): [optional]  # noqa: E501
+            service_id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-2.2.2/fastly/model/vcl_diff.py` & `fastly-2.3.0/fastly/model/vcl_diff.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/vcl_response.py` & `fastly-2.3.0/fastly/model/vcl_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/version.py` & `fastly-2.3.0/fastly/model/version.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/version_create_response.py` & `fastly-2.3.0/fastly/model/waf_active_rule_response_data_attributes_all_of.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class VersionCreateResponse(ModelNormal):
+class WafActiveRuleResponseDataAttributesAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -75,39 +75,39 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'number': (int,),  # noqa: E501
-            'service_id': (str,),  # noqa: E501
+            'latest_revision': (int,),  # noqa: E501
+            'outdated': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'number': 'number',  # noqa: E501
-        'service_id': 'service_id',  # noqa: E501
+        'latest_revision': 'latest_revision',  # noqa: E501
+        'outdated': 'outdated',  # noqa: E501
     }
 
     read_only_vars = {
-        'number',  # noqa: E501
-        'service_id',  # noqa: E501
+        'latest_revision',  # noqa: E501
+        'outdated',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """VersionCreateResponse - a model defined in OpenAPI
+        """WafActiveRuleResponseDataAttributesAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,16 +132,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            number (int): [optional]  # noqa: E501
-            service_id (str): [optional]  # noqa: E501
+            latest_revision (int): The latest rule revision number that is available for the associated rule revision.. [optional]  # noqa: E501
+            outdated (bool): Indicates if the associated rule revision is up to date or not.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -182,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """VersionCreateResponse - a model defined in OpenAPI
+        """WafActiveRuleResponseDataAttributesAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -215,16 +215,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            number (int): [optional]  # noqa: E501
-            service_id (str): [optional]  # noqa: E501
+            latest_revision (int): The latest rule revision number that is available for the associated rule revision.. [optional]  # noqa: E501
+            outdated (bool): Indicates if the associated rule revision is up to date or not.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-2.2.2/fastly/model/version_detail.py` & `fastly-2.3.0/fastly/model/version_detail.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/version_detail_settings.py` & `fastly-2.3.0/fastly/model/version_detail_settings.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/version_response.py` & `fastly-2.3.0/fastly/model/version_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/version_response_all_of.py` & `fastly-2.3.0/fastly/model/historical_field_results_attributes_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fastly.model.read_only_id_service import ReadOnlyIdService
+    globals()['ReadOnlyIdService'] = ReadOnlyIdService
 
-class VersionResponseAllOf(ModelNormal):
+
+class HistoricalFieldResultsAttributesAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -60,51 +64,54 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'service_id': (str,),  # noqa: E501
+            'service_id': (ReadOnlyIdService,),  # noqa: E501
+            'start_time': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'service_id': 'service_id',  # noqa: E501
+        'start_time': 'start_time',  # noqa: E501
     }
 
     read_only_vars = {
-        'service_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """VersionResponseAllOf - a model defined in OpenAPI
+        """HistoricalFieldResultsAttributesAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -129,15 +136,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            service_id (str): [optional]  # noqa: E501
+            service_id (ReadOnlyIdService): [optional]  # noqa: E501
+            start_time (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -178,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """VersionResponseAllOf - a model defined in OpenAPI
+        """HistoricalFieldResultsAttributesAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -211,15 +219,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            service_id (str): [optional]  # noqa: E501
+            service_id (ReadOnlyIdService): [optional]  # noqa: E501
+            start_time (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-2.2.2/fastly/model/waf_active_rule.py` & `fastly-2.3.0/fastly/model/waf_active_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_active_rule_creation_response.py` & `fastly-2.3.0/fastly/model/waf_active_rule_creation_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_active_rule_data.py` & `fastly-2.3.0/fastly/model/waf_active_rule_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_active_rule_data_attributes.py` & `fastly-2.3.0/fastly/model/waf_active_rule_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_active_rule_response.py` & `fastly-2.3.0/fastly/model/waf_active_rule_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_active_rule_response_data.py` & `fastly-2.3.0/fastly/model/waf_active_rule_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_active_rule_response_data_all_of.py` & `fastly-2.3.0/fastly/model/waf_active_rule_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_active_rule_response_data_attributes.py` & `fastly-2.3.0/fastly/model/waf_active_rule_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_active_rule_response_data_attributes_all_of.py` & `fastly-2.3.0/fastly/model/waf_rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,22 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fastly.model.type_waf_rule import TypeWafRule
+    from fastly.model.waf_rule_attributes import WafRuleAttributes
+    globals()['TypeWafRule'] = TypeWafRule
+    globals()['WafRuleAttributes'] = WafRuleAttributes
 
-class WafActiveRuleResponseDataAttributesAllOf(ModelNormal):
+
+class WafRule(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -60,54 +66,57 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'latest_revision': (int,),  # noqa: E501
-            'outdated': (bool,),  # noqa: E501
+            'type': (TypeWafRule,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'attributes': (WafRuleAttributes,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'latest_revision': 'latest_revision',  # noqa: E501
-        'outdated': 'outdated',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
-        'latest_revision',  # noqa: E501
-        'outdated',  # noqa: E501
+        'id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafActiveRuleResponseDataAttributesAllOf - a model defined in OpenAPI
+        """WafRule - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,16 +141,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            latest_revision (int): The latest rule revision number that is available for the associated rule revision.. [optional]  # noqa: E501
-            outdated (bool): Indicates if the associated rule revision is up to date or not.. [optional]  # noqa: E501
+            type (TypeWafRule): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            attributes (WafRuleAttributes): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -182,15 +192,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafActiveRuleResponseDataAttributesAllOf - a model defined in OpenAPI
+        """WafRule - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -215,16 +225,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            latest_revision (int): The latest rule revision number that is available for the associated rule revision.. [optional]  # noqa: E501
-            outdated (bool): Indicates if the associated rule revision is up to date or not.. [optional]  # noqa: E501
+            type (TypeWafRule): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            attributes (WafRuleAttributes): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-2.2.2/fastly/model/waf_active_rule_response_data_relationships.py` & `fastly-2.3.0/fastly/model/waf_active_rule_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_active_rules_response.py` & `fastly-2.3.0/fastly/model/waf_active_rules_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_active_rules_response_all_of.py` & `fastly-2.3.0/fastly/model/waf_active_rules_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_exclusion.py` & `fastly-2.3.0/fastly/model/waf_exclusion.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_exclusion_data.py` & `fastly-2.3.0/fastly/model/waf_exclusion_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_exclusion_data_attributes.py` & `fastly-2.3.0/fastly/model/waf_exclusion_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_exclusion_response.py` & `fastly-2.3.0/fastly/model/waf_exclusion_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_exclusion_response_data.py` & `fastly-2.3.0/fastly/model/waf_exclusion_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_exclusion_response_data_all_of.py` & `fastly-2.3.0/fastly/model/waf_exclusion_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_exclusion_response_data_attributes.py` & `fastly-2.3.0/fastly/model/waf_exclusion_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_exclusion_response_data_attributes_all_of.py` & `fastly-2.3.0/fastly/model/waf_exclusion_response_data_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_exclusion_response_data_relationships.py` & `fastly-2.3.0/fastly/model/waf_exclusion_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_exclusions_response.py` & `fastly-2.3.0/fastly/model/waf_exclusions_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_exclusions_response_all_of.py` & `fastly-2.3.0/fastly/model/waf_exclusions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_firewall.py` & `fastly-2.3.0/fastly/model/waf_firewall.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_firewall_data.py` & `fastly-2.3.0/fastly/model/waf_firewall_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_firewall_data_attributes.py` & `fastly-2.3.0/fastly/model/waf_firewall_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_firewall_response.py` & `fastly-2.3.0/fastly/model/waf_firewall_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_firewall_response_data.py` & `fastly-2.3.0/fastly/model/waf_firewall_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_firewall_response_data_all_of.py` & `fastly-2.3.0/fastly/model/waf_firewall_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_firewall_response_data_attributes.py` & `fastly-2.3.0/fastly/model/waf_firewall_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_firewall_response_data_attributes_all_of.py` & `fastly-2.3.0/fastly/model/waf_firewall_response_data_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_firewall_version.py` & `fastly-2.3.0/fastly/model/waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_firewall_version_data.py` & `fastly-2.3.0/fastly/model/waf_firewall_version_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_firewall_version_data_attributes.py` & `fastly-2.3.0/fastly/model/waf_firewall_version_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_firewall_version_response.py` & `fastly-2.3.0/fastly/model/waf_firewall_version_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_firewall_version_response_data.py` & `fastly-2.3.0/fastly/model/waf_firewall_version_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_firewall_version_response_data_all_of.py` & `fastly-2.3.0/fastly/model/waf_firewall_version_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_firewall_version_response_data_attributes.py` & `fastly-2.3.0/fastly/model/waf_firewall_version_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_firewall_version_response_data_attributes_all_of.py` & `fastly-2.3.0/fastly/model/waf_firewall_version_response_data_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_firewall_versions_response.py` & `fastly-2.3.0/fastly/model/waf_firewall_versions_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_firewall_versions_response_all_of.py` & `fastly-2.3.0/fastly/model/waf_firewall_versions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_firewalls_response.py` & `fastly-2.3.0/fastly/model/waf_firewalls_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_firewalls_response_all_of.py` & `fastly-2.3.0/fastly/model/waf_firewalls_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_rule.py` & `fastly-2.3.0/fastly/model/waf_rule_attributes.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,22 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from fastly.model.type_waf_rule import TypeWafRule
-    from fastly.model.waf_rule_attributes import WafRuleAttributes
-    globals()['TypeWafRule'] = TypeWafRule
-    globals()['WafRuleAttributes'] = WafRuleAttributes
 
-
-class WafRule(ModelNormal):
+class WafRuleAttributes(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -55,68 +49,78 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('publisher',): {
+            'FASTLY': "fastly",
+            'TRUSTWAVE': "trustwave",
+            'OWASP': "owasp",
+        },
+        ('type',): {
+            'STRICT': "strict",
+            'SCORE': "score",
+            'THRESHOLD': "threshold",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'type': (TypeWafRule,),  # noqa: E501
-            'id': (str,),  # noqa: E501
-            'attributes': (WafRuleAttributes,),  # noqa: E501
+            'modsec_rule_id': (int,),  # noqa: E501
+            'publisher': (str,),  # noqa: E501
+            'type': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'modsec_rule_id': 'modsec_rule_id',  # noqa: E501
+        'publisher': 'publisher',  # noqa: E501
         'type': 'type',  # noqa: E501
-        'id': 'id',  # noqa: E501
-        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
-        'id',  # noqa: E501
+        'modsec_rule_id',  # noqa: E501
+        'publisher',  # noqa: E501
+        'type',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafRule - a model defined in OpenAPI
+        """WafRuleAttributes - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -141,17 +145,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (TypeWafRule): [optional]  # noqa: E501
-            id (str): [optional]  # noqa: E501
-            attributes (WafRuleAttributes): [optional]  # noqa: E501
+            modsec_rule_id (int): Corresponding ModSecurity rule ID.. [optional]  # noqa: E501
+            publisher (str): Rule publisher.. [optional]  # noqa: E501
+            type (str): The rule's [type](https://docs.fastly.com/en/guides/managing-rules-on-the-fastly-waf#understanding-the-types-of-rules).. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -192,15 +196,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafRule - a model defined in OpenAPI
+        """WafRuleAttributes - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -225,17 +229,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (TypeWafRule): [optional]  # noqa: E501
-            id (str): [optional]  # noqa: E501
-            attributes (WafRuleAttributes): [optional]  # noqa: E501
+            modsec_rule_id (int): Corresponding ModSecurity rule ID.. [optional]  # noqa: E501
+            publisher (str): Rule publisher.. [optional]  # noqa: E501
+            type (str): The rule's [type](https://docs.fastly.com/en/guides/managing-rules-on-the-fastly-waf#understanding-the-types-of-rules).. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-2.2.2/fastly/model/waf_rule_attributes.py` & `fastly-2.3.0/fastly/model/waf_rules_response_all_of.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,16 +25,22 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fastly.model.included_with_waf_rule import IncludedWithWafRule
+    from fastly.model.waf_rule_response_data import WafRuleResponseData
+    globals()['IncludedWithWafRule'] = IncludedWithWafRule
+    globals()['WafRuleResponseData'] = WafRuleResponseData
 
-class WafRuleAttributes(ModelNormal):
+
+class WafRulesResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -49,78 +55,65 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('publisher',): {
-            'FASTLY': "fastly",
-            'TRUSTWAVE': "trustwave",
-            'OWASP': "owasp",
-        },
-        ('type',): {
-            'STRICT': "strict",
-            'SCORE': "score",
-            'THRESHOLD': "threshold",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'modsec_rule_id': (int,),  # noqa: E501
-            'publisher': (str,),  # noqa: E501
-            'type': (str,),  # noqa: E501
+            'data': ([WafRuleResponseData],),  # noqa: E501
+            'included': (IncludedWithWafRule,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'modsec_rule_id': 'modsec_rule_id',  # noqa: E501
-        'publisher': 'publisher',  # noqa: E501
-        'type': 'type',  # noqa: E501
+        'data': 'data',  # noqa: E501
+        'included': 'included',  # noqa: E501
     }
 
     read_only_vars = {
-        'modsec_rule_id',  # noqa: E501
-        'publisher',  # noqa: E501
-        'type',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafRuleAttributes - a model defined in OpenAPI
+        """WafRulesResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -145,17 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            modsec_rule_id (int): Corresponding ModSecurity rule ID.. [optional]  # noqa: E501
-            publisher (str): Rule publisher.. [optional]  # noqa: E501
-            type (str): The rule's [type](https://docs.fastly.com/en/guides/managing-rules-on-the-fastly-waf#understanding-the-types-of-rules).. [optional]  # noqa: E501
+            data ([WafRuleResponseData]): [optional]  # noqa: E501
+            included (IncludedWithWafRule): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -196,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafRuleAttributes - a model defined in OpenAPI
+        """WafRulesResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -229,17 +221,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            modsec_rule_id (int): Corresponding ModSecurity rule ID.. [optional]  # noqa: E501
-            publisher (str): Rule publisher.. [optional]  # noqa: E501
-            type (str): The rule's [type](https://docs.fastly.com/en/guides/managing-rules-on-the-fastly-waf#understanding-the-types-of-rules).. [optional]  # noqa: E501
+            data ([WafRuleResponseData]): [optional]  # noqa: E501
+            included (IncludedWithWafRule): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-2.2.2/fastly/model/waf_rule_response.py` & `fastly-2.3.0/fastly/model/waf_rule_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_rule_response_data.py` & `fastly-2.3.0/fastly/model/waf_rule_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_rule_response_data_all_of.py` & `fastly-2.3.0/fastly/model/waf_rule_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_rule_revision.py` & `fastly-2.3.0/fastly/model/waf_rule_revision.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_rule_revision_attributes.py` & `fastly-2.3.0/fastly/model/waf_rule_revision_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_rule_revision_or_latest.py` & `fastly-2.3.0/fastly/model/waf_rule_revision_or_latest.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_rule_revision_response.py` & `fastly-2.3.0/fastly/model/waf_rule_revision_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_rule_revision_response_data.py` & `fastly-2.3.0/fastly/model/waf_rule_revision_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_rule_revision_response_data_all_of.py` & `fastly-2.3.0/fastly/model/waf_rule_revision_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_rule_revisions_response.py` & `fastly-2.3.0/fastly/model/waf_rule_revisions_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_rule_revisions_response_all_of.py` & `fastly-2.3.0/fastly/model/waf_rule_revisions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_rules_response.py` & `fastly-2.3.0/fastly/model/waf_rules_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_rules_response_all_of.py` & `fastly-2.3.0/fastly/model/waf_tags_response_all_of.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.included_with_waf_rule import IncludedWithWafRule
-    from fastly.model.waf_rule_response_data import WafRuleResponseData
-    globals()['IncludedWithWafRule'] = IncludedWithWafRule
-    globals()['WafRuleResponseData'] = WafRuleResponseData
+    from fastly.model.waf_rule import WafRule
+    from fastly.model.waf_tags_response_data_item import WafTagsResponseDataItem
+    globals()['WafRule'] = WafRule
+    globals()['WafTagsResponseDataItem'] = WafTagsResponseDataItem
 
 
-class WafRulesResponseAllOf(ModelNormal):
+class WafTagsResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -83,16 +83,16 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([WafRuleResponseData],),  # noqa: E501
-            'included': (IncludedWithWafRule,),  # noqa: E501
+            'data': ([WafTagsResponseDataItem],),  # noqa: E501
+            'included': ([WafRule],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -105,15 +105,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafRulesResponseAllOf - a model defined in OpenAPI
+        """WafTagsResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,16 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([WafRuleResponseData]): [optional]  # noqa: E501
-            included (IncludedWithWafRule): [optional]  # noqa: E501
+            data ([WafTagsResponseDataItem]): [optional]  # noqa: E501
+            included ([WafRule]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -188,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafRulesResponseAllOf - a model defined in OpenAPI
+        """WafTagsResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -221,16 +221,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([WafRuleResponseData]): [optional]  # noqa: E501
-            included (IncludedWithWafRule): [optional]  # noqa: E501
+            data ([WafTagsResponseDataItem]): [optional]  # noqa: E501
+            included ([WafRule]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-2.2.2/fastly/model/waf_tag.py` & `fastly-2.3.0/fastly/model/waf_tag.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_tag_attributes.py` & `fastly-2.3.0/fastly/model/waf_tag_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_tags_response.py` & `fastly-2.3.0/fastly/model/waf_tags_response.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/waf_tags_response_all_of.py` & `fastly-2.3.0/fastly/model/ws_message_format.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,22 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from fastly.model.waf_rule import WafRule
-    from fastly.model.waf_tags_response_data_item import WafTagsResponseDataItem
-    globals()['WafRule'] = WafRule
-    globals()['WafTagsResponseDataItem'] = WafTagsResponseDataItem
 
-
-class WafTagsResponseAllOf(ModelNormal):
+class WsMessageFormat(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -66,54 +60,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'data': ([WafTagsResponseDataItem],),  # noqa: E501
-            'included': ([WafRule],),  # noqa: E501
+            'content': (str,),  # noqa: E501
+            'content_bin': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
-        'included': 'included',  # noqa: E501
+        'content': 'content',  # noqa: E501
+        'content_bin': 'content-bin',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafTagsResponseAllOf - a model defined in OpenAPI
+        """WsMessageFormat - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,16 +130,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([WafTagsResponseDataItem]): [optional]  # noqa: E501
-            included ([WafRule]): [optional]  # noqa: E501
+            content (str): The content of a WebSocket `TEXT` message.. [optional]  # noqa: E501
+            content_bin (str): The base64-encoded content of a WebSocket `BINARY` message.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -188,15 +180,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafTagsResponseAllOf - a model defined in OpenAPI
+        """WsMessageFormat - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -221,16 +213,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([WafTagsResponseDataItem]): [optional]  # noqa: E501
-            included ([WafRule]): [optional]  # noqa: E501
+            content (str): The content of a WebSocket `TEXT` message.. [optional]  # noqa: E501
+            content_bin (str): The base64-encoded content of a WebSocket `BINARY` message.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-2.2.2/fastly/model/waf_tags_response_data_item.py` & `fastly-2.3.0/fastly/model/waf_tags_response_data_item.py`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/fastly/model/ws_message_format.py` & `fastly-2.3.0/fastly/model/read_only_id_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class WsMessageFormat(ModelNormal):
+class ReadOnlyIdService(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -54,58 +54,48 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'content': (str,),  # noqa: E501
-            'content_bin': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'content': 'content',  # noqa: E501
-        'content_bin': 'content-bin',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WsMessageFormat - a model defined in OpenAPI
+        """ReadOnlyIdService - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -130,16 +120,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            content (str): The content of a WebSocket `TEXT` message.. [optional]  # noqa: E501
-            content_bin (str): The base64-encoded content of a WebSocket `BINARY` message.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -180,15 +168,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WsMessageFormat - a model defined in OpenAPI
+        """ReadOnlyIdService - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -213,16 +201,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            content (str): The content of a WebSocket `TEXT` message.. [optional]  # noqa: E501
-            content_bin (str): The base64-encoded content of a WebSocket `BINARY` message.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-2.2.2/fastly/models/__init__.py` & `fastly-2.3.0/fastly/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,16 +282,16 @@
 from fastly.model.publish_item_formats import PublishItemFormats
 from fastly.model.publish_request import PublishRequest
 from fastly.model.purge_keys import PurgeKeys
 from fastly.model.purge_keys_response import PurgeKeysResponse
 from fastly.model.purge_response import PurgeResponse
 from fastly.model.rate_limiter import RateLimiter
 from fastly.model.rate_limiter_response import RateLimiterResponse
-from fastly.model.rate_limiter_response1 import RateLimiterResponse1
 from fastly.model.rate_limiter_response_all_of import RateLimiterResponseAllOf
+from fastly.model.read_only_id_service import ReadOnlyIdService
 from fastly.model.realtime import Realtime
 from fastly.model.realtime_entry import RealtimeEntry
 from fastly.model.realtime_measurements import RealtimeMeasurements
 from fastly.model.relationship_common_name import RelationshipCommonName
 from fastly.model.relationship_customer import RelationshipCustomer
 from fastly.model.relationship_customer_customer import RelationshipCustomerCustomer
 from fastly.model.relationship_member_customer import RelationshipMemberCustomer
```

### Comparing `fastly-2.2.2/.gitignore` & `fastly-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/LICENSE` & `fastly-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastly-2.2.2/README.md` & `fastly-2.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -346,17 +346,19 @@
 *PoolApi* | [**update_server_pool**](docs/PoolApi.md#update_server_pool) | **PUT** /service/{service_id}/version/{version_id}/pool/{pool_name} | Update a server pool
 *PopApi* | [**list_pops**](docs/PopApi.md#list_pops) | **GET** /datacenters | List Fastly POPs
 *PublicIpListApi* | [**list_fastly_ips**](docs/PublicIpListApi.md#list_fastly_ips) | **GET** /public-ip-list | List Fastly&#39;s public IPs
 *PublishApi* | [**publish**](docs/PublishApi.md#publish) | **POST** /service/{service_id}/publish/ | Send messages to Fanout subscribers
 *PurgeApi* | [**purge_all**](docs/PurgeApi.md#purge_all) | **POST** /service/{service_id}/purge_all | Purge everything from a service
 *PurgeApi* | [**purge_single_url**](docs/PurgeApi.md#purge_single_url) | **POST** /purge/{cached_url} | Purge a URL
 *PurgeApi* | [**purge_tag**](docs/PurgeApi.md#purge_tag) | **POST** /service/{service_id}/purge/{surrogate_key} | Purge by surrogate key tag
+*RateLimiterApi* | [**create_rate_limiter**](docs/RateLimiterApi.md#create_rate_limiter) | **POST** /service/{service_id}/version/{version_id}/rate-limiters | Create a rate limiter
 *RateLimiterApi* | [**delete_rate_limiter**](docs/RateLimiterApi.md#delete_rate_limiter) | **DELETE** /rate-limiters/{rate_limiter_id} | Delete a rate limiter
 *RateLimiterApi* | [**get_rate_limiter**](docs/RateLimiterApi.md#get_rate_limiter) | **GET** /rate-limiters/{rate_limiter_id} | Get a rate limiter
 *RateLimiterApi* | [**list_rate_limiters**](docs/RateLimiterApi.md#list_rate_limiters) | **GET** /service/{service_id}/version/{version_id}/rate-limiters | List rate limiters
+*RateLimiterApi* | [**update_rate_limiter**](docs/RateLimiterApi.md#update_rate_limiter) | **PUT** /rate-limiters/{rate_limiter_id} | Update a rate limiter
 *RealtimeApi* | [**get_stats_last120_seconds**](docs/RealtimeApi.md#get_stats_last120_seconds) | **GET** /v1/channel/{service_id}/ts/h | Get real-time data for the last 120 seconds
 *RealtimeApi* | [**get_stats_last120_seconds_limit_entries**](docs/RealtimeApi.md#get_stats_last120_seconds_limit_entries) | **GET** /v1/channel/{service_id}/ts/h/limit/{max_entries} | Get a limited number of real-time data entries
 *RealtimeApi* | [**get_stats_last_second**](docs/RealtimeApi.md#get_stats_last_second) | **GET** /v1/channel/{service_id}/ts/{timestamp_in_seconds} | Get real-time data from specified time
 *RequestSettingsApi* | [**delete_request_settings**](docs/RequestSettingsApi.md#delete_request_settings) | **DELETE** /service/{service_id}/version/{version_id}/request_settings/{request_settings_name} | Delete a Request Settings object
 *RequestSettingsApi* | [**get_request_settings**](docs/RequestSettingsApi.md#get_request_settings) | **GET** /service/{service_id}/version/{version_id}/request_settings/{request_settings_name} | Get a Request Settings object
 *RequestSettingsApi* | [**list_request_settings**](docs/RequestSettingsApi.md#list_request_settings) | **GET** /service/{service_id}/version/{version_id}/request_settings | List Request Settings objects
 *RequestSettingsApi* | [**update_request_settings**](docs/RequestSettingsApi.md#update_request_settings) | **PUT** /service/{service_id}/version/{version_id}/request_settings/{request_settings_name} | Update a Request Settings object
@@ -501,15 +503,14 @@
 - [`/automation-tokens/{id}`](https://developer.fastly.com/reference/api/auth-tokens/automation) (DELETE, GET)
 - [`/automation-tokens`](https://developer.fastly.com/reference/api/auth-tokens/automation) (GET, POST)
 - [`/customer/{customer_id}/contacts`](https://developer.fastly.com/reference/api/account/contact) (POST)
 - [`/docs/section/{section}`](https://developer.fastly.com/reference/api/utils/docs) (GET)
 - [`/docs/subject/{subject}`](https://developer.fastly.com/reference/api/utils/docs) (GET)
 - [`/metrics/domains/services/{service_id}`](https://developer.fastly.com/reference/api/metrics-stats/domain-inspector/historical) (GET)
 - [`/metrics/origins/services/{service_id}`](https://developer.fastly.com/reference/api/metrics-stats/origin-inspector/historical) (GET)
-- [`/rate-limiters/{rate_limiter_id}`](https://developer.fastly.com/reference/api/vcl-services/rate-limiter) (PUT)
 - [`/resources/stores/secret/client-key`](https://developer.fastly.com/reference/api/services/resources/secret-store) (POST)
 - [`/resources/stores/secret/signing-key`](https://developer.fastly.com/reference/api/services/resources/secret-store) (GET)
 - [`/resources/stores/secret/{store_id}/secrets/{secret_name}`](https://developer.fastly.com/reference/api/services/resources/secret) (DELETE, GET)
 - [`/resources/stores/secret/{store_id}/secrets`](https://developer.fastly.com/reference/api/services/resources/secret) (GET, PATCH, POST, PUT)
 - [`/resources/stores/secret/{store_id}`](https://developer.fastly.com/reference/api/services/resources/secret-store) (DELETE, GET)
 - [`/resources/stores/secret`](https://developer.fastly.com/reference/api/services/resources/secret-store) (GET, POST)
 - [`/roles/{role_id}/permissions`](https://developer.fastly.com/reference/api/account/roles) (DELETE, POST)
@@ -521,15 +522,14 @@
 - [`/service-groups`](https://developer.fastly.com/reference/api/account/service-groups) (POST)
 - [`/service/{service_id}/purge`](https://developer.fastly.com/reference/api/purging) (POST)
 - [`/service/{service_id}/version/{version_id}/apex-redirects`](https://developer.fastly.com/reference/api/vcl-services/apex-redirect) (POST)
 - [`/service/{service_id}/version/{version_id}/director/{director_name}`](https://developer.fastly.com/reference/api/load-balancing/directors/director) (PUT)
 - [`/service/{service_id}/version/{version_id}/generated_vcl/content`](https://developer.fastly.com/reference/api/vcl-services/vcl) (GET)
 - [`/service/{service_id}/version/{version_id}/logging/kafka/{logging_kafka_name}`](https://developer.fastly.com/reference/api/logging/kafka) (PUT)
 - [`/service/{service_id}/version/{version_id}/logging/kinesis/{logging_kinesis_name}`](https://developer.fastly.com/reference/api/logging/kinesis) (PUT)
-- [`/service/{service_id}/version/{version_id}/rate-limiters`](https://developer.fastly.com/reference/api/vcl-services/rate-limiter) (POST)
 - [`/service/{service_id}/version/{version_id}/request_settings`](https://developer.fastly.com/reference/api/vcl-services/request-settings) (POST)
 - [`/service/{service_id}/version/{version_id}/response_object/{response_object_name}`](https://developer.fastly.com/reference/api/vcl-services/response-object) (PUT)
 - [`/service/{service_id}/version/{version_id}/response_object`](https://developer.fastly.com/reference/api/vcl-services/response-object) (POST)
 - [`/service/{service_id}/version/{version_id}/snippet/{snippet_name}`](https://developer.fastly.com/reference/api/vcl-services/snippet) (PUT)
 - [`/service/{service_id}/version/{version_id}/vcl/{vcl_name}/content`](https://developer.fastly.com/reference/api/vcl-services/vcl) (GET)
 - [`/service/{service_id}/version/{version_id}/wafs/{firewall_id}`](https://developer.fastly.com/reference/api/legacy-waf/firewall) (GET, PATCH)
 - [`/service/{service_id}/version/{version_id}/wafs`](https://developer.fastly.com/reference/api/legacy-waf/firewall) (GET, POST)
```

### Comparing `fastly-2.2.2/pyproject.toml` & `fastly-2.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastly"
-version = "2.2.2"
+version = "2.3.0"
 authors = [{ name = "Fastly", email = "oss@fastly.com" }]
 description = "A Python Fastly API client library"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `fastly-2.2.2/PKG-INFO` & `fastly-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastly
-Version: 2.2.2
+Version: 2.3.0
 Summary: A Python Fastly API client library
 Project-URL: Homepage, https://github.com/fastly/fastly-py
 Project-URL: Bug Tracker, https://github.com/fastly/fastly-py/issues
 Author-email: Fastly <oss@fastly.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -360,17 +360,19 @@
 *PoolApi* | [**update_server_pool**](docs/PoolApi.md#update_server_pool) | **PUT** /service/{service_id}/version/{version_id}/pool/{pool_name} | Update a server pool
 *PopApi* | [**list_pops**](docs/PopApi.md#list_pops) | **GET** /datacenters | List Fastly POPs
 *PublicIpListApi* | [**list_fastly_ips**](docs/PublicIpListApi.md#list_fastly_ips) | **GET** /public-ip-list | List Fastly&#39;s public IPs
 *PublishApi* | [**publish**](docs/PublishApi.md#publish) | **POST** /service/{service_id}/publish/ | Send messages to Fanout subscribers
 *PurgeApi* | [**purge_all**](docs/PurgeApi.md#purge_all) | **POST** /service/{service_id}/purge_all | Purge everything from a service
 *PurgeApi* | [**purge_single_url**](docs/PurgeApi.md#purge_single_url) | **POST** /purge/{cached_url} | Purge a URL
 *PurgeApi* | [**purge_tag**](docs/PurgeApi.md#purge_tag) | **POST** /service/{service_id}/purge/{surrogate_key} | Purge by surrogate key tag
+*RateLimiterApi* | [**create_rate_limiter**](docs/RateLimiterApi.md#create_rate_limiter) | **POST** /service/{service_id}/version/{version_id}/rate-limiters | Create a rate limiter
 *RateLimiterApi* | [**delete_rate_limiter**](docs/RateLimiterApi.md#delete_rate_limiter) | **DELETE** /rate-limiters/{rate_limiter_id} | Delete a rate limiter
 *RateLimiterApi* | [**get_rate_limiter**](docs/RateLimiterApi.md#get_rate_limiter) | **GET** /rate-limiters/{rate_limiter_id} | Get a rate limiter
 *RateLimiterApi* | [**list_rate_limiters**](docs/RateLimiterApi.md#list_rate_limiters) | **GET** /service/{service_id}/version/{version_id}/rate-limiters | List rate limiters
+*RateLimiterApi* | [**update_rate_limiter**](docs/RateLimiterApi.md#update_rate_limiter) | **PUT** /rate-limiters/{rate_limiter_id} | Update a rate limiter
 *RealtimeApi* | [**get_stats_last120_seconds**](docs/RealtimeApi.md#get_stats_last120_seconds) | **GET** /v1/channel/{service_id}/ts/h | Get real-time data for the last 120 seconds
 *RealtimeApi* | [**get_stats_last120_seconds_limit_entries**](docs/RealtimeApi.md#get_stats_last120_seconds_limit_entries) | **GET** /v1/channel/{service_id}/ts/h/limit/{max_entries} | Get a limited number of real-time data entries
 *RealtimeApi* | [**get_stats_last_second**](docs/RealtimeApi.md#get_stats_last_second) | **GET** /v1/channel/{service_id}/ts/{timestamp_in_seconds} | Get real-time data from specified time
 *RequestSettingsApi* | [**delete_request_settings**](docs/RequestSettingsApi.md#delete_request_settings) | **DELETE** /service/{service_id}/version/{version_id}/request_settings/{request_settings_name} | Delete a Request Settings object
 *RequestSettingsApi* | [**get_request_settings**](docs/RequestSettingsApi.md#get_request_settings) | **GET** /service/{service_id}/version/{version_id}/request_settings/{request_settings_name} | Get a Request Settings object
 *RequestSettingsApi* | [**list_request_settings**](docs/RequestSettingsApi.md#list_request_settings) | **GET** /service/{service_id}/version/{version_id}/request_settings | List Request Settings objects
 *RequestSettingsApi* | [**update_request_settings**](docs/RequestSettingsApi.md#update_request_settings) | **PUT** /service/{service_id}/version/{version_id}/request_settings/{request_settings_name} | Update a Request Settings object
@@ -515,15 +517,14 @@
 - [`/automation-tokens/{id}`](https://developer.fastly.com/reference/api/auth-tokens/automation) (DELETE, GET)
 - [`/automation-tokens`](https://developer.fastly.com/reference/api/auth-tokens/automation) (GET, POST)
 - [`/customer/{customer_id}/contacts`](https://developer.fastly.com/reference/api/account/contact) (POST)
 - [`/docs/section/{section}`](https://developer.fastly.com/reference/api/utils/docs) (GET)
 - [`/docs/subject/{subject}`](https://developer.fastly.com/reference/api/utils/docs) (GET)
 - [`/metrics/domains/services/{service_id}`](https://developer.fastly.com/reference/api/metrics-stats/domain-inspector/historical) (GET)
 - [`/metrics/origins/services/{service_id}`](https://developer.fastly.com/reference/api/metrics-stats/origin-inspector/historical) (GET)
-- [`/rate-limiters/{rate_limiter_id}`](https://developer.fastly.com/reference/api/vcl-services/rate-limiter) (PUT)
 - [`/resources/stores/secret/client-key`](https://developer.fastly.com/reference/api/services/resources/secret-store) (POST)
 - [`/resources/stores/secret/signing-key`](https://developer.fastly.com/reference/api/services/resources/secret-store) (GET)
 - [`/resources/stores/secret/{store_id}/secrets/{secret_name}`](https://developer.fastly.com/reference/api/services/resources/secret) (DELETE, GET)
 - [`/resources/stores/secret/{store_id}/secrets`](https://developer.fastly.com/reference/api/services/resources/secret) (GET, PATCH, POST, PUT)
 - [`/resources/stores/secret/{store_id}`](https://developer.fastly.com/reference/api/services/resources/secret-store) (DELETE, GET)
 - [`/resources/stores/secret`](https://developer.fastly.com/reference/api/services/resources/secret-store) (GET, POST)
 - [`/roles/{role_id}/permissions`](https://developer.fastly.com/reference/api/account/roles) (DELETE, POST)
@@ -535,15 +536,14 @@
 - [`/service-groups`](https://developer.fastly.com/reference/api/account/service-groups) (POST)
 - [`/service/{service_id}/purge`](https://developer.fastly.com/reference/api/purging) (POST)
 - [`/service/{service_id}/version/{version_id}/apex-redirects`](https://developer.fastly.com/reference/api/vcl-services/apex-redirect) (POST)
 - [`/service/{service_id}/version/{version_id}/director/{director_name}`](https://developer.fastly.com/reference/api/load-balancing/directors/director) (PUT)
 - [`/service/{service_id}/version/{version_id}/generated_vcl/content`](https://developer.fastly.com/reference/api/vcl-services/vcl) (GET)
 - [`/service/{service_id}/version/{version_id}/logging/kafka/{logging_kafka_name}`](https://developer.fastly.com/reference/api/logging/kafka) (PUT)
 - [`/service/{service_id}/version/{version_id}/logging/kinesis/{logging_kinesis_name}`](https://developer.fastly.com/reference/api/logging/kinesis) (PUT)
-- [`/service/{service_id}/version/{version_id}/rate-limiters`](https://developer.fastly.com/reference/api/vcl-services/rate-limiter) (POST)
 - [`/service/{service_id}/version/{version_id}/request_settings`](https://developer.fastly.com/reference/api/vcl-services/request-settings) (POST)
 - [`/service/{service_id}/version/{version_id}/response_object/{response_object_name}`](https://developer.fastly.com/reference/api/vcl-services/response-object) (PUT)
 - [`/service/{service_id}/version/{version_id}/response_object`](https://developer.fastly.com/reference/api/vcl-services/response-object) (POST)
 - [`/service/{service_id}/version/{version_id}/snippet/{snippet_name}`](https://developer.fastly.com/reference/api/vcl-services/snippet) (PUT)
 - [`/service/{service_id}/version/{version_id}/vcl/{vcl_name}/content`](https://developer.fastly.com/reference/api/vcl-services/vcl) (GET)
 - [`/service/{service_id}/version/{version_id}/wafs/{firewall_id}`](https://developer.fastly.com/reference/api/legacy-waf/firewall) (GET, PATCH)
 - [`/service/{service_id}/version/{version_id}/wafs`](https://developer.fastly.com/reference/api/legacy-waf/firewall) (GET, POST)
```

