# Comparing `tmp/splitit_web_python_sdk-2.4.0.tar.gz` & `tmp/splitit_web_python_sdk-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splitit_web_python_sdk-2.4.0.tar", max compression
+gzip compressed data, was "splitit_web_python_sdk-2.5.0.tar", max compression
```

## Comparing `splitit_web_python_sdk-2.4.0.tar` & `splitit_web_python_sdk-2.5.0.tar`

### file list

```diff
@@ -1,228 +1,249 @@
--rw-r--r--   0        0        0     1081 2023-06-21 16:10:41.533167 splitit_web_python_sdk-2.4.0/LICENSE
--rw-r--r--   0        0        0     8431 2023-06-21 16:10:41.589259 splitit_web_python_sdk-2.4.0/README.md
--rw-r--r--   0        0        0      737 2023-06-21 16:10:41.483983 splitit_web_python_sdk-2.4.0/pyproject.toml
--rw-r--r--   0        0        0      725 2023-06-21 16:10:41.484375 splitit_web_python_sdk-2.4.0/splitit_client/__init__.py
--rw-r--r--   0        0        0    72963 2023-06-21 16:10:41.484593 splitit_web_python_sdk-2.4.0/splitit_client/api_client.py
--rw-r--r--   0        0        0      663 2023-06-21 16:10:41.484792 splitit_web_python_sdk-2.4.0/splitit_client/api_response.py
--rw-r--r--   0        0        0      214 2023-06-21 16:10:41.484922 splitit_web_python_sdk-2.4.0/splitit_client/apis/__init__.py
--rw-r--r--   0        0        0     3411 2023-06-21 16:10:41.485039 splitit_web_python_sdk-2.4.0/splitit_client/apis/path_to_api.py
--rw-r--r--   0        0        0      241 2023-06-21 16:10:41.485173 splitit_web_python_sdk-2.4.0/splitit_client/apis/paths/__init__.py
--rw-r--r--   0        0        0      127 2023-06-21 16:10:41.485279 splitit_web_python_sdk-2.4.0/splitit_client/apis/paths/api_installmentplans.py
--rw-r--r--   0        0        0      161 2023-06-21 16:10:41.485421 splitit_web_python_sdk-2.4.0/splitit_client/apis/paths/api_installmentplans_check_eligibility.py
--rw-r--r--   0        0        0      144 2023-06-21 16:10:41.485549 splitit_web_python_sdk-2.4.0/splitit_client/apis/paths/api_installmentplans_initiate.py
--rw-r--r--   0        0        0      169 2023-06-21 16:10:41.485674 splitit_web_python_sdk-2.4.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number.py
--rw-r--r--   0        0        0      185 2023-06-21 16:10:41.485802 splitit_web_python_sdk-2.4.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_cancel.py
--rw-r--r--   0        0        0      185 2023-06-21 16:10:41.485969 splitit_web_python_sdk-2.4.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_refund.py
--rw-r--r--   0        0        0      192 2023-06-21 16:10:41.486123 splitit_web_python_sdk-2.4.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_updateorder.py
--rw-r--r--   0        0        0      208 2023-06-21 16:10:41.486273 splitit_web_python_sdk-2.4.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_verifyauthorization.py
--rw-r--r--   0        0        0      137 2023-06-21 16:10:41.486397 splitit_web_python_sdk-2.4.0/splitit_client/apis/paths/api_installmentplans_search.py
--rw-r--r--   0        0        0      147 2023-06-21 16:10:41.486527 splitit_web_python_sdk-2.4.0/splitit_client/apis/paths/api_installmentplans_updateorder.py
--rw-r--r--   0        0        0      371 2023-06-21 16:10:41.486651 splitit_web_python_sdk-2.4.0/splitit_client/apis/tag_to_api.py
--rw-r--r--   0        0        0      328 2023-06-21 16:10:41.486785 splitit_web_python_sdk-2.4.0/splitit_client/apis/tags/__init__.py
--rw-r--r--   0        0        0     1333 2023-06-21 16:10:41.486915 splitit_web_python_sdk-2.4.0/splitit_client/apis/tags/installment_plan_api.py
--rw-r--r--   0        0        0      989 2023-06-21 16:10:41.487033 splitit_web_python_sdk-2.4.0/splitit_client/client.py
--rw-r--r--   0        0        0      989 2023-06-21 16:10:41.487141 splitit_web_python_sdk-2.4.0/splitit_client/client.pyi
--rw-r--r--   0        0        0      669 2023-06-21 16:10:41.487247 splitit_web_python_sdk-2.4.0/splitit_client/client_custom.py
--rw-r--r--   0        0        0    18575 2023-06-21 16:10:41.487387 splitit_web_python_sdk-2.4.0/splitit_client/configuration.py
--rw-r--r--   0        0        0     7672 2023-06-21 16:10:41.487526 splitit_web_python_sdk-2.4.0/splitit_client/exceptions.py
--rw-r--r--   0        0        0     2274 2023-06-21 16:10:41.487650 splitit_web_python_sdk-2.4.0/splitit_client/exceptions_base.py
--rw-r--r--   0        0        0      348 2023-06-21 16:10:41.487841 splitit_web_python_sdk-2.4.0/splitit_client/model/__init__.py
--rw-r--r--   0        0        0     4871 2023-06-21 16:10:41.487939 splitit_web_python_sdk-2.4.0/splitit_client/model/address_data.py
--rw-r--r--   0        0        0     4871 2023-06-21 16:10:41.488052 splitit_web_python_sdk-2.4.0/splitit_client/model/address_data.pyi
--rw-r--r--   0        0        0     4894 2023-06-21 16:10:41.488166 splitit_web_python_sdk-2.4.0/splitit_client/model/address_data_model.py
--rw-r--r--   0        0        0     4894 2023-06-21 16:10:41.488372 splitit_web_python_sdk-2.4.0/splitit_client/model/address_data_model.pyi
--rw-r--r--   0        0        0     7418 2023-06-21 16:10:41.488564 splitit_web_python_sdk-2.4.0/splitit_client/model/authorization_model.py
--rw-r--r--   0        0        0     7418 2023-06-21 16:10:41.488675 splitit_web_python_sdk-2.4.0/splitit_client/model/authorization_model.pyi
--rw-r--r--   0        0        0     1752 2023-06-21 16:10:41.488787 splitit_web_python_sdk-2.4.0/splitit_client/model/card_brand.py
--rw-r--r--   0        0        0     1392 2023-06-21 16:10:41.488902 splitit_web_python_sdk-2.4.0/splitit_client/model/card_brand.pyi
--rw-r--r--   0        0        0     5874 2023-06-21 16:10:41.489009 splitit_web_python_sdk-2.4.0/splitit_client/model/card_data.py
--rw-r--r--   0        0        0     5874 2023-06-21 16:10:41.489134 splitit_web_python_sdk-2.4.0/splitit_client/model/card_data.pyi
--rw-r--r--   0        0        0     1571 2023-06-21 16:10:41.489239 splitit_web_python_sdk-2.4.0/splitit_client/model/card_type.py
--rw-r--r--   0        0        0     1251 2023-06-21 16:10:41.489781 splitit_web_python_sdk-2.4.0/splitit_client/model/card_type.pyi
--rw-r--r--   0        0        0     3738 2023-06-21 16:10:41.490145 splitit_web_python_sdk-2.4.0/splitit_client/model/check_installments_eligibility_request.py
--rw-r--r--   0        0        0     3738 2023-06-21 16:10:41.490305 splitit_web_python_sdk-2.4.0/splitit_client/model/check_installments_eligibility_request.pyi
--rw-r--r--   0        0        0     3357 2023-06-21 16:10:41.490450 splitit_web_python_sdk-2.4.0/splitit_client/model/error.py
--rw-r--r--   0        0        0     3357 2023-06-21 16:10:41.490604 splitit_web_python_sdk-2.4.0/splitit_client/model/error.pyi
--rw-r--r--   0        0        0     5464 2023-06-21 16:10:41.490749 splitit_web_python_sdk-2.4.0/splitit_client/model/error_extended.py
--rw-r--r--   0        0        0     5464 2023-06-21 16:10:41.490878 splitit_web_python_sdk-2.4.0/splitit_client/model/error_extended.pyi
--rw-r--r--   0        0        0     2403 2023-06-21 16:10:41.491165 splitit_web_python_sdk-2.4.0/splitit_client/model/events_endpoints_model.py
--rw-r--r--   0        0        0     2403 2023-06-21 16:10:41.491371 splitit_web_python_sdk-2.4.0/splitit_client/model/events_endpoints_model.pyi
--rw-r--r--   0        0        0     2898 2023-06-21 16:10:41.491515 splitit_web_python_sdk-2.4.0/splitit_client/model/failed_response.py
--rw-r--r--   0        0        0     2898 2023-06-21 16:10:41.491700 splitit_web_python_sdk-2.4.0/splitit_client/model/failed_response.pyi
--rw-r--r--   0        0        0     1188 2023-06-21 16:10:41.491880 splitit_web_python_sdk-2.4.0/splitit_client/model/gw_authorization_status.py
--rw-r--r--   0        0        0      991 2023-06-21 16:10:41.492025 splitit_web_python_sdk-2.4.0/splitit_client/model/gw_authorization_status.pyi
--rw-r--r--   0        0        0     4856 2023-06-21 16:10:41.492201 splitit_web_python_sdk-2.4.0/splitit_client/model/identifier_contract.py
--rw-r--r--   0        0        0     4856 2023-06-21 16:10:41.492384 splitit_web_python_sdk-2.4.0/splitit_client/model/identifier_contract.pyi
--rw-r--r--   0        0        0     9111 2023-06-21 16:10:41.492538 splitit_web_python_sdk-2.4.0/splitit_client/model/initiate_plan_response.py
--rw-r--r--   0        0        0     9111 2023-06-21 16:10:41.492740 splitit_web_python_sdk-2.4.0/splitit_client/model/initiate_plan_response.pyi
--rw-r--r--   0        0        0     3361 2023-06-21 16:10:41.492914 splitit_web_python_sdk-2.4.0/splitit_client/model/initiate_redirection_endpoints_model.py
--rw-r--r--   0        0        0     3361 2023-06-21 16:10:41.493071 splitit_web_python_sdk-2.4.0/splitit_client/model/initiate_redirection_endpoints_model.pyi
--rw-r--r--   0        0        0     4303 2023-06-21 16:10:41.493216 splitit_web_python_sdk-2.4.0/splitit_client/model/installment.py
--rw-r--r--   0        0        0     4303 2023-06-21 16:10:41.493336 splitit_web_python_sdk-2.4.0/splitit_client/model/installment.pyi
--rw-r--r--   0        0        0     2499 2023-06-21 16:10:41.493504 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_cancel_response.py
--rw-r--r--   0        0        0     2499 2023-06-21 16:10:41.493659 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_cancel_response.pyi
--rw-r--r--   0        0        0     8108 2023-06-21 16:10:41.493824 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_create_request.py
--rw-r--r--   0        0        0     8108 2023-06-21 16:10:41.493996 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_create_request.pyi
--rw-r--r--   0        0        0    13350 2023-06-21 16:10:41.494147 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_create_response.py
--rw-r--r--   0        0        0    13350 2023-06-21 16:10:41.494344 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_create_response.pyi
--rw-r--r--   0        0        0    14794 2023-06-21 16:10:41.494519 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_get_response.py
--rw-r--r--   0        0        0    14794 2023-06-21 16:10:41.494694 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_get_response.pyi
--rw-r--r--   0        0        0     7288 2023-06-21 16:10:41.494850 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_initiate_request.py
--rw-r--r--   0        0        0     7288 2023-06-21 16:10:41.494968 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_initiate_request.pyi
--rw-r--r--   0        0        0     3076 2023-06-21 16:10:41.495083 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_refund_request.py
--rw-r--r--   0        0        0     3076 2023-06-21 16:10:41.495206 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_refund_request.pyi
--rw-r--r--   0        0        0     5607 2023-06-21 16:10:41.495310 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_refund_response.py
--rw-r--r--   0        0        0     5607 2023-06-21 16:10:41.495420 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_refund_response.pyi
--rw-r--r--   0        0        0     3421 2023-06-21 16:10:41.495508 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_search_response.py
--rw-r--r--   0        0        0     3421 2023-06-21 16:10:41.495597 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_search_response.pyi
--rw-r--r--   0        0        0     4250 2023-06-21 16:10:41.495685 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_update_request.py
--rw-r--r--   0        0        0     4250 2023-06-21 16:10:41.495772 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_update_request.pyi
--rw-r--r--   0        0        0     4385 2023-06-21 16:10:41.495861 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_update_request_by_identifier.py
--rw-r--r--   0        0        0     4385 2023-06-21 16:10:41.495947 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_update_request_by_identifier.pyi
--rw-r--r--   0        0        0     4417 2023-06-21 16:10:41.496044 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_update_response.py
--rw-r--r--   0        0        0     4417 2023-06-21 16:10:41.496153 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_update_response.pyi
--rw-r--r--   0        0        0     1082 2023-06-21 16:10:41.498597 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_status.py
--rw-r--r--   0        0        0      911 2023-06-21 16:10:41.498850 splitit_web_python_sdk-2.4.0/splitit_client/model/installment_status.pyi
--rw-r--r--   0        0        0     4161 2023-06-21 16:10:41.498964 splitit_web_python_sdk-2.4.0/splitit_client/model/installments_eligibility_response.py
--rw-r--r--   0        0        0     4161 2023-06-21 16:10:41.499061 splitit_web_python_sdk-2.4.0/splitit_client/model/installments_eligibility_response.pyi
--rw-r--r--   0        0        0     4052 2023-06-21 16:10:41.499158 splitit_web_python_sdk-2.4.0/splitit_client/model/links_data.py
--rw-r--r--   0        0        0     4052 2023-06-21 16:10:41.499250 splitit_web_python_sdk-2.4.0/splitit_client/model/links_data.pyi
--rw-r--r--   0        0        0     3679 2023-06-21 16:10:41.499338 splitit_web_python_sdk-2.4.0/splitit_client/model/links_model.py
--rw-r--r--   0        0        0     3679 2023-06-21 16:10:41.499439 splitit_web_python_sdk-2.4.0/splitit_client/model/links_model.pyi
--rw-r--r--   0        0        0     3476 2023-06-21 16:10:41.499548 splitit_web_python_sdk-2.4.0/splitit_client/model/payment_method_model.py
--rw-r--r--   0        0        0     3476 2023-06-21 16:10:41.499662 splitit_web_python_sdk-2.4.0/splitit_client/model/payment_method_model.pyi
--rw-r--r--   0        0        0      962 2023-06-21 16:10:41.499752 splitit_web_python_sdk-2.4.0/splitit_client/model/payment_method_type.py
--rw-r--r--   0        0        0      826 2023-06-21 16:10:41.499853 splitit_web_python_sdk-2.4.0/splitit_client/model/payment_method_type.pyi
--rw-r--r--   0        0        0     6852 2023-06-21 16:10:41.499953 splitit_web_python_sdk-2.4.0/splitit_client/model/payment_plan_option_model.py
--rw-r--r--   0        0        0     6852 2023-06-21 16:10:41.500052 splitit_web_python_sdk-2.4.0/splitit_client/model/payment_plan_option_model.pyi
--rw-r--r--   0        0        0    10239 2023-06-21 16:10:41.500184 splitit_web_python_sdk-2.4.0/splitit_client/model/plan_data.py
--rw-r--r--   0        0        0    10239 2023-06-21 16:10:41.500363 splitit_web_python_sdk-2.4.0/splitit_client/model/plan_data.pyi
--rw-r--r--   0        0        0     8734 2023-06-21 16:10:41.500577 splitit_web_python_sdk-2.4.0/splitit_client/model/plan_data_model.py
--rw-r--r--   0        0        0     8734 2023-06-21 16:10:41.500802 splitit_web_python_sdk-2.4.0/splitit_client/model/plan_data_model.pyi
--rw-r--r--   0        0        0     4276 2023-06-21 16:10:41.500978 splitit_web_python_sdk-2.4.0/splitit_client/model/plan_error_response.py
--rw-r--r--   0        0        0     4276 2023-06-21 16:10:41.503418 splitit_web_python_sdk-2.4.0/splitit_client/model/plan_error_response.pyi
--rw-r--r--   0        0        0     1345 2023-06-21 16:10:41.504271 splitit_web_python_sdk-2.4.0/splitit_client/model/plan_status.py
--rw-r--r--   0        0        0     1089 2023-06-21 16:10:41.504379 splitit_web_python_sdk-2.4.0/splitit_client/model/plan_status.pyi
--rw-r--r--   0        0        0     1091 2023-06-21 16:10:41.504476 splitit_web_python_sdk-2.4.0/splitit_client/model/purchase_method.py
--rw-r--r--   0        0        0      914 2023-06-21 16:10:41.504569 splitit_web_python_sdk-2.4.0/splitit_client/model/purchase_method.pyi
--rw-r--r--   0        0        0     4123 2023-06-21 16:10:41.504667 splitit_web_python_sdk-2.4.0/splitit_client/model/redirection_endpoints_model.py
--rw-r--r--   0        0        0     4123 2023-06-21 16:10:41.504758 splitit_web_python_sdk-2.4.0/splitit_client/model/redirection_endpoints_model.pyi
--rw-r--r--   0        0        0     5623 2023-06-21 16:10:41.504845 splitit_web_python_sdk-2.4.0/splitit_client/model/refund_model.py
--rw-r--r--   0        0        0     5623 2023-06-21 16:10:41.504931 splitit_web_python_sdk-2.4.0/splitit_client/model/refund_model.pyi
--rw-r--r--   0        0        0     1069 2023-06-21 16:10:41.505019 splitit_web_python_sdk-2.4.0/splitit_client/model/refund_status.py
--rw-r--r--   0        0        0      902 2023-06-21 16:10:41.505102 splitit_web_python_sdk-2.4.0/splitit_client/model/refund_status.pyi
--rw-r--r--   0        0        0     1485 2023-06-21 16:10:41.505189 splitit_web_python_sdk-2.4.0/splitit_client/model/refund_strategy.py
--rw-r--r--   0        0        0     1136 2023-06-21 16:10:41.505278 splitit_web_python_sdk-2.4.0/splitit_client/model/refund_strategy.pyi
--rw-r--r--   0        0        0     4246 2023-06-21 16:10:41.505372 splitit_web_python_sdk-2.4.0/splitit_client/model/refund_summary.py
--rw-r--r--   0        0        0     4246 2023-06-21 16:10:41.505475 splitit_web_python_sdk-2.4.0/splitit_client/model/refund_summary.pyi
--rw-r--r--   0        0        0    14808 2023-06-21 16:10:41.505605 splitit_web_python_sdk-2.4.0/splitit_client/model/search_installment_plan_response_item.py
--rw-r--r--   0        0        0    14808 2023-06-21 16:10:41.505757 splitit_web_python_sdk-2.4.0/splitit_client/model/search_installment_plan_response_item.pyi
--rw-r--r--   0        0        0     1075 2023-06-21 16:10:41.505891 splitit_web_python_sdk-2.4.0/splitit_client/model/shipping_status.py
--rw-r--r--   0        0        0      906 2023-06-21 16:10:41.506002 splitit_web_python_sdk-2.4.0/splitit_client/model/shipping_status.pyi
--rw-r--r--   0        0        0      958 2023-06-21 16:10:41.506110 splitit_web_python_sdk-2.4.0/splitit_client/model/shipping_status2.py
--rw-r--r--   0        0        0      823 2023-06-21 16:10:41.506209 splitit_web_python_sdk-2.4.0/splitit_client/model/shipping_status2.pyi
--rw-r--r--   0        0        0     3874 2023-06-21 16:10:41.506316 splitit_web_python_sdk-2.4.0/splitit_client/model/shopper_data.py
--rw-r--r--   0        0        0     3874 2023-06-21 16:10:41.506461 splitit_web_python_sdk-2.4.0/splitit_client/model/shopper_data.pyi
--rw-r--r--   0        0        0     1168 2023-06-21 16:10:41.507093 splitit_web_python_sdk-2.4.0/splitit_client/model/test_modes.py
--rw-r--r--   0        0        0      975 2023-06-21 16:10:41.507260 splitit_web_python_sdk-2.4.0/splitit_client/model/test_modes.pyi
--rw-r--r--   0        0        0     4386 2023-06-21 16:10:41.509605 splitit_web_python_sdk-2.4.0/splitit_client/model/three_ds_redirect_data_v3.py
--rw-r--r--   0        0        0     4386 2023-06-21 16:10:41.510682 splitit_web_python_sdk-2.4.0/splitit_client/model/three_ds_redirect_data_v3.pyi
--rw-r--r--   0        0        0     4223 2023-06-21 16:10:41.510842 splitit_web_python_sdk-2.4.0/splitit_client/model/update_order_request.py
--rw-r--r--   0        0        0     4223 2023-06-21 16:10:41.510959 splitit_web_python_sdk-2.4.0/splitit_client/model/update_order_request.pyi
--rw-r--r--   0        0        0     3409 2023-06-21 16:10:41.511062 splitit_web_python_sdk-2.4.0/splitit_client/model/ux_settings_model.py
--rw-r--r--   0        0        0     3409 2023-06-21 16:10:41.511156 splitit_web_python_sdk-2.4.0/splitit_client/model/ux_settings_model.pyi
--rw-r--r--   0        0        0     3864 2023-06-21 16:10:41.511257 splitit_web_python_sdk-2.4.0/splitit_client/model/verify_authorization_response.py
--rw-r--r--   0        0        0     3864 2023-06-21 16:10:41.511350 splitit_web_python_sdk-2.4.0/splitit_client/model/verify_authorization_response.pyi
--rw-r--r--   0        0        0     4366 2023-06-21 16:10:41.511467 splitit_web_python_sdk-2.4.0/splitit_client/models/__init__.py
--rw-r--r--   0        0        0     1223 2023-06-21 16:10:41.511566 splitit_web_python_sdk-2.4.0/splitit_client/paths/__init__.py
--rw-r--r--   0        0        0      327 2023-06-21 16:10:41.511687 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans/__init__.py
--rw-r--r--   0        0        0    28553 2023-06-21 16:10:41.511900 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans/post.py
--rw-r--r--   0        0        0    28104 2023-06-21 16:10:41.512059 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans/post.pyi
--rw-r--r--   0        0        0      362 2023-06-21 16:10:41.512189 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_check_eligibility/__init__.py
--rw-r--r--   0        0        0    22133 2023-06-21 16:10:41.512362 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_check_eligibility/post.py
--rw-r--r--   0        0        0    21907 2023-06-21 16:10:41.512528 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_check_eligibility/post.pyi
--rw-r--r--   0        0        0      345 2023-06-21 16:10:41.512681 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_initiate/__init__.py
--rw-r--r--   0        0        0    27824 2023-06-21 16:10:41.512833 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_initiate/post.py
--rw-r--r--   0        0        0    27375 2023-06-21 16:10:41.513034 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_initiate/post.pyi
--rw-r--r--   0        0        0      375 2023-06-21 16:10:41.513208 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number/__init__.py
--rw-r--r--   0        0        0    19746 2023-06-21 16:10:41.513363 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.py
--rw-r--r--   0        0        0    19520 2023-06-21 16:10:41.513535 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.pyi
--rw-r--r--   0        0        0      389 2023-06-21 16:10:41.513706 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/__init__.py
--rw-r--r--   0        0        0    19823 2023-06-21 16:10:41.513861 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.py
--rw-r--r--   0        0        0    19597 2023-06-21 16:10:41.514017 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.pyi
--rw-r--r--   0        0        0      389 2023-06-21 16:10:41.514143 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/__init__.py
--rw-r--r--   0        0        0    23713 2023-06-21 16:10:41.514271 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.py
--rw-r--r--   0        0        0    23487 2023-06-21 16:10:41.514392 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.pyi
--rw-r--r--   0        0        0      399 2023-06-21 16:10:41.514511 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/__init__.py
--rw-r--r--   0        0        0    24805 2023-06-21 16:10:41.514622 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.py
--rw-r--r--   0        0        0    24579 2023-06-21 16:10:41.514758 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.pyi
--rw-r--r--   0        0        0      415 2023-06-21 16:10:41.514877 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/__init__.py
--rw-r--r--   0        0        0    19991 2023-06-21 16:10:41.514998 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.py
--rw-r--r--   0        0        0    19765 2023-06-21 16:10:41.515123 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.pyi
--rw-r--r--   0        0        0      341 2023-06-21 16:10:41.515235 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_search/__init__.py
--rw-r--r--   0        0        0    23160 2023-06-21 16:10:41.515361 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_search/get.py
--rw-r--r--   0        0        0    22934 2023-06-21 16:10:41.515495 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_search/get.pyi
--rw-r--r--   0        0        0      351 2023-06-21 16:10:41.515600 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_updateorder/__init__.py
--rw-r--r--   0        0        0    23256 2023-06-21 16:10:41.515717 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_updateorder/put.py
--rw-r--r--   0        0        0    23030 2023-06-21 16:10:41.515875 splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_updateorder/put.pyi
--rw-r--r--   0        0        0      639 2023-06-21 16:10:41.516021 splitit_web_python_sdk-2.4.0/splitit_client/request_after_hook.py
--rw-r--r--   0        0        0      640 2023-06-21 16:10:41.516134 splitit_web_python_sdk-2.4.0/splitit_client/request_before_hook.py
--rw-r--r--   0        0        0    10957 2023-06-21 16:10:41.516244 splitit_web_python_sdk-2.4.0/splitit_client/rest.py
--rw-r--r--   0        0        0    95571 2023-06-21 16:10:41.516444 splitit_web_python_sdk-2.4.0/splitit_client/schemas.py
--rw-r--r--   0        0        0        0 2023-06-21 16:10:41.516560 splitit_web_python_sdk-2.4.0/splitit_client/type/__init__.py
--rw-r--r--   0        0        0      561 2023-06-21 16:10:41.516671 splitit_web_python_sdk-2.4.0/splitit_client/type/address_data.py
--rw-r--r--   0        0        0      587 2023-06-21 16:10:41.516781 splitit_web_python_sdk-2.4.0/splitit_client/type/address_data_model.py
--rw-r--r--   0        0        0      887 2023-06-21 16:10:41.516871 splitit_web_python_sdk-2.4.0/splitit_client/type/authorization_model.py
--rw-r--r--   0        0        0      398 2023-06-21 16:10:41.516962 splitit_web_python_sdk-2.4.0/splitit_client/type/card_brand.py
--rw-r--r--   0        0        0      705 2023-06-21 16:10:41.517053 splitit_web_python_sdk-2.4.0/splitit_client/type/card_data.py
--rw-r--r--   0        0        0      388 2023-06-21 16:10:41.517136 splitit_web_python_sdk-2.4.0/splitit_client/type/card_type.py
--rw-r--r--   0        0        0      816 2023-06-21 16:10:41.517246 splitit_web_python_sdk-2.4.0/splitit_client/type/check_installments_eligibility_request.py
--rw-r--r--   0        0        0      481 2023-06-21 16:10:41.517356 splitit_web_python_sdk-2.4.0/splitit_client/type/error.py
--rw-r--r--   0        0        0      452 2023-06-21 16:10:41.517465 splitit_web_python_sdk-2.4.0/splitit_client/type/error_extended.py
--rw-r--r--   0        0        0      524 2023-06-21 16:10:41.517580 splitit_web_python_sdk-2.4.0/splitit_client/type/events_endpoints_model.py
--rw-r--r--   0        0        0      573 2023-06-21 16:10:41.517724 splitit_web_python_sdk-2.4.0/splitit_client/type/failed_response.py
--rw-r--r--   0        0        0      359 2023-06-21 16:10:41.517915 splitit_web_python_sdk-2.4.0/splitit_client/type/gw_authorization_status.py
--rw-r--r--   0        0        0      588 2023-06-21 16:10:41.518053 splitit_web_python_sdk-2.4.0/splitit_client/type/identifier_contract.py
--rw-r--r--   0        0        0     1018 2023-06-21 16:10:41.518189 splitit_web_python_sdk-2.4.0/splitit_client/type/initiate_plan_response.py
--rw-r--r--   0        0        0      617 2023-06-21 16:10:41.518317 splitit_web_python_sdk-2.4.0/splitit_client/type/initiate_redirection_endpoints_model.py
--rw-r--r--   0        0        0      640 2023-06-21 16:10:41.518437 splitit_web_python_sdk-2.4.0/splitit_client/type/installment.py
--rw-r--r--   0        0        0      575 2023-06-21 16:10:41.518549 splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_cancel_response.py
--rw-r--r--   0        0        0     1257 2023-06-21 16:10:41.518662 splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_create_request.py
--rw-r--r--   0        0        0     1510 2023-06-21 16:10:41.518804 splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_create_response.py
--rw-r--r--   0        0        0     1591 2023-06-21 16:10:41.518913 splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_get_response.py
--rw-r--r--   0        0        0     1242 2023-06-21 16:10:41.519027 splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_initiate_request.py
--rw-r--r--   0        0        0      665 2023-06-21 16:10:41.519139 splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_refund_request.py
--rw-r--r--   0        0        0      805 2023-06-21 16:10:41.519255 splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_refund_response.py
--rw-r--r--   0        0        0      709 2023-06-21 16:10:41.519362 splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_search_response.py
--rw-r--r--   0        0        0      709 2023-06-21 16:10:41.519467 splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_update_request.py
--rw-r--r--   0        0        0      622 2023-06-21 16:10:41.519576 splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_update_request_by_identifier.py
--rw-r--r--   0        0        0      768 2023-06-21 16:10:41.519681 splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_update_response.py
--rw-r--r--   0        0        0      348 2023-06-21 16:10:41.519805 splitit_web_python_sdk-2.4.0/splitit_client/type/installment_status.py
--rw-r--r--   0        0        0      725 2023-06-21 16:10:41.519939 splitit_web_python_sdk-2.4.0/splitit_client/type/installments_eligibility_response.py
--rw-r--r--   0        0        0      532 2023-06-21 16:10:41.520052 splitit_web_python_sdk-2.4.0/splitit_client/type/links_data.py
--rw-r--r--   0        0        0      530 2023-06-21 16:10:41.520167 splitit_web_python_sdk-2.4.0/splitit_client/type/links_model.py
--rw-r--r--   0        0        0      664 2023-06-21 16:10:41.520305 splitit_web_python_sdk-2.4.0/splitit_client/type/payment_method_model.py
--rw-r--r--   0        0        0      336 2023-06-21 16:10:41.520446 splitit_web_python_sdk-2.4.0/splitit_client/type/payment_method_type.py
--rw-r--r--   0        0        0      828 2023-06-21 16:10:41.520587 splitit_web_python_sdk-2.4.0/splitit_client/type/payment_plan_option_model.py
--rw-r--r--   0        0        0      838 2023-06-21 16:10:41.520724 splitit_web_python_sdk-2.4.0/splitit_client/type/plan_data.py
--rw-r--r--   0        0        0      824 2023-06-21 16:10:41.520871 splitit_web_python_sdk-2.4.0/splitit_client/type/plan_data_model.py
--rw-r--r--   0        0        0      484 2023-06-21 16:10:41.520994 splitit_web_python_sdk-2.4.0/splitit_client/type/plan_error_response.py
--rw-r--r--   0        0        0      371 2023-06-21 16:10:41.521129 splitit_web_python_sdk-2.4.0/splitit_client/type/plan_status.py
--rw-r--r--   0        0        0      347 2023-06-21 16:10:41.521265 splitit_web_python_sdk-2.4.0/splitit_client/type/purchase_method.py
--rw-r--r--   0        0        0      615 2023-06-21 16:10:41.521405 splitit_web_python_sdk-2.4.0/splitit_client/type/redirection_endpoints_model.py
--rw-r--r--   0        0        0      719 2023-06-21 16:10:41.521527 splitit_web_python_sdk-2.4.0/splitit_client/type/refund_model.py
--rw-r--r--   0        0        0      341 2023-06-21 16:10:41.521633 splitit_web_python_sdk-2.4.0/splitit_client/type/refund_status.py
--rw-r--r--   0        0        0      423 2023-06-21 16:10:41.521746 splitit_web_python_sdk-2.4.0/splitit_client/type/refund_strategy.py
--rw-r--r--   0        0        0      642 2023-06-21 16:10:41.521844 splitit_web_python_sdk-2.4.0/splitit_client/type/refund_summary.py
--rw-r--r--   0        0        0     1626 2023-06-21 16:10:41.521959 splitit_web_python_sdk-2.4.0/splitit_client/type/search_installment_plan_response_item.py
--rw-r--r--   0        0        0      344 2023-06-21 16:10:41.522091 splitit_web_python_sdk-2.4.0/splitit_client/type/shipping_status.py
--rw-r--r--   0        0        0      334 2023-06-21 16:10:41.522237 splitit_web_python_sdk-2.4.0/splitit_client/type/shipping_status2.py
--rw-r--r--   0        0        0      528 2023-06-21 16:10:41.522373 splitit_web_python_sdk-2.4.0/splitit_client/type/shopper_data.py
--rw-r--r--   0        0        0      345 2023-06-21 16:10:41.522512 splitit_web_python_sdk-2.4.0/splitit_client/type/test_modes.py
--rw-r--r--   0        0        0      567 2023-06-21 16:10:41.522657 splitit_web_python_sdk-2.4.0/splitit_client/type/three_ds_redirect_data_v3.py
--rw-r--r--   0        0        0      656 2023-06-21 16:10:41.522799 splitit_web_python_sdk-2.4.0/splitit_client/type/update_order_request.py
--rw-r--r--   0        0        0      524 2023-06-21 16:10:41.522947 splitit_web_python_sdk-2.4.0/splitit_client/type/ux_settings_model.py
--rw-r--r--   0        0        0      708 2023-06-21 16:10:41.523104 splitit_web_python_sdk-2.4.0/splitit_client/type/verify_authorization_response.py
--rw-r--r--   0        0        0      491 2023-06-21 16:10:41.523265 splitit_web_python_sdk-2.4.0/splitit_client/type_util.py
--rw-r--r--   0        0        0     3170 2023-06-21 16:10:41.523418 splitit_web_python_sdk-2.4.0/splitit_client/validation_metadata.py
--rw-r--r--   0        0        0     9340 1970-01-01 00:00:00.000000 splitit_web_python_sdk-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-27 16:02:40.341745 splitit_web_python_sdk-2.5.0/LICENSE
+-rw-r--r--   0        0        0     8818 2023-06-27 16:03:14.423019 splitit_web_python_sdk-2.5.0/README.md
+-rw-r--r--   0        0        0      737 2023-06-27 16:03:14.426020 splitit_web_python_sdk-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0      725 2023-06-27 16:03:14.426612 splitit_web_python_sdk-2.5.0/splitit_client/__init__.py
+-rw-r--r--   0        0        0    72963 2023-06-27 16:03:14.427309 splitit_web_python_sdk-2.5.0/splitit_client/api_client.py
+-rw-r--r--   0        0        0      663 2023-06-27 16:02:40.302970 splitit_web_python_sdk-2.5.0/splitit_client/api_response.py
+-rw-r--r--   0        0        0      214 2023-06-27 16:02:40.303080 splitit_web_python_sdk-2.5.0/splitit_client/apis/__init__.py
+-rw-r--r--   0        0        0     3411 2023-06-27 16:02:40.303173 splitit_web_python_sdk-2.5.0/splitit_client/apis/path_to_api.py
+-rw-r--r--   0        0        0      241 2023-06-27 16:02:40.303275 splitit_web_python_sdk-2.5.0/splitit_client/apis/paths/__init__.py
+-rw-r--r--   0        0        0      127 2023-06-27 16:02:40.303449 splitit_web_python_sdk-2.5.0/splitit_client/apis/paths/api_installmentplans.py
+-rw-r--r--   0        0        0      161 2023-06-27 16:02:40.303570 splitit_web_python_sdk-2.5.0/splitit_client/apis/paths/api_installmentplans_check_eligibility.py
+-rw-r--r--   0        0        0      144 2023-06-27 16:02:40.303695 splitit_web_python_sdk-2.5.0/splitit_client/apis/paths/api_installmentplans_initiate.py
+-rw-r--r--   0        0        0      169 2023-06-27 16:02:40.303808 splitit_web_python_sdk-2.5.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number.py
+-rw-r--r--   0        0        0      185 2023-06-27 16:02:40.303933 splitit_web_python_sdk-2.5.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_cancel.py
+-rw-r--r--   0        0        0      185 2023-06-27 16:02:40.304051 splitit_web_python_sdk-2.5.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_refund.py
+-rw-r--r--   0        0        0      192 2023-06-27 16:02:40.304170 splitit_web_python_sdk-2.5.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_updateorder.py
+-rw-r--r--   0        0        0      208 2023-06-27 16:02:40.304279 splitit_web_python_sdk-2.5.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_verifyauthorization.py
+-rw-r--r--   0        0        0      137 2023-06-27 16:02:40.304391 splitit_web_python_sdk-2.5.0/splitit_client/apis/paths/api_installmentplans_search.py
+-rw-r--r--   0        0        0      147 2023-06-27 16:02:40.304504 splitit_web_python_sdk-2.5.0/splitit_client/apis/paths/api_installmentplans_updateorder.py
+-rw-r--r--   0        0        0      371 2023-06-27 16:02:40.304622 splitit_web_python_sdk-2.5.0/splitit_client/apis/tag_to_api.py
+-rw-r--r--   0        0        0      328 2023-06-27 16:02:40.304743 splitit_web_python_sdk-2.5.0/splitit_client/apis/tags/__init__.py
+-rw-r--r--   0        0        0     1333 2023-06-27 16:02:40.304867 splitit_web_python_sdk-2.5.0/splitit_client/apis/tags/installment_plan_api.py
+-rw-r--r--   0        0        0      989 2023-06-27 16:02:40.304974 splitit_web_python_sdk-2.5.0/splitit_client/client.py
+-rw-r--r--   0        0        0      989 2023-06-27 16:02:40.305076 splitit_web_python_sdk-2.5.0/splitit_client/client.pyi
+-rw-r--r--   0        0        0      669 2023-06-27 16:02:40.305188 splitit_web_python_sdk-2.5.0/splitit_client/client_custom.py
+-rw-r--r--   0        0        0    18575 2023-06-27 16:03:14.427838 splitit_web_python_sdk-2.5.0/splitit_client/configuration.py
+-rw-r--r--   0        0        0     7672 2023-06-27 16:02:40.305446 splitit_web_python_sdk-2.5.0/splitit_client/exceptions.py
+-rw-r--r--   0        0        0     2274 2023-06-27 16:02:40.305572 splitit_web_python_sdk-2.5.0/splitit_client/exceptions_base.py
+-rw-r--r--   0        0        0      348 2023-06-27 16:02:40.305752 splitit_web_python_sdk-2.5.0/splitit_client/model/__init__.py
+-rw-r--r--   0        0        0     4871 2023-06-27 16:02:40.305880 splitit_web_python_sdk-2.5.0/splitit_client/model/address_data.py
+-rw-r--r--   0        0        0     4871 2023-06-27 16:02:40.305996 splitit_web_python_sdk-2.5.0/splitit_client/model/address_data.pyi
+-rw-r--r--   0        0        0     4894 2023-06-27 16:02:40.306118 splitit_web_python_sdk-2.5.0/splitit_client/model/address_data_model.py
+-rw-r--r--   0        0        0     4894 2023-06-27 16:02:40.306231 splitit_web_python_sdk-2.5.0/splitit_client/model/address_data_model.pyi
+-rw-r--r--   0        0        0     8118 2023-06-27 16:03:14.428142 splitit_web_python_sdk-2.5.0/splitit_client/model/authorization_model.py
+-rw-r--r--   0        0        0     8118 2023-06-27 16:03:14.428306 splitit_web_python_sdk-2.5.0/splitit_client/model/authorization_model.pyi
+-rw-r--r--   0        0        0     2063 2023-06-27 16:03:14.428501 splitit_web_python_sdk-2.5.0/splitit_client/model/bluesnap_vaulted_shopper_token.py
+-rw-r--r--   0        0        0     2063 2023-06-27 16:03:14.428650 splitit_web_python_sdk-2.5.0/splitit_client/model/bluesnap_vaulted_shopper_token.pyi
+-rw-r--r--   0        0        0     1752 2023-06-27 16:02:40.306724 splitit_web_python_sdk-2.5.0/splitit_client/model/card_brand.py
+-rw-r--r--   0        0        0     1392 2023-06-27 16:02:40.306807 splitit_web_python_sdk-2.5.0/splitit_client/model/card_brand.pyi
+-rw-r--r--   0        0        0     5874 2023-06-27 16:02:40.306895 splitit_web_python_sdk-2.5.0/splitit_client/model/card_data.py
+-rw-r--r--   0        0        0     5874 2023-06-27 16:02:40.306983 splitit_web_python_sdk-2.5.0/splitit_client/model/card_data.pyi
+-rw-r--r--   0        0        0     1571 2023-06-27 16:02:40.307066 splitit_web_python_sdk-2.5.0/splitit_client/model/card_type.py
+-rw-r--r--   0        0        0     1251 2023-06-27 16:02:40.307146 splitit_web_python_sdk-2.5.0/splitit_client/model/card_type.pyi
+-rw-r--r--   0        0        0     3738 2023-06-27 16:02:40.307232 splitit_web_python_sdk-2.5.0/splitit_client/model/check_installments_eligibility_request.py
+-rw-r--r--   0        0        0     3738 2023-06-27 16:02:40.307320 splitit_web_python_sdk-2.5.0/splitit_client/model/check_installments_eligibility_request.pyi
+-rw-r--r--   0        0        0     3357 2023-06-27 16:02:40.307401 splitit_web_python_sdk-2.5.0/splitit_client/model/error.py
+-rw-r--r--   0        0        0     3357 2023-06-27 16:02:40.307511 splitit_web_python_sdk-2.5.0/splitit_client/model/error.pyi
+-rw-r--r--   0        0        0     5464 2023-06-27 16:02:40.307606 splitit_web_python_sdk-2.5.0/splitit_client/model/error_extended.py
+-rw-r--r--   0        0        0     5464 2023-06-27 16:02:40.307705 splitit_web_python_sdk-2.5.0/splitit_client/model/error_extended.pyi
+-rw-r--r--   0        0        0     2403 2023-06-27 16:02:40.307812 splitit_web_python_sdk-2.5.0/splitit_client/model/events_endpoints_model.py
+-rw-r--r--   0        0        0     2403 2023-06-27 16:02:40.308480 splitit_web_python_sdk-2.5.0/splitit_client/model/events_endpoints_model.pyi
+-rw-r--r--   0        0        0     2898 2023-06-27 16:02:40.308622 splitit_web_python_sdk-2.5.0/splitit_client/model/failed_response.py
+-rw-r--r--   0        0        0     2898 2023-06-27 16:02:40.308748 splitit_web_python_sdk-2.5.0/splitit_client/model/failed_response.pyi
+-rw-r--r--   0        0        0     2822 2023-06-27 16:03:14.428837 splitit_web_python_sdk-2.5.0/splitit_client/model/gateway_token_data.py
+-rw-r--r--   0        0        0     2822 2023-06-27 16:03:14.428993 splitit_web_python_sdk-2.5.0/splitit_client/model/gateway_token_data.pyi
+-rw-r--r--   0        0        0     1188 2023-06-27 16:02:40.309092 splitit_web_python_sdk-2.5.0/splitit_client/model/gw_authorization_status.py
+-rw-r--r--   0        0        0      991 2023-06-27 16:02:40.309215 splitit_web_python_sdk-2.5.0/splitit_client/model/gw_authorization_status.pyi
+-rw-r--r--   0        0        0     4856 2023-06-27 16:02:40.309330 splitit_web_python_sdk-2.5.0/splitit_client/model/identifier_contract.py
+-rw-r--r--   0        0        0     4856 2023-06-27 16:02:40.309448 splitit_web_python_sdk-2.5.0/splitit_client/model/identifier_contract.pyi
+-rw-r--r--   0        0        0     9111 2023-06-27 16:02:40.309573 splitit_web_python_sdk-2.5.0/splitit_client/model/initiate_plan_response.py
+-rw-r--r--   0        0        0     9111 2023-06-27 16:02:40.310038 splitit_web_python_sdk-2.5.0/splitit_client/model/initiate_plan_response.pyi
+-rw-r--r--   0        0        0     3361 2023-06-27 16:02:40.310213 splitit_web_python_sdk-2.5.0/splitit_client/model/initiate_redirection_endpoints_model.py
+-rw-r--r--   0        0        0     3361 2023-06-27 16:02:40.310391 splitit_web_python_sdk-2.5.0/splitit_client/model/initiate_redirection_endpoints_model.pyi
+-rw-r--r--   0        0        0     4303 2023-06-27 16:02:40.310540 splitit_web_python_sdk-2.5.0/splitit_client/model/installment.py
+-rw-r--r--   0        0        0     4303 2023-06-27 16:02:40.310654 splitit_web_python_sdk-2.5.0/splitit_client/model/installment.pyi
+-rw-r--r--   0        0        0     2499 2023-06-27 16:02:40.310813 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_cancel_response.py
+-rw-r--r--   0        0        0     2499 2023-06-27 16:02:40.310949 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_cancel_response.pyi
+-rw-r--r--   0        0        0     8815 2023-06-27 16:03:14.429285 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_create_request.py
+-rw-r--r--   0        0        0     8815 2023-06-27 16:03:14.429470 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_create_request.pyi
+-rw-r--r--   0        0        0    13350 2023-06-27 16:02:40.311465 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_create_response.py
+-rw-r--r--   0        0        0    13350 2023-06-27 16:02:40.311661 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_create_response.pyi
+-rw-r--r--   0        0        0    14794 2023-06-27 16:02:40.311822 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_get_response.py
+-rw-r--r--   0        0        0    14794 2023-06-27 16:02:40.311944 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_get_response.pyi
+-rw-r--r--   0        0        0     7995 2023-06-27 16:03:14.429702 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_initiate_request.py
+-rw-r--r--   0        0        0     7995 2023-06-27 16:03:14.429870 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_initiate_request.pyi
+-rw-r--r--   0        0        0     3076 2023-06-27 16:02:40.312271 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_refund_request.py
+-rw-r--r--   0        0        0     3076 2023-06-27 16:02:40.312370 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_refund_request.pyi
+-rw-r--r--   0        0        0     5607 2023-06-27 16:02:40.312466 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_refund_response.py
+-rw-r--r--   0        0        0     5607 2023-06-27 16:02:40.312565 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_refund_response.pyi
+-rw-r--r--   0        0        0     3421 2023-06-27 16:02:40.312650 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_search_response.py
+-rw-r--r--   0        0        0     3421 2023-06-27 16:02:40.312736 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_search_response.pyi
+-rw-r--r--   0        0        0     4250 2023-06-27 16:02:40.312849 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_update_request.py
+-rw-r--r--   0        0        0     4250 2023-06-27 16:02:40.312957 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_update_request.pyi
+-rw-r--r--   0        0        0     4385 2023-06-27 16:02:40.313064 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_update_request_by_identifier.py
+-rw-r--r--   0        0        0     4385 2023-06-27 16:02:40.313168 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_update_request_by_identifier.pyi
+-rw-r--r--   0        0        0     4417 2023-06-27 16:02:40.313292 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_update_response.py
+-rw-r--r--   0        0        0     4417 2023-06-27 16:02:40.313413 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_update_response.pyi
+-rw-r--r--   0        0        0     1082 2023-06-27 16:02:40.313522 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_status.py
+-rw-r--r--   0        0        0      911 2023-06-27 16:02:40.313629 splitit_web_python_sdk-2.5.0/splitit_client/model/installment_status.pyi
+-rw-r--r--   0        0        0     4161 2023-06-27 16:02:40.313740 splitit_web_python_sdk-2.5.0/splitit_client/model/installments_eligibility_response.py
+-rw-r--r--   0        0        0     4161 2023-06-27 16:02:40.313857 splitit_web_python_sdk-2.5.0/splitit_client/model/installments_eligibility_response.pyi
+-rw-r--r--   0        0        0     4052 2023-06-27 16:02:40.313984 splitit_web_python_sdk-2.5.0/splitit_client/model/links_data.py
+-rw-r--r--   0        0        0     4052 2023-06-27 16:02:40.314112 splitit_web_python_sdk-2.5.0/splitit_client/model/links_data.pyi
+-rw-r--r--   0        0        0     3679 2023-06-27 16:02:40.314256 splitit_web_python_sdk-2.5.0/splitit_client/model/links_model.py
+-rw-r--r--   0        0        0     3679 2023-06-27 16:02:40.314386 splitit_web_python_sdk-2.5.0/splitit_client/model/links_model.pyi
+-rw-r--r--   0        0        0     2045 2023-06-27 16:03:14.430042 splitit_web_python_sdk-2.5.0/splitit_client/model/mocker_shopper_token.py
+-rw-r--r--   0        0        0     2045 2023-06-27 16:03:14.430173 splitit_web_python_sdk-2.5.0/splitit_client/model/mocker_shopper_token.pyi
+-rw-r--r--   0        0        0     5182 2023-06-27 16:03:14.430391 splitit_web_python_sdk-2.5.0/splitit_client/model/payment_method_model.py
+-rw-r--r--   0        0        0     5182 2023-06-27 16:03:14.430565 splitit_web_python_sdk-2.5.0/splitit_client/model/payment_method_model.pyi
+-rw-r--r--   0        0        0     1340 2023-06-27 16:03:14.430778 splitit_web_python_sdk-2.5.0/splitit_client/model/payment_method_type.py
+-rw-r--r--   0        0        0     1065 2023-06-27 16:03:14.431001 splitit_web_python_sdk-2.5.0/splitit_client/model/payment_method_type.pyi
+-rw-r--r--   0        0        0     6852 2023-06-27 16:02:40.315199 splitit_web_python_sdk-2.5.0/splitit_client/model/payment_plan_option_model.py
+-rw-r--r--   0        0        0     6852 2023-06-27 16:02:40.315299 splitit_web_python_sdk-2.5.0/splitit_client/model/payment_plan_option_model.pyi
+-rw-r--r--   0        0        0    10953 2023-06-27 16:03:14.431228 splitit_web_python_sdk-2.5.0/splitit_client/model/plan_data.py
+-rw-r--r--   0        0        0    10953 2023-06-27 16:03:14.431428 splitit_web_python_sdk-2.5.0/splitit_client/model/plan_data.pyi
+-rw-r--r--   0        0        0     8734 2023-06-27 16:02:40.315709 splitit_web_python_sdk-2.5.0/splitit_client/model/plan_data_model.py
+-rw-r--r--   0        0        0     8734 2023-06-27 16:02:40.315837 splitit_web_python_sdk-2.5.0/splitit_client/model/plan_data_model.pyi
+-rw-r--r--   0        0        0     4276 2023-06-27 16:02:40.315975 splitit_web_python_sdk-2.5.0/splitit_client/model/plan_error_response.py
+-rw-r--r--   0        0        0     4276 2023-06-27 16:02:40.316078 splitit_web_python_sdk-2.5.0/splitit_client/model/plan_error_response.pyi
+-rw-r--r--   0        0        0     1345 2023-06-27 16:02:40.316180 splitit_web_python_sdk-2.5.0/splitit_client/model/plan_status.py
+-rw-r--r--   0        0        0     1089 2023-06-27 16:02:40.316283 splitit_web_python_sdk-2.5.0/splitit_client/model/plan_status.pyi
+-rw-r--r--   0        0        0     3725 2023-06-27 16:03:14.431634 splitit_web_python_sdk-2.5.0/splitit_client/model/processing_data.py
+-rw-r--r--   0        0        0     3725 2023-06-27 16:03:14.431765 splitit_web_python_sdk-2.5.0/splitit_client/model/processing_data.pyi
+-rw-r--r--   0        0        0     3734 2023-06-27 16:03:14.431998 splitit_web_python_sdk-2.5.0/splitit_client/model/processing_data2.py
+-rw-r--r--   0        0        0     3734 2023-06-27 16:03:14.432160 splitit_web_python_sdk-2.5.0/splitit_client/model/processing_data2.pyi
+-rw-r--r--   0        0        0     1091 2023-06-27 16:02:40.316770 splitit_web_python_sdk-2.5.0/splitit_client/model/purchase_method.py
+-rw-r--r--   0        0        0      914 2023-06-27 16:02:40.316864 splitit_web_python_sdk-2.5.0/splitit_client/model/purchase_method.pyi
+-rw-r--r--   0        0        0     4123 2023-06-27 16:02:40.316965 splitit_web_python_sdk-2.5.0/splitit_client/model/redirection_endpoints_model.py
+-rw-r--r--   0        0        0     4123 2023-06-27 16:02:40.317057 splitit_web_python_sdk-2.5.0/splitit_client/model/redirection_endpoints_model.pyi
+-rw-r--r--   0        0        0     5623 2023-06-27 16:02:40.317140 splitit_web_python_sdk-2.5.0/splitit_client/model/refund_model.py
+-rw-r--r--   0        0        0     5623 2023-06-27 16:02:40.317225 splitit_web_python_sdk-2.5.0/splitit_client/model/refund_model.pyi
+-rw-r--r--   0        0        0     1069 2023-06-27 16:02:40.317312 splitit_web_python_sdk-2.5.0/splitit_client/model/refund_status.py
+-rw-r--r--   0        0        0      902 2023-06-27 16:02:40.317402 splitit_web_python_sdk-2.5.0/splitit_client/model/refund_status.pyi
+-rw-r--r--   0        0        0     1485 2023-06-27 16:02:40.317486 splitit_web_python_sdk-2.5.0/splitit_client/model/refund_strategy.py
+-rw-r--r--   0        0        0     1136 2023-06-27 16:02:40.317597 splitit_web_python_sdk-2.5.0/splitit_client/model/refund_strategy.pyi
+-rw-r--r--   0        0        0     4246 2023-06-27 16:02:40.317703 splitit_web_python_sdk-2.5.0/splitit_client/model/refund_summary.py
+-rw-r--r--   0        0        0     4246 2023-06-27 16:02:40.317816 splitit_web_python_sdk-2.5.0/splitit_client/model/refund_summary.pyi
+-rw-r--r--   0        0        0    14808 2023-06-27 16:02:40.317939 splitit_web_python_sdk-2.5.0/splitit_client/model/search_installment_plan_response_item.py
+-rw-r--r--   0        0        0    14808 2023-06-27 16:02:40.318110 splitit_web_python_sdk-2.5.0/splitit_client/model/search_installment_plan_response_item.pyi
+-rw-r--r--   0        0        0     1075 2023-06-27 16:02:40.318281 splitit_web_python_sdk-2.5.0/splitit_client/model/shipping_status.py
+-rw-r--r--   0        0        0      906 2023-06-27 16:02:40.318399 splitit_web_python_sdk-2.5.0/splitit_client/model/shipping_status.pyi
+-rw-r--r--   0        0        0      958 2023-06-27 16:02:40.318518 splitit_web_python_sdk-2.5.0/splitit_client/model/shipping_status2.py
+-rw-r--r--   0        0        0      823 2023-06-27 16:02:40.318645 splitit_web_python_sdk-2.5.0/splitit_client/model/shipping_status2.pyi
+-rw-r--r--   0        0        0     3874 2023-06-27 16:02:40.318774 splitit_web_python_sdk-2.5.0/splitit_client/model/shopper_data.py
+-rw-r--r--   0        0        0     3874 2023-06-27 16:02:40.318887 splitit_web_python_sdk-2.5.0/splitit_client/model/shopper_data.pyi
+-rw-r--r--   0        0        0     1168 2023-06-27 16:02:40.318999 splitit_web_python_sdk-2.5.0/splitit_client/model/test_modes.py
+-rw-r--r--   0        0        0      975 2023-06-27 16:02:40.319115 splitit_web_python_sdk-2.5.0/splitit_client/model/test_modes.pyi
+-rw-r--r--   0        0        0     5066 2023-06-27 16:03:14.432345 splitit_web_python_sdk-2.5.0/splitit_client/model/three_ds_data.py
+-rw-r--r--   0        0        0     5066 2023-06-27 16:03:14.432493 splitit_web_python_sdk-2.5.0/splitit_client/model/three_ds_data.pyi
+-rw-r--r--   0        0        0     5068 2023-06-27 16:03:14.432733 splitit_web_python_sdk-2.5.0/splitit_client/model/three_ds_data2.py
+-rw-r--r--   0        0        0     5068 2023-06-27 16:03:14.432907 splitit_web_python_sdk-2.5.0/splitit_client/model/three_ds_data2.pyi
+-rw-r--r--   0        0        0     4386 2023-06-27 16:02:40.319697 splitit_web_python_sdk-2.5.0/splitit_client/model/three_ds_redirect_data_v3.py
+-rw-r--r--   0        0        0     4386 2023-06-27 16:02:40.319821 splitit_web_python_sdk-2.5.0/splitit_client/model/three_ds_redirect_data_v3.pyi
+-rw-r--r--   0        0        0     4223 2023-06-27 16:02:40.319923 splitit_web_python_sdk-2.5.0/splitit_client/model/update_order_request.py
+-rw-r--r--   0        0        0     4223 2023-06-27 16:02:40.320031 splitit_web_python_sdk-2.5.0/splitit_client/model/update_order_request.pyi
+-rw-r--r--   0        0        0     3409 2023-06-27 16:02:40.320177 splitit_web_python_sdk-2.5.0/splitit_client/model/ux_settings_model.py
+-rw-r--r--   0        0        0     3409 2023-06-27 16:02:40.320316 splitit_web_python_sdk-2.5.0/splitit_client/model/ux_settings_model.pyi
+-rw-r--r--   0        0        0     3864 2023-06-27 16:02:40.320454 splitit_web_python_sdk-2.5.0/splitit_client/model/verify_authorization_response.py
+-rw-r--r--   0        0        0     3864 2023-06-27 16:02:40.320581 splitit_web_python_sdk-2.5.0/splitit_client/model/verify_authorization_response.pyi
+-rw-r--r--   0        0        0     4850 2023-06-27 16:03:14.433209 splitit_web_python_sdk-2.5.0/splitit_client/models/__init__.py
+-rw-r--r--   0        0        0     1223 2023-06-27 16:02:40.320877 splitit_web_python_sdk-2.5.0/splitit_client/paths/__init__.py
+-rw-r--r--   0        0        0      327 2023-06-27 16:02:40.321013 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans/__init__.py
+-rw-r--r--   0        0        0    29303 2023-06-27 16:03:14.433617 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans/post.py
+-rw-r--r--   0        0        0    28854 2023-06-27 16:03:14.433959 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans/post.pyi
+-rw-r--r--   0        0        0      362 2023-06-27 16:02:40.321550 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_check_eligibility/__init__.py
+-rw-r--r--   0        0        0    22133 2023-06-27 16:02:40.321706 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_check_eligibility/post.py
+-rw-r--r--   0        0        0    21907 2023-06-27 16:02:40.321858 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_check_eligibility/post.pyi
+-rw-r--r--   0        0        0      345 2023-06-27 16:02:40.321978 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_initiate/__init__.py
+-rw-r--r--   0        0        0    28574 2023-06-27 16:03:14.434269 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_initiate/post.py
+-rw-r--r--   0        0        0    28125 2023-06-27 16:03:14.434668 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_initiate/post.pyi
+-rw-r--r--   0        0        0      375 2023-06-27 16:02:40.322463 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number/__init__.py
+-rw-r--r--   0        0        0    19746 2023-06-27 16:02:40.322586 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.py
+-rw-r--r--   0        0        0    19520 2023-06-27 16:02:40.322731 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.pyi
+-rw-r--r--   0        0        0      389 2023-06-27 16:02:40.322887 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/__init__.py
+-rw-r--r--   0        0        0    19823 2023-06-27 16:02:40.323032 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.py
+-rw-r--r--   0        0        0    19597 2023-06-27 16:02:40.323195 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.pyi
+-rw-r--r--   0        0        0      389 2023-06-27 16:02:40.323324 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/__init__.py
+-rw-r--r--   0        0        0    23713 2023-06-27 16:02:40.323443 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.py
+-rw-r--r--   0        0        0    23487 2023-06-27 16:02:40.323576 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.pyi
+-rw-r--r--   0        0        0      399 2023-06-27 16:02:40.323710 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/__init__.py
+-rw-r--r--   0        0        0    24805 2023-06-27 16:02:40.323833 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.py
+-rw-r--r--   0        0        0    24579 2023-06-27 16:02:40.323968 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.pyi
+-rw-r--r--   0        0        0      415 2023-06-27 16:02:40.324099 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/__init__.py
+-rw-r--r--   0        0        0    19991 2023-06-27 16:02:40.324213 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.py
+-rw-r--r--   0        0        0    19765 2023-06-27 16:02:40.324332 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.pyi
+-rw-r--r--   0        0        0      341 2023-06-27 16:02:40.324437 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_search/__init__.py
+-rw-r--r--   0        0        0    23160 2023-06-27 16:02:40.324540 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_search/get.py
+-rw-r--r--   0        0        0    22934 2023-06-27 16:02:40.324655 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_search/get.pyi
+-rw-r--r--   0        0        0      351 2023-06-27 16:02:40.324768 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_updateorder/__init__.py
+-rw-r--r--   0        0        0    23256 2023-06-27 16:02:40.324879 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_updateorder/put.py
+-rw-r--r--   0        0        0    23030 2023-06-27 16:02:40.325017 splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_updateorder/put.pyi
+-rw-r--r--   0        0        0      639 2023-06-27 16:02:40.325129 splitit_web_python_sdk-2.5.0/splitit_client/request_after_hook.py
+-rw-r--r--   0        0        0      640 2023-06-27 16:02:40.325225 splitit_web_python_sdk-2.5.0/splitit_client/request_before_hook.py
+-rw-r--r--   0        0        0    10957 2023-06-27 16:02:40.325322 splitit_web_python_sdk-2.5.0/splitit_client/rest.py
+-rw-r--r--   0        0        0    95571 2023-06-27 16:02:40.325519 splitit_web_python_sdk-2.5.0/splitit_client/schemas.py
+-rw-r--r--   0        0        0        0 2023-06-27 16:02:40.325634 splitit_web_python_sdk-2.5.0/splitit_client/type/__init__.py
+-rw-r--r--   0        0        0      561 2023-06-27 16:02:40.325722 splitit_web_python_sdk-2.5.0/splitit_client/type/address_data.py
+-rw-r--r--   0        0        0      587 2023-06-27 16:02:40.325813 splitit_web_python_sdk-2.5.0/splitit_client/type/address_data_model.py
+-rw-r--r--   0        0        0      919 2023-06-27 16:03:14.435003 splitit_web_python_sdk-2.5.0/splitit_client/type/authorization_model.py
+-rw-r--r--   0        0        0      501 2023-06-27 16:03:14.435302 splitit_web_python_sdk-2.5.0/splitit_client/type/bluesnap_vaulted_shopper_token.py
+-rw-r--r--   0        0        0      398 2023-06-27 16:02:40.326094 splitit_web_python_sdk-2.5.0/splitit_client/type/card_brand.py
+-rw-r--r--   0        0        0      705 2023-06-27 16:02:40.326178 splitit_web_python_sdk-2.5.0/splitit_client/type/card_data.py
+-rw-r--r--   0        0        0      388 2023-06-27 16:02:40.326262 splitit_web_python_sdk-2.5.0/splitit_client/type/card_type.py
+-rw-r--r--   0        0        0      816 2023-06-27 16:02:40.326345 splitit_web_python_sdk-2.5.0/splitit_client/type/check_installments_eligibility_request.py
+-rw-r--r--   0        0        0      481 2023-06-27 16:02:40.326425 splitit_web_python_sdk-2.5.0/splitit_client/type/error.py
+-rw-r--r--   0        0        0      452 2023-06-27 16:02:40.326514 splitit_web_python_sdk-2.5.0/splitit_client/type/error_extended.py
+-rw-r--r--   0        0        0      524 2023-06-27 16:02:40.326599 splitit_web_python_sdk-2.5.0/splitit_client/type/events_endpoints_model.py
+-rw-r--r--   0        0        0      573 2023-06-27 16:02:40.326680 splitit_web_python_sdk-2.5.0/splitit_client/type/failed_response.py
+-rw-r--r--   0        0        0      515 2023-06-27 16:03:14.435666 splitit_web_python_sdk-2.5.0/splitit_client/type/gateway_token_data.py
+-rw-r--r--   0        0        0      359 2023-06-27 16:02:40.326866 splitit_web_python_sdk-2.5.0/splitit_client/type/gw_authorization_status.py
+-rw-r--r--   0        0        0      588 2023-06-27 16:02:40.326952 splitit_web_python_sdk-2.5.0/splitit_client/type/identifier_contract.py
+-rw-r--r--   0        0        0     1018 2023-06-27 16:02:40.327040 splitit_web_python_sdk-2.5.0/splitit_client/type/initiate_plan_response.py
+-rw-r--r--   0        0        0      617 2023-06-27 16:02:40.327128 splitit_web_python_sdk-2.5.0/splitit_client/type/initiate_redirection_endpoints_model.py
+-rw-r--r--   0        0        0      640 2023-06-27 16:02:40.327227 splitit_web_python_sdk-2.5.0/splitit_client/type/installment.py
+-rw-r--r--   0        0        0      575 2023-06-27 16:02:40.327453 splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_cancel_response.py
+-rw-r--r--   0        0        0     1356 2023-06-27 16:03:14.435976 splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_create_request.py
+-rw-r--r--   0        0        0     1510 2023-06-27 16:02:40.327723 splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_create_response.py
+-rw-r--r--   0        0        0     1591 2023-06-27 16:02:40.327819 splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_get_response.py
+-rw-r--r--   0        0        0     1341 2023-06-27 16:03:14.436240 splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_initiate_request.py
+-rw-r--r--   0        0        0      665 2023-06-27 16:02:40.328009 splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_refund_request.py
+-rw-r--r--   0        0        0      805 2023-06-27 16:02:40.328111 splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_refund_response.py
+-rw-r--r--   0        0        0      709 2023-06-27 16:02:40.328217 splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_search_response.py
+-rw-r--r--   0        0        0      709 2023-06-27 16:02:40.328325 splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_update_request.py
+-rw-r--r--   0        0        0      622 2023-06-27 16:02:40.328428 splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_update_request_by_identifier.py
+-rw-r--r--   0        0        0      768 2023-06-27 16:02:40.328530 splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_update_response.py
+-rw-r--r--   0        0        0      348 2023-06-27 16:02:40.328636 splitit_web_python_sdk-2.5.0/splitit_client/type/installment_status.py
+-rw-r--r--   0        0        0      725 2023-06-27 16:02:40.328738 splitit_web_python_sdk-2.5.0/splitit_client/type/installments_eligibility_response.py
+-rw-r--r--   0        0        0      532 2023-06-27 16:02:40.328838 splitit_web_python_sdk-2.5.0/splitit_client/type/links_data.py
+-rw-r--r--   0        0        0      530 2023-06-27 16:02:40.328938 splitit_web_python_sdk-2.5.0/splitit_client/type/links_model.py
+-rw-r--r--   0        0        0      492 2023-06-27 16:03:14.436452 splitit_web_python_sdk-2.5.0/splitit_client/type/mocker_shopper_token.py
+-rw-r--r--   0        0        0      933 2023-06-27 16:03:14.436724 splitit_web_python_sdk-2.5.0/splitit_client/type/payment_method_model.py
+-rw-r--r--   0        0        0      391 2023-06-27 16:03:14.437027 splitit_web_python_sdk-2.5.0/splitit_client/type/payment_method_type.py
+-rw-r--r--   0        0        0      828 2023-06-27 16:02:40.329352 splitit_web_python_sdk-2.5.0/splitit_client/type/payment_plan_option_model.py
+-rw-r--r--   0        0        0      940 2023-06-27 16:03:14.437268 splitit_web_python_sdk-2.5.0/splitit_client/type/plan_data.py
+-rw-r--r--   0        0        0      824 2023-06-27 16:02:40.329558 splitit_web_python_sdk-2.5.0/splitit_client/type/plan_data_model.py
+-rw-r--r--   0        0        0      484 2023-06-27 16:02:40.329651 splitit_web_python_sdk-2.5.0/splitit_client/type/plan_error_response.py
+-rw-r--r--   0        0        0      371 2023-06-27 16:02:40.329740 splitit_web_python_sdk-2.5.0/splitit_client/type/plan_status.py
+-rw-r--r--   0        0        0      613 2023-06-27 16:03:14.437455 splitit_web_python_sdk-2.5.0/splitit_client/type/processing_data.py
+-rw-r--r--   0        0        0      621 2023-06-27 16:03:14.437653 splitit_web_python_sdk-2.5.0/splitit_client/type/processing_data2.py
+-rw-r--r--   0        0        0      347 2023-06-27 16:02:40.330078 splitit_web_python_sdk-2.5.0/splitit_client/type/purchase_method.py
+-rw-r--r--   0        0        0      615 2023-06-27 16:02:40.330202 splitit_web_python_sdk-2.5.0/splitit_client/type/redirection_endpoints_model.py
+-rw-r--r--   0        0        0      719 2023-06-27 16:02:40.330324 splitit_web_python_sdk-2.5.0/splitit_client/type/refund_model.py
+-rw-r--r--   0        0        0      341 2023-06-27 16:02:40.330449 splitit_web_python_sdk-2.5.0/splitit_client/type/refund_status.py
+-rw-r--r--   0        0        0      423 2023-06-27 16:02:40.330581 splitit_web_python_sdk-2.5.0/splitit_client/type/refund_strategy.py
+-rw-r--r--   0        0        0      642 2023-06-27 16:02:40.330699 splitit_web_python_sdk-2.5.0/splitit_client/type/refund_summary.py
+-rw-r--r--   0        0        0     1626 2023-06-27 16:02:40.330821 splitit_web_python_sdk-2.5.0/splitit_client/type/search_installment_plan_response_item.py
+-rw-r--r--   0        0        0      344 2023-06-27 16:02:40.330951 splitit_web_python_sdk-2.5.0/splitit_client/type/shipping_status.py
+-rw-r--r--   0        0        0      334 2023-06-27 16:02:40.331072 splitit_web_python_sdk-2.5.0/splitit_client/type/shipping_status2.py
+-rw-r--r--   0        0        0      528 2023-06-27 16:02:40.331203 splitit_web_python_sdk-2.5.0/splitit_client/type/shopper_data.py
+-rw-r--r--   0        0        0      345 2023-06-27 16:02:40.331330 splitit_web_python_sdk-2.5.0/splitit_client/type/test_modes.py
+-rw-r--r--   0        0        0      576 2023-06-27 16:03:14.437813 splitit_web_python_sdk-2.5.0/splitit_client/type/three_ds_data.py
+-rw-r--r--   0        0        0      581 2023-06-27 16:03:14.437952 splitit_web_python_sdk-2.5.0/splitit_client/type/three_ds_data2.py
+-rw-r--r--   0        0        0      567 2023-06-27 16:02:40.331731 splitit_web_python_sdk-2.5.0/splitit_client/type/three_ds_redirect_data_v3.py
+-rw-r--r--   0        0        0      656 2023-06-27 16:02:40.331847 splitit_web_python_sdk-2.5.0/splitit_client/type/update_order_request.py
+-rw-r--r--   0        0        0      524 2023-06-27 16:02:40.331959 splitit_web_python_sdk-2.5.0/splitit_client/type/ux_settings_model.py
+-rw-r--r--   0        0        0      708 2023-06-27 16:02:40.332072 splitit_web_python_sdk-2.5.0/splitit_client/type/verify_authorization_response.py
+-rw-r--r--   0        0        0      491 2023-06-27 16:02:40.332212 splitit_web_python_sdk-2.5.0/splitit_client/type_util.py
+-rw-r--r--   0        0        0     3170 2023-06-27 16:02:40.332346 splitit_web_python_sdk-2.5.0/splitit_client/validation_metadata.py
+-rw-r--r--   0        0        0     9727 1970-01-01 00:00:00.000000 splitit_web_python_sdk-2.5.0/PKG-INFO
```

### Comparing `splitit_web_python_sdk-2.4.0/LICENSE` & `splitit_web_python_sdk-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/README.md` & `splitit_web_python_sdk-2.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# splitit-web-python-sdk@2.4.0
+# splitit-web-python-sdk@2.5.0
 Splitit's Web API
 
 
 ## Requirements
 
 Python >=3.7
 
 ## Installing
 
 ```sh
-pip install splitit-web-python-sdk==2.4.0
+pip install splitit-web-python-sdk==2.5.0
 ```
 
 ## Getting Started
 
 ```python
 from pprint import pprint
 from splitit_client import Splitit, ApiException
@@ -131,22 +131,24 @@
 *InstallmentPlanApi* | [**verify_authorization**](docs/apis/tags/InstallmentPlanApi.md#verify_authorization) | **get** /api/installmentplans/{installmentPlanNumber}/verifyauthorization | 
 
 ## Documentation For Models
 
  - [AddressData](docs/models/AddressData.md)
  - [AddressDataModel](docs/models/AddressDataModel.md)
  - [AuthorizationModel](docs/models/AuthorizationModel.md)
+ - [BluesnapVaultedShopperToken](docs/models/BluesnapVaultedShopperToken.md)
  - [CardBrand](docs/models/CardBrand.md)
  - [CardData](docs/models/CardData.md)
  - [CardType](docs/models/CardType.md)
  - [CheckInstallmentsEligibilityRequest](docs/models/CheckInstallmentsEligibilityRequest.md)
  - [Error](docs/models/Error.md)
  - [ErrorExtended](docs/models/ErrorExtended.md)
  - [EventsEndpointsModel](docs/models/EventsEndpointsModel.md)
  - [FailedResponse](docs/models/FailedResponse.md)
+ - [GatewayTokenData](docs/models/GatewayTokenData.md)
  - [GwAuthorizationStatus](docs/models/GwAuthorizationStatus.md)
  - [IdentifierContract](docs/models/IdentifierContract.md)
  - [InitiatePlanResponse](docs/models/InitiatePlanResponse.md)
  - [InitiateRedirectionEndpointsModel](docs/models/InitiateRedirectionEndpointsModel.md)
  - [Installment](docs/models/Installment.md)
  - [InstallmentPlanCancelResponse](docs/models/InstallmentPlanCancelResponse.md)
  - [InstallmentPlanCreateRequest](docs/models/InstallmentPlanCreateRequest.md)
@@ -159,32 +161,37 @@
  - [InstallmentPlanUpdateRequest](docs/models/InstallmentPlanUpdateRequest.md)
  - [InstallmentPlanUpdateRequestByIdentifier](docs/models/InstallmentPlanUpdateRequestByIdentifier.md)
  - [InstallmentPlanUpdateResponse](docs/models/InstallmentPlanUpdateResponse.md)
  - [InstallmentStatus](docs/models/InstallmentStatus.md)
  - [InstallmentsEligibilityResponse](docs/models/InstallmentsEligibilityResponse.md)
  - [LinksData](docs/models/LinksData.md)
  - [LinksModel](docs/models/LinksModel.md)
+ - [MockerShopperToken](docs/models/MockerShopperToken.md)
  - [PaymentMethodModel](docs/models/PaymentMethodModel.md)
  - [PaymentMethodType](docs/models/PaymentMethodType.md)
  - [PaymentPlanOptionModel](docs/models/PaymentPlanOptionModel.md)
  - [PlanData](docs/models/PlanData.md)
  - [PlanDataModel](docs/models/PlanDataModel.md)
  - [PlanErrorResponse](docs/models/PlanErrorResponse.md)
  - [PlanStatus](docs/models/PlanStatus.md)
+ - [ProcessingData](docs/models/ProcessingData.md)
+ - [ProcessingData2](docs/models/ProcessingData2.md)
  - [PurchaseMethod](docs/models/PurchaseMethod.md)
  - [RedirectionEndpointsModel](docs/models/RedirectionEndpointsModel.md)
  - [RefundModel](docs/models/RefundModel.md)
  - [RefundStatus](docs/models/RefundStatus.md)
  - [RefundStrategy](docs/models/RefundStrategy.md)
  - [RefundSummary](docs/models/RefundSummary.md)
  - [SearchInstallmentPlanResponseItem](docs/models/SearchInstallmentPlanResponseItem.md)
  - [ShippingStatus](docs/models/ShippingStatus.md)
  - [ShippingStatus2](docs/models/ShippingStatus2.md)
  - [ShopperData](docs/models/ShopperData.md)
  - [TestModes](docs/models/TestModes.md)
+ - [ThreeDSData](docs/models/ThreeDSData.md)
+ - [ThreeDSData2](docs/models/ThreeDSData2.md)
  - [ThreeDsRedirectDataV3](docs/models/ThreeDsRedirectDataV3.md)
  - [UpdateOrderRequest](docs/models/UpdateOrderRequest.md)
  - [UxSettingsModel](docs/models/UxSettingsModel.md)
  - [VerifyAuthorizationResponse](docs/models/VerifyAuthorizationResponse.md)
 
 
 ## Author
```

### Comparing `splitit_web_python_sdk-2.4.0/pyproject.toml` & `splitit_web_python_sdk-2.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "splitit-web-python-sdk"
-version = "2.4.0"
+version = "2.5.0"
 description = "Client for splitit-web-api-v3"
 authors = ["Konfig <engineering@konfigthis.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "splitit_client"}]
 
 [tool.poetry.dependencies]
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/__init__.py` & `splitit_web_python_sdk-2.5.0/splitit_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     Splitit's Web API
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
-__version__ = "2.4.0"
+__version__ = "2.5.0"
 
 # import ApiClient
 from splitit_client.api_client import ApiClient
 
 # import Configuration
 from splitit_client.configuration import Configuration
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/api_client.py` & `splitit_web_python_sdk-2.5.0/splitit_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2734,15 +2734,15 @@
 0000aad0: 5f6e 616d 655d 203d 2068 6561 6465 725f  _name] = header_
 0000aae0: 7661 6c75 650a 2020 2020 2020 2020 7365  value.        se
 0000aaf0: 6c66 2e63 6f6f 6b69 6520 3d20 636f 6f6b  lf.cookie = cook
 0000ab00: 6965 0a20 2020 2020 2020 2023 2053 6574  ie.        # Set
 0000ab10: 2064 6566 6175 6c74 2055 7365 722d 4167   default User-Ag
 0000ab20: 656e 742e 0a20 2020 2020 2020 2073 656c  ent..        sel
 0000ab30: 662e 7573 6572 5f61 6765 6e74 203d 2027  f.user_agent = '
-0000ab40: 4b6f 6e66 6967 2f32 2e34 2e30 2f70 7974  Konfig/2.4.0/pyt
+0000ab40: 4b6f 6e66 6967 2f32 2e35 2e30 2f70 7974  Konfig/2.5.0/pyt
 0000ab50: 686f 6e27 0a0a 2020 2020 6465 6620 5f5f  hon'..    def __
 0000ab60: 656e 7465 725f 5f28 7365 6c66 293a 0a20  enter__(self):. 
 0000ab70: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
 0000ab80: 6c66 0a0a 2020 2020 6465 6620 5f5f 6578  lf..    def __ex
 0000ab90: 6974 5f5f 2873 656c 662c 2065 7863 5f74  it__(self, exc_t
 0000aba0: 7970 652c 2065 7863 5f76 616c 7565 2c20  ype, exc_value, 
 0000abb0: 7472 6163 6562 6163 6b29 3a0a 2020 2020  traceback):.
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/api_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/api_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/apis/path_to_api.py` & `splitit_web_python_sdk-2.5.0/splitit_client/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/apis/tags/installment_plan_api.py` & `splitit_web_python_sdk-2.5.0/splitit_client/apis/tags/installment_plan_api.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/client.py` & `splitit_web_python_sdk-2.5.0/splitit_client/client.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/client.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/client.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/client_custom.py` & `splitit_web_python_sdk-2.5.0/splitit_client/client_custom.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/configuration.py` & `splitit_web_python_sdk-2.5.0/splitit_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 2.4.0".\
+               "SDK Package Version: 2.5.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/exceptions.py` & `splitit_web_python_sdk-2.5.0/splitit_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/exceptions_base.py` & `splitit_web_python_sdk-2.5.0/splitit_client/exceptions_base.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/address_data.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/address_data.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/address_data.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/address_data.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/address_data_model.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/address_data_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/address_data_model.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/address_data_model.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/authorization_model.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/authorization_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,24 +48,26 @@
             GatewayResultMessage = schemas.StrSchema
         
             @staticmethod
             def ThreeDSRedirect() -> typing.Type['ThreeDsRedirectDataV3']:
                 return ThreeDsRedirectDataV3
             CAVV = schemas.StrSchema
             ECI = schemas.StrSchema
+            GatewaySourceResponse = schemas.StrSchema
             __annotations__ = {
                 "Status": Status,
                 "Date": Date,
                 "SplititErrorResultCode": SplititErrorResultCode,
                 "GatewayTransactionID": GatewayTransactionID,
                 "GatewayResultCode": GatewayResultCode,
                 "GatewayResultMessage": GatewayResultMessage,
                 "ThreeDSRedirect": ThreeDSRedirect,
                 "CAVV": CAVV,
                 "ECI": ECI,
+                "GatewaySourceResponse": GatewaySourceResponse,
             }
     
     Status: 'GwAuthorizationStatus'
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Status"]) -> 'GwAuthorizationStatus': ...
     
@@ -90,17 +92,20 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["CAVV"]) -> MetaOapg.properties.CAVV: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["ECI"]) -> MetaOapg.properties.ECI: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["GatewaySourceResponse"]) -> MetaOapg.properties.GatewaySourceResponse: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["Status", "Date", "SplititErrorResultCode", "GatewayTransactionID", "GatewayResultCode", "GatewayResultMessage", "ThreeDSRedirect", "CAVV", "ECI", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["Status", "Date", "SplititErrorResultCode", "GatewayTransactionID", "GatewayResultCode", "GatewayResultMessage", "ThreeDSRedirect", "CAVV", "ECI", "GatewaySourceResponse", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Status"]) -> 'GwAuthorizationStatus': ...
     
@@ -125,17 +130,20 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["CAVV"]) -> typing.Union[MetaOapg.properties.CAVV, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["ECI"]) -> typing.Union[MetaOapg.properties.ECI, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["GatewaySourceResponse"]) -> typing.Union[MetaOapg.properties.GatewaySourceResponse, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["Status", "Date", "SplititErrorResultCode", "GatewayTransactionID", "GatewayResultCode", "GatewayResultMessage", "ThreeDSRedirect", "CAVV", "ECI", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["Status", "Date", "SplititErrorResultCode", "GatewayTransactionID", "GatewayResultCode", "GatewayResultMessage", "ThreeDSRedirect", "CAVV", "ECI", "GatewaySourceResponse", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         Status: 'GwAuthorizationStatus',
@@ -143,14 +151,15 @@
         SplititErrorResultCode: typing.Union[MetaOapg.properties.SplititErrorResultCode, str, schemas.Unset] = schemas.unset,
         GatewayTransactionID: typing.Union[MetaOapg.properties.GatewayTransactionID, str, schemas.Unset] = schemas.unset,
         GatewayResultCode: typing.Union[MetaOapg.properties.GatewayResultCode, str, schemas.Unset] = schemas.unset,
         GatewayResultMessage: typing.Union[MetaOapg.properties.GatewayResultMessage, str, schemas.Unset] = schemas.unset,
         ThreeDSRedirect: typing.Union['ThreeDsRedirectDataV3', schemas.Unset] = schemas.unset,
         CAVV: typing.Union[MetaOapg.properties.CAVV, str, schemas.Unset] = schemas.unset,
         ECI: typing.Union[MetaOapg.properties.ECI, str, schemas.Unset] = schemas.unset,
+        GatewaySourceResponse: typing.Union[MetaOapg.properties.GatewaySourceResponse, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'AuthorizationModel':
         return super().__new__(
             cls,
             *args,
             Status=Status,
@@ -158,13 +167,14 @@
             SplititErrorResultCode=SplititErrorResultCode,
             GatewayTransactionID=GatewayTransactionID,
             GatewayResultCode=GatewayResultCode,
             GatewayResultMessage=GatewayResultMessage,
             ThreeDSRedirect=ThreeDSRedirect,
             CAVV=CAVV,
             ECI=ECI,
+            GatewaySourceResponse=GatewaySourceResponse,
             _configuration=_configuration,
             **kwargs,
         )
 
 from splitit_client.model.gw_authorization_status import GwAuthorizationStatus
 from splitit_client.model.three_ds_redirect_data_v3 import ThreeDsRedirectDataV3
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/authorization_model.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/authorization_model.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -48,24 +48,26 @@
             GatewayResultMessage = schemas.StrSchema
         
             @staticmethod
             def ThreeDSRedirect() -> typing.Type['ThreeDsRedirectDataV3']:
                 return ThreeDsRedirectDataV3
             CAVV = schemas.StrSchema
             ECI = schemas.StrSchema
+            GatewaySourceResponse = schemas.StrSchema
             __annotations__ = {
                 "Status": Status,
                 "Date": Date,
                 "SplititErrorResultCode": SplititErrorResultCode,
                 "GatewayTransactionID": GatewayTransactionID,
                 "GatewayResultCode": GatewayResultCode,
                 "GatewayResultMessage": GatewayResultMessage,
                 "ThreeDSRedirect": ThreeDSRedirect,
                 "CAVV": CAVV,
                 "ECI": ECI,
+                "GatewaySourceResponse": GatewaySourceResponse,
             }
     
     Status: 'GwAuthorizationStatus'
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Status"]) -> 'GwAuthorizationStatus': ...
     
@@ -90,17 +92,20 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["CAVV"]) -> MetaOapg.properties.CAVV: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["ECI"]) -> MetaOapg.properties.ECI: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["GatewaySourceResponse"]) -> MetaOapg.properties.GatewaySourceResponse: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["Status", "Date", "SplititErrorResultCode", "GatewayTransactionID", "GatewayResultCode", "GatewayResultMessage", "ThreeDSRedirect", "CAVV", "ECI", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["Status", "Date", "SplititErrorResultCode", "GatewayTransactionID", "GatewayResultCode", "GatewayResultMessage", "ThreeDSRedirect", "CAVV", "ECI", "GatewaySourceResponse", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Status"]) -> 'GwAuthorizationStatus': ...
     
@@ -125,17 +130,20 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["CAVV"]) -> typing.Union[MetaOapg.properties.CAVV, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["ECI"]) -> typing.Union[MetaOapg.properties.ECI, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["GatewaySourceResponse"]) -> typing.Union[MetaOapg.properties.GatewaySourceResponse, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["Status", "Date", "SplititErrorResultCode", "GatewayTransactionID", "GatewayResultCode", "GatewayResultMessage", "ThreeDSRedirect", "CAVV", "ECI", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["Status", "Date", "SplititErrorResultCode", "GatewayTransactionID", "GatewayResultCode", "GatewayResultMessage", "ThreeDSRedirect", "CAVV", "ECI", "GatewaySourceResponse", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         Status: 'GwAuthorizationStatus',
@@ -143,14 +151,15 @@
         SplititErrorResultCode: typing.Union[MetaOapg.properties.SplititErrorResultCode, str, schemas.Unset] = schemas.unset,
         GatewayTransactionID: typing.Union[MetaOapg.properties.GatewayTransactionID, str, schemas.Unset] = schemas.unset,
         GatewayResultCode: typing.Union[MetaOapg.properties.GatewayResultCode, str, schemas.Unset] = schemas.unset,
         GatewayResultMessage: typing.Union[MetaOapg.properties.GatewayResultMessage, str, schemas.Unset] = schemas.unset,
         ThreeDSRedirect: typing.Union['ThreeDsRedirectDataV3', schemas.Unset] = schemas.unset,
         CAVV: typing.Union[MetaOapg.properties.CAVV, str, schemas.Unset] = schemas.unset,
         ECI: typing.Union[MetaOapg.properties.ECI, str, schemas.Unset] = schemas.unset,
+        GatewaySourceResponse: typing.Union[MetaOapg.properties.GatewaySourceResponse, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'AuthorizationModel':
         return super().__new__(
             cls,
             *args,
             Status=Status,
@@ -158,13 +167,14 @@
             SplititErrorResultCode=SplititErrorResultCode,
             GatewayTransactionID=GatewayTransactionID,
             GatewayResultCode=GatewayResultCode,
             GatewayResultMessage=GatewayResultMessage,
             ThreeDSRedirect=ThreeDSRedirect,
             CAVV=CAVV,
             ECI=ECI,
+            GatewaySourceResponse=GatewaySourceResponse,
             _configuration=_configuration,
             **kwargs,
         )
 
 from splitit_client.model.gw_authorization_status import GwAuthorizationStatus
 from splitit_client.model.three_ds_redirect_data_v3 import ThreeDsRedirectDataV3
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/card_brand.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/card_brand.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/card_brand.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/card_brand.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/card_data.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/card_data.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/card_data.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/card_data.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/card_type.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/card_type.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/card_type.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/card_type.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/check_installments_eligibility_request.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/check_installments_eligibility_request.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/check_installments_eligibility_request.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/check_installments_eligibility_request.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/error.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/error.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/error.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/error.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/error_extended.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/error_extended.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/error_extended.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/error_extended.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/events_endpoints_model.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/events_endpoints_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/events_endpoints_model.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/events_endpoints_model.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/failed_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/failed_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/failed_response.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/failed_response.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/gw_authorization_status.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/gw_authorization_status.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/gw_authorization_status.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/gw_authorization_status.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/identifier_contract.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/identifier_contract.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/identifier_contract.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/identifier_contract.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/initiate_plan_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/initiate_plan_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/initiate_plan_response.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/initiate_plan_response.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/initiate_redirection_endpoints_model.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/initiate_redirection_endpoints_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/initiate_redirection_endpoints_model.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/initiate_redirection_endpoints_model.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_cancel_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_cancel_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_cancel_response.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_cancel_response.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_create_request.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_create_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,25 +59,30 @@
                 return PaymentMethodModel
         
             @staticmethod
             def RedirectUrls() -> typing.Type['RedirectionEndpointsModel']:
                 return RedirectionEndpointsModel
         
             @staticmethod
+            def ProcessingData() -> typing.Type['ProcessingData']:
+                return ProcessingData
+        
+            @staticmethod
             def EventsEndpoints() -> typing.Type['EventsEndpointsModel']:
                 return EventsEndpointsModel
             __annotations__ = {
                 "AutoCapture": AutoCapture,
                 "TermsAndConditionsAccepted": TermsAndConditionsAccepted,
                 "Attempt3dSecure": Attempt3dSecure,
                 "Shopper": Shopper,
                 "PlanData": PlanData,
                 "BillingAddress": BillingAddress,
                 "PaymentMethod": PaymentMethod,
                 "RedirectUrls": RedirectUrls,
+                "ProcessingData": ProcessingData,
                 "EventsEndpoints": EventsEndpoints,
             }
     
     TermsAndConditionsAccepted: MetaOapg.properties.TermsAndConditionsAccepted
     AutoCapture: MetaOapg.properties.AutoCapture
     
     @typing.overload
@@ -101,20 +106,23 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["PaymentMethod"]) -> 'PaymentMethodModel': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["RedirectUrls"]) -> 'RedirectionEndpointsModel': ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["ProcessingData"]) -> 'ProcessingData': ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["EventsEndpoints"]) -> 'EventsEndpointsModel': ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "TermsAndConditionsAccepted", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "PaymentMethod", "RedirectUrls", "EventsEndpoints", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "TermsAndConditionsAccepted", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "PaymentMethod", "RedirectUrls", "ProcessingData", "EventsEndpoints", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["AutoCapture"]) -> MetaOapg.properties.AutoCapture: ...
     
@@ -136,34 +144,38 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["PaymentMethod"]) -> typing.Union['PaymentMethodModel', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["RedirectUrls"]) -> typing.Union['RedirectionEndpointsModel', schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["ProcessingData"]) -> typing.Union['ProcessingData', schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["EventsEndpoints"]) -> typing.Union['EventsEndpointsModel', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "TermsAndConditionsAccepted", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "PaymentMethod", "RedirectUrls", "EventsEndpoints", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "TermsAndConditionsAccepted", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "PaymentMethod", "RedirectUrls", "ProcessingData", "EventsEndpoints", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         TermsAndConditionsAccepted: typing.Union[MetaOapg.properties.TermsAndConditionsAccepted, bool, ],
         AutoCapture: typing.Union[MetaOapg.properties.AutoCapture, bool, ],
         Attempt3dSecure: typing.Union[MetaOapg.properties.Attempt3dSecure, bool, schemas.Unset] = schemas.unset,
         Shopper: typing.Union['ShopperData', schemas.Unset] = schemas.unset,
         PlanData: typing.Union['PlanDataModel', schemas.Unset] = schemas.unset,
         BillingAddress: typing.Union['AddressDataModel', schemas.Unset] = schemas.unset,
         PaymentMethod: typing.Union['PaymentMethodModel', schemas.Unset] = schemas.unset,
         RedirectUrls: typing.Union['RedirectionEndpointsModel', schemas.Unset] = schemas.unset,
+        ProcessingData: typing.Union['ProcessingData', schemas.Unset] = schemas.unset,
         EventsEndpoints: typing.Union['EventsEndpointsModel', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'InstallmentPlanCreateRequest':
         return super().__new__(
             cls,
             *args,
@@ -171,18 +183,20 @@
             AutoCapture=AutoCapture,
             Attempt3dSecure=Attempt3dSecure,
             Shopper=Shopper,
             PlanData=PlanData,
             BillingAddress=BillingAddress,
             PaymentMethod=PaymentMethod,
             RedirectUrls=RedirectUrls,
+            ProcessingData=ProcessingData,
             EventsEndpoints=EventsEndpoints,
             _configuration=_configuration,
             **kwargs,
         )
 
 from splitit_client.model.address_data_model import AddressDataModel
 from splitit_client.model.events_endpoints_model import EventsEndpointsModel
 from splitit_client.model.payment_method_model import PaymentMethodModel
 from splitit_client.model.plan_data_model import PlanDataModel
+from splitit_client.model.processing_data import ProcessingData
 from splitit_client.model.redirection_endpoints_model import RedirectionEndpointsModel
 from splitit_client.model.shopper_data import ShopperData
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_create_request.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_create_request.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -59,25 +59,30 @@
                 return PaymentMethodModel
         
             @staticmethod
             def RedirectUrls() -> typing.Type['RedirectionEndpointsModel']:
                 return RedirectionEndpointsModel
         
             @staticmethod
+            def ProcessingData() -> typing.Type['ProcessingData']:
+                return ProcessingData
+        
+            @staticmethod
             def EventsEndpoints() -> typing.Type['EventsEndpointsModel']:
                 return EventsEndpointsModel
             __annotations__ = {
                 "AutoCapture": AutoCapture,
                 "TermsAndConditionsAccepted": TermsAndConditionsAccepted,
                 "Attempt3dSecure": Attempt3dSecure,
                 "Shopper": Shopper,
                 "PlanData": PlanData,
                 "BillingAddress": BillingAddress,
                 "PaymentMethod": PaymentMethod,
                 "RedirectUrls": RedirectUrls,
+                "ProcessingData": ProcessingData,
                 "EventsEndpoints": EventsEndpoints,
             }
     
     TermsAndConditionsAccepted: MetaOapg.properties.TermsAndConditionsAccepted
     AutoCapture: MetaOapg.properties.AutoCapture
     
     @typing.overload
@@ -101,20 +106,23 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["PaymentMethod"]) -> 'PaymentMethodModel': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["RedirectUrls"]) -> 'RedirectionEndpointsModel': ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["ProcessingData"]) -> 'ProcessingData': ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["EventsEndpoints"]) -> 'EventsEndpointsModel': ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "TermsAndConditionsAccepted", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "PaymentMethod", "RedirectUrls", "EventsEndpoints", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "TermsAndConditionsAccepted", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "PaymentMethod", "RedirectUrls", "ProcessingData", "EventsEndpoints", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["AutoCapture"]) -> MetaOapg.properties.AutoCapture: ...
     
@@ -136,34 +144,38 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["PaymentMethod"]) -> typing.Union['PaymentMethodModel', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["RedirectUrls"]) -> typing.Union['RedirectionEndpointsModel', schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["ProcessingData"]) -> typing.Union['ProcessingData', schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["EventsEndpoints"]) -> typing.Union['EventsEndpointsModel', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "TermsAndConditionsAccepted", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "PaymentMethod", "RedirectUrls", "EventsEndpoints", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "TermsAndConditionsAccepted", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "PaymentMethod", "RedirectUrls", "ProcessingData", "EventsEndpoints", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         TermsAndConditionsAccepted: typing.Union[MetaOapg.properties.TermsAndConditionsAccepted, bool, ],
         AutoCapture: typing.Union[MetaOapg.properties.AutoCapture, bool, ],
         Attempt3dSecure: typing.Union[MetaOapg.properties.Attempt3dSecure, bool, schemas.Unset] = schemas.unset,
         Shopper: typing.Union['ShopperData', schemas.Unset] = schemas.unset,
         PlanData: typing.Union['PlanDataModel', schemas.Unset] = schemas.unset,
         BillingAddress: typing.Union['AddressDataModel', schemas.Unset] = schemas.unset,
         PaymentMethod: typing.Union['PaymentMethodModel', schemas.Unset] = schemas.unset,
         RedirectUrls: typing.Union['RedirectionEndpointsModel', schemas.Unset] = schemas.unset,
+        ProcessingData: typing.Union['ProcessingData', schemas.Unset] = schemas.unset,
         EventsEndpoints: typing.Union['EventsEndpointsModel', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'InstallmentPlanCreateRequest':
         return super().__new__(
             cls,
             *args,
@@ -171,18 +183,20 @@
             AutoCapture=AutoCapture,
             Attempt3dSecure=Attempt3dSecure,
             Shopper=Shopper,
             PlanData=PlanData,
             BillingAddress=BillingAddress,
             PaymentMethod=PaymentMethod,
             RedirectUrls=RedirectUrls,
+            ProcessingData=ProcessingData,
             EventsEndpoints=EventsEndpoints,
             _configuration=_configuration,
             **kwargs,
         )
 
 from splitit_client.model.address_data_model import AddressDataModel
 from splitit_client.model.events_endpoints_model import EventsEndpointsModel
 from splitit_client.model.payment_method_model import PaymentMethodModel
 from splitit_client.model.plan_data_model import PlanDataModel
+from splitit_client.model.processing_data import ProcessingData
 from splitit_client.model.redirection_endpoints_model import RedirectionEndpointsModel
 from splitit_client.model.shopper_data import ShopperData
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_create_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_create_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_create_response.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_create_response.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_get_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_get_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_get_response.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_get_response.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_initiate_request.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_initiate_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -59,23 +59,28 @@
             @staticmethod
             def UxSettings() -> typing.Type['UxSettingsModel']:
                 return UxSettingsModel
         
             @staticmethod
             def EventsEndpoints() -> typing.Type['EventsEndpointsModel']:
                 return EventsEndpointsModel
+        
+            @staticmethod
+            def ProcessingData() -> typing.Type['ProcessingData']:
+                return ProcessingData
             __annotations__ = {
                 "AutoCapture": AutoCapture,
                 "Attempt3dSecure": Attempt3dSecure,
                 "Shopper": Shopper,
                 "PlanData": PlanData,
                 "BillingAddress": BillingAddress,
                 "RedirectUrls": RedirectUrls,
                 "UxSettings": UxSettings,
                 "EventsEndpoints": EventsEndpoints,
+                "ProcessingData": ProcessingData,
             }
     
     AutoCapture: MetaOapg.properties.AutoCapture
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["AutoCapture"]) -> MetaOapg.properties.AutoCapture: ...
     
@@ -97,17 +102,20 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["UxSettings"]) -> 'UxSettingsModel': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["EventsEndpoints"]) -> 'EventsEndpointsModel': ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["ProcessingData"]) -> 'ProcessingData': ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "RedirectUrls", "UxSettings", "EventsEndpoints", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "RedirectUrls", "UxSettings", "EventsEndpoints", "ProcessingData", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["AutoCapture"]) -> MetaOapg.properties.AutoCapture: ...
     
@@ -129,48 +137,54 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["UxSettings"]) -> typing.Union['UxSettingsModel', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["EventsEndpoints"]) -> typing.Union['EventsEndpointsModel', schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["ProcessingData"]) -> typing.Union['ProcessingData', schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "RedirectUrls", "UxSettings", "EventsEndpoints", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "RedirectUrls", "UxSettings", "EventsEndpoints", "ProcessingData", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         AutoCapture: typing.Union[MetaOapg.properties.AutoCapture, bool, ],
         Attempt3dSecure: typing.Union[MetaOapg.properties.Attempt3dSecure, bool, schemas.Unset] = schemas.unset,
         Shopper: typing.Union['ShopperData', schemas.Unset] = schemas.unset,
         PlanData: typing.Union['PlanDataModel', schemas.Unset] = schemas.unset,
         BillingAddress: typing.Union['AddressDataModel', schemas.Unset] = schemas.unset,
         RedirectUrls: typing.Union['InitiateRedirectionEndpointsModel', schemas.Unset] = schemas.unset,
         UxSettings: typing.Union['UxSettingsModel', schemas.Unset] = schemas.unset,
         EventsEndpoints: typing.Union['EventsEndpointsModel', schemas.Unset] = schemas.unset,
+        ProcessingData: typing.Union['ProcessingData', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'InstallmentPlanInitiateRequest':
         return super().__new__(
             cls,
             *args,
             AutoCapture=AutoCapture,
             Attempt3dSecure=Attempt3dSecure,
             Shopper=Shopper,
             PlanData=PlanData,
             BillingAddress=BillingAddress,
             RedirectUrls=RedirectUrls,
             UxSettings=UxSettings,
             EventsEndpoints=EventsEndpoints,
+            ProcessingData=ProcessingData,
             _configuration=_configuration,
             **kwargs,
         )
 
 from splitit_client.model.address_data_model import AddressDataModel
 from splitit_client.model.events_endpoints_model import EventsEndpointsModel
 from splitit_client.model.initiate_redirection_endpoints_model import InitiateRedirectionEndpointsModel
 from splitit_client.model.plan_data_model import PlanDataModel
+from splitit_client.model.processing_data import ProcessingData
 from splitit_client.model.shopper_data import ShopperData
 from splitit_client.model.ux_settings_model import UxSettingsModel
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_initiate_request.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_initiate_request.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -59,23 +59,28 @@
             @staticmethod
             def UxSettings() -> typing.Type['UxSettingsModel']:
                 return UxSettingsModel
         
             @staticmethod
             def EventsEndpoints() -> typing.Type['EventsEndpointsModel']:
                 return EventsEndpointsModel
+        
+            @staticmethod
+            def ProcessingData() -> typing.Type['ProcessingData']:
+                return ProcessingData
             __annotations__ = {
                 "AutoCapture": AutoCapture,
                 "Attempt3dSecure": Attempt3dSecure,
                 "Shopper": Shopper,
                 "PlanData": PlanData,
                 "BillingAddress": BillingAddress,
                 "RedirectUrls": RedirectUrls,
                 "UxSettings": UxSettings,
                 "EventsEndpoints": EventsEndpoints,
+                "ProcessingData": ProcessingData,
             }
     
     AutoCapture: MetaOapg.properties.AutoCapture
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["AutoCapture"]) -> MetaOapg.properties.AutoCapture: ...
     
@@ -97,17 +102,20 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["UxSettings"]) -> 'UxSettingsModel': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["EventsEndpoints"]) -> 'EventsEndpointsModel': ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["ProcessingData"]) -> 'ProcessingData': ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "RedirectUrls", "UxSettings", "EventsEndpoints", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "RedirectUrls", "UxSettings", "EventsEndpoints", "ProcessingData", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["AutoCapture"]) -> MetaOapg.properties.AutoCapture: ...
     
@@ -129,48 +137,54 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["UxSettings"]) -> typing.Union['UxSettingsModel', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["EventsEndpoints"]) -> typing.Union['EventsEndpointsModel', schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["ProcessingData"]) -> typing.Union['ProcessingData', schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "RedirectUrls", "UxSettings", "EventsEndpoints", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "RedirectUrls", "UxSettings", "EventsEndpoints", "ProcessingData", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         AutoCapture: typing.Union[MetaOapg.properties.AutoCapture, bool, ],
         Attempt3dSecure: typing.Union[MetaOapg.properties.Attempt3dSecure, bool, schemas.Unset] = schemas.unset,
         Shopper: typing.Union['ShopperData', schemas.Unset] = schemas.unset,
         PlanData: typing.Union['PlanDataModel', schemas.Unset] = schemas.unset,
         BillingAddress: typing.Union['AddressDataModel', schemas.Unset] = schemas.unset,
         RedirectUrls: typing.Union['InitiateRedirectionEndpointsModel', schemas.Unset] = schemas.unset,
         UxSettings: typing.Union['UxSettingsModel', schemas.Unset] = schemas.unset,
         EventsEndpoints: typing.Union['EventsEndpointsModel', schemas.Unset] = schemas.unset,
+        ProcessingData: typing.Union['ProcessingData', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'InstallmentPlanInitiateRequest':
         return super().__new__(
             cls,
             *args,
             AutoCapture=AutoCapture,
             Attempt3dSecure=Attempt3dSecure,
             Shopper=Shopper,
             PlanData=PlanData,
             BillingAddress=BillingAddress,
             RedirectUrls=RedirectUrls,
             UxSettings=UxSettings,
             EventsEndpoints=EventsEndpoints,
+            ProcessingData=ProcessingData,
             _configuration=_configuration,
             **kwargs,
         )
 
 from splitit_client.model.address_data_model import AddressDataModel
 from splitit_client.model.events_endpoints_model import EventsEndpointsModel
 from splitit_client.model.initiate_redirection_endpoints_model import InitiateRedirectionEndpointsModel
 from splitit_client.model.plan_data_model import PlanDataModel
+from splitit_client.model.processing_data import ProcessingData
 from splitit_client.model.shopper_data import ShopperData
 from splitit_client.model.ux_settings_model import UxSettingsModel
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_refund_request.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_refund_request.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_refund_request.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_refund_request.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_refund_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_refund_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_refund_response.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_refund_response.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_search_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_search_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_search_response.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_search_response.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_update_request.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_update_request.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_update_request.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_update_request.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_update_request_by_identifier.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_update_request_by_identifier.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_update_request_by_identifier.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_update_request_by_identifier.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_update_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_update_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_plan_update_response.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_plan_update_response.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_status.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_status.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installment_status.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installment_status.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installments_eligibility_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installments_eligibility_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/installments_eligibility_response.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/installments_eligibility_response.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/links_data.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/links_data.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/links_data.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/links_data.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/links_model.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/links_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/links_model.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/links_model.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/payment_method_model.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/shopper_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,92 +19,88 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class PaymentMethodModel(
+class ShopperData(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
-        required = {
-            "Type",
-        }
         
         class properties:
-        
-            @staticmethod
-            def Type() -> typing.Type['PaymentMethodType']:
-                return PaymentMethodType
-        
-            @staticmethod
-            def Card() -> typing.Type['CardData']:
-                return CardData
-            Token = schemas.StrSchema
+            FullName = schemas.StrSchema
+            Email = schemas.StrSchema
+            PhoneNumber = schemas.StrSchema
+            Culture = schemas.StrSchema
             __annotations__ = {
-                "Type": Type,
-                "Card": Card,
-                "Token": Token,
+                "FullName": FullName,
+                "Email": Email,
+                "PhoneNumber": PhoneNumber,
+                "Culture": Culture,
             }
     
-    Type: 'PaymentMethodType'
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["FullName"]) -> MetaOapg.properties.FullName: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Type"]) -> 'PaymentMethodType': ...
+    def __getitem__(self, name: typing_extensions.Literal["Email"]) -> MetaOapg.properties.Email: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Card"]) -> 'CardData': ...
+    def __getitem__(self, name: typing_extensions.Literal["PhoneNumber"]) -> MetaOapg.properties.PhoneNumber: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Token"]) -> MetaOapg.properties.Token: ...
+    def __getitem__(self, name: typing_extensions.Literal["Culture"]) -> MetaOapg.properties.Culture: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["Type", "Card", "Token", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["FullName", "Email", "PhoneNumber", "Culture", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Type"]) -> 'PaymentMethodType': ...
+    def get_item_oapg(self, name: typing_extensions.Literal["FullName"]) -> typing.Union[MetaOapg.properties.FullName, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Card"]) -> typing.Union['CardData', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Email"]) -> typing.Union[MetaOapg.properties.Email, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Token"]) -> typing.Union[MetaOapg.properties.Token, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["PhoneNumber"]) -> typing.Union[MetaOapg.properties.PhoneNumber, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["Culture"]) -> typing.Union[MetaOapg.properties.Culture, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["Type", "Card", "Token", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["FullName", "Email", "PhoneNumber", "Culture", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        Type: 'PaymentMethodType',
-        Card: typing.Union['CardData', schemas.Unset] = schemas.unset,
-        Token: typing.Union[MetaOapg.properties.Token, str, schemas.Unset] = schemas.unset,
+        FullName: typing.Union[MetaOapg.properties.FullName, str, schemas.Unset] = schemas.unset,
+        Email: typing.Union[MetaOapg.properties.Email, str, schemas.Unset] = schemas.unset,
+        PhoneNumber: typing.Union[MetaOapg.properties.PhoneNumber, str, schemas.Unset] = schemas.unset,
+        Culture: typing.Union[MetaOapg.properties.Culture, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'PaymentMethodModel':
+    ) -> 'ShopperData':
         return super().__new__(
             cls,
             *args,
-            Type=Type,
-            Card=Card,
-            Token=Token,
+            FullName=FullName,
+            Email=Email,
+            PhoneNumber=PhoneNumber,
+            Culture=Culture,
             _configuration=_configuration,
             **kwargs,
         )
-
-from splitit_client.model.card_data import CardData
-from splitit_client.model.payment_method_type import PaymentMethodType
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/payment_method_model.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/shopper_data.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -19,92 +19,88 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class PaymentMethodModel(
+class ShopperData(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
-        required = {
-            "Type",
-        }
         
         class properties:
-        
-            @staticmethod
-            def Type() -> typing.Type['PaymentMethodType']:
-                return PaymentMethodType
-        
-            @staticmethod
-            def Card() -> typing.Type['CardData']:
-                return CardData
-            Token = schemas.StrSchema
+            FullName = schemas.StrSchema
+            Email = schemas.StrSchema
+            PhoneNumber = schemas.StrSchema
+            Culture = schemas.StrSchema
             __annotations__ = {
-                "Type": Type,
-                "Card": Card,
-                "Token": Token,
+                "FullName": FullName,
+                "Email": Email,
+                "PhoneNumber": PhoneNumber,
+                "Culture": Culture,
             }
     
-    Type: 'PaymentMethodType'
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["FullName"]) -> MetaOapg.properties.FullName: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Type"]) -> 'PaymentMethodType': ...
+    def __getitem__(self, name: typing_extensions.Literal["Email"]) -> MetaOapg.properties.Email: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Card"]) -> 'CardData': ...
+    def __getitem__(self, name: typing_extensions.Literal["PhoneNumber"]) -> MetaOapg.properties.PhoneNumber: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Token"]) -> MetaOapg.properties.Token: ...
+    def __getitem__(self, name: typing_extensions.Literal["Culture"]) -> MetaOapg.properties.Culture: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["Type", "Card", "Token", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["FullName", "Email", "PhoneNumber", "Culture", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Type"]) -> 'PaymentMethodType': ...
+    def get_item_oapg(self, name: typing_extensions.Literal["FullName"]) -> typing.Union[MetaOapg.properties.FullName, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Card"]) -> typing.Union['CardData', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Email"]) -> typing.Union[MetaOapg.properties.Email, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Token"]) -> typing.Union[MetaOapg.properties.Token, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["PhoneNumber"]) -> typing.Union[MetaOapg.properties.PhoneNumber, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["Culture"]) -> typing.Union[MetaOapg.properties.Culture, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["Type", "Card", "Token", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["FullName", "Email", "PhoneNumber", "Culture", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        Type: 'PaymentMethodType',
-        Card: typing.Union['CardData', schemas.Unset] = schemas.unset,
-        Token: typing.Union[MetaOapg.properties.Token, str, schemas.Unset] = schemas.unset,
+        FullName: typing.Union[MetaOapg.properties.FullName, str, schemas.Unset] = schemas.unset,
+        Email: typing.Union[MetaOapg.properties.Email, str, schemas.Unset] = schemas.unset,
+        PhoneNumber: typing.Union[MetaOapg.properties.PhoneNumber, str, schemas.Unset] = schemas.unset,
+        Culture: typing.Union[MetaOapg.properties.Culture, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'PaymentMethodModel':
+    ) -> 'ShopperData':
         return super().__new__(
             cls,
             *args,
-            Type=Type,
-            Card=Card,
-            Token=Token,
+            FullName=FullName,
+            Email=Email,
+            PhoneNumber=PhoneNumber,
+            Culture=Culture,
             _configuration=_configuration,
             **kwargs,
         )
-
-from splitit_client.model.card_data import CardData
-from splitit_client.model.payment_method_type import PaymentMethodType
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/payment_method_type.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/purchase_method.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,29 +19,34 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class PaymentMethodType(
+class PurchaseMethod(
     schemas.EnumBase,
     schemas.StrSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         enum_value_to_name = {
-            "Card": "CARD",
-            "SplititToken": "SPLITIT_TOKEN",
+            "InStore": "IN_STORE",
+            "PhoneOrder": "PHONE_ORDER",
+            "ECommerce": "ECOMMERCE",
         }
     
     @schemas.classproperty
-    def CARD(cls):
-        return cls("Card")
+    def IN_STORE(cls):
+        return cls("InStore")
     
     @schemas.classproperty
-    def SPLITIT_TOKEN(cls):
-        return cls("SplititToken")
+    def PHONE_ORDER(cls):
+        return cls("PhoneOrder")
+    
+    @schemas.classproperty
+    def ECOMMERCE(cls):
+        return cls("ECommerce")
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/payment_method_type.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/shipping_status.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -19,22 +19,26 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class PaymentMethodType(
+class ShippingStatus(
     schemas.EnumBase,
     schemas.StrSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
     
     @schemas.classproperty
-    def CARD(cls):
-        return cls("Card")
+    def PENDING(cls):
+        return cls("Pending")
     
     @schemas.classproperty
-    def SPLITIT_TOKEN(cls):
-        return cls("SplititToken")
+    def SHIPPED(cls):
+        return cls("Shipped")
+    
+    @schemas.classproperty
+    def DELIVERED(cls):
+        return cls("Delivered")
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/payment_plan_option_model.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/payment_plan_option_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/payment_plan_option_model.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/payment_plan_option_model.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/plan_data.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/plan_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,25 +97,30 @@
                 ) -> 'Tags':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
+        
+            @staticmethod
+            def ProcessingData() -> typing.Type['ProcessingData2']:
+                return ProcessingData2
             FirstInstallmentDate = schemas.DateTimeSchema
             __annotations__ = {
                 "TotalAmount": TotalAmount,
                 "NumberOfInstallments": NumberOfInstallments,
                 "PurchaseMethod": PurchaseMethod,
                 "TerminalId": TerminalId,
                 "FirstInstallmentAmount": FirstInstallmentAmount,
                 "Currency": Currency,
                 "RefOrderNumber": RefOrderNumber,
                 "AllowedInstallmentOptions": AllowedInstallmentOptions,
                 "Tags": Tags,
+                "ProcessingData": ProcessingData,
                 "FirstInstallmentDate": FirstInstallmentDate,
             }
     
     PurchaseMethod: 'PurchaseMethod'
     TotalAmount: MetaOapg.properties.TotalAmount
     NumberOfInstallments: MetaOapg.properties.NumberOfInstallments
     
@@ -143,20 +148,23 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["AllowedInstallmentOptions"]) -> MetaOapg.properties.AllowedInstallmentOptions: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Tags"]) -> MetaOapg.properties.Tags: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["ProcessingData"]) -> 'ProcessingData2': ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["FirstInstallmentDate"]) -> MetaOapg.properties.FirstInstallmentDate: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["TotalAmount", "NumberOfInstallments", "PurchaseMethod", "TerminalId", "FirstInstallmentAmount", "Currency", "RefOrderNumber", "AllowedInstallmentOptions", "Tags", "FirstInstallmentDate", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["TotalAmount", "NumberOfInstallments", "PurchaseMethod", "TerminalId", "FirstInstallmentAmount", "Currency", "RefOrderNumber", "AllowedInstallmentOptions", "Tags", "ProcessingData", "FirstInstallmentDate", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["TotalAmount"]) -> MetaOapg.properties.TotalAmount: ...
     
@@ -181,20 +189,23 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["AllowedInstallmentOptions"]) -> typing.Union[MetaOapg.properties.AllowedInstallmentOptions, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Tags"]) -> typing.Union[MetaOapg.properties.Tags, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["ProcessingData"]) -> typing.Union['ProcessingData2', schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["FirstInstallmentDate"]) -> typing.Union[MetaOapg.properties.FirstInstallmentDate, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["TotalAmount", "NumberOfInstallments", "PurchaseMethod", "TerminalId", "FirstInstallmentAmount", "Currency", "RefOrderNumber", "AllowedInstallmentOptions", "Tags", "FirstInstallmentDate", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["TotalAmount", "NumberOfInstallments", "PurchaseMethod", "TerminalId", "FirstInstallmentAmount", "Currency", "RefOrderNumber", "AllowedInstallmentOptions", "Tags", "ProcessingData", "FirstInstallmentDate", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         PurchaseMethod: 'PurchaseMethod',
@@ -202,14 +213,15 @@
         NumberOfInstallments: typing.Union[MetaOapg.properties.NumberOfInstallments, decimal.Decimal, int, ],
         TerminalId: typing.Union[MetaOapg.properties.TerminalId, str, schemas.Unset] = schemas.unset,
         FirstInstallmentAmount: typing.Union[MetaOapg.properties.FirstInstallmentAmount, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         Currency: typing.Union[MetaOapg.properties.Currency, str, schemas.Unset] = schemas.unset,
         RefOrderNumber: typing.Union[MetaOapg.properties.RefOrderNumber, str, schemas.Unset] = schemas.unset,
         AllowedInstallmentOptions: typing.Union[MetaOapg.properties.AllowedInstallmentOptions, list, tuple, schemas.Unset] = schemas.unset,
         Tags: typing.Union[MetaOapg.properties.Tags, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
+        ProcessingData: typing.Union['ProcessingData2', schemas.Unset] = schemas.unset,
         FirstInstallmentDate: typing.Union[MetaOapg.properties.FirstInstallmentDate, str, datetime, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'PlanData':
         return super().__new__(
             cls,
             *args,
@@ -218,13 +230,15 @@
             NumberOfInstallments=NumberOfInstallments,
             TerminalId=TerminalId,
             FirstInstallmentAmount=FirstInstallmentAmount,
             Currency=Currency,
             RefOrderNumber=RefOrderNumber,
             AllowedInstallmentOptions=AllowedInstallmentOptions,
             Tags=Tags,
+            ProcessingData=ProcessingData,
             FirstInstallmentDate=FirstInstallmentDate,
             _configuration=_configuration,
             **kwargs,
         )
 
+from splitit_client.model.processing_data2 import ProcessingData2
 from splitit_client.model.purchase_method import PurchaseMethod
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/plan_data.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/plan_data.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -97,25 +97,30 @@
                 ) -> 'Tags':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
+        
+            @staticmethod
+            def ProcessingData() -> typing.Type['ProcessingData2']:
+                return ProcessingData2
             FirstInstallmentDate = schemas.DateTimeSchema
             __annotations__ = {
                 "TotalAmount": TotalAmount,
                 "NumberOfInstallments": NumberOfInstallments,
                 "PurchaseMethod": PurchaseMethod,
                 "TerminalId": TerminalId,
                 "FirstInstallmentAmount": FirstInstallmentAmount,
                 "Currency": Currency,
                 "RefOrderNumber": RefOrderNumber,
                 "AllowedInstallmentOptions": AllowedInstallmentOptions,
                 "Tags": Tags,
+                "ProcessingData": ProcessingData,
                 "FirstInstallmentDate": FirstInstallmentDate,
             }
     
     PurchaseMethod: 'PurchaseMethod'
     TotalAmount: MetaOapg.properties.TotalAmount
     NumberOfInstallments: MetaOapg.properties.NumberOfInstallments
     
@@ -143,20 +148,23 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["AllowedInstallmentOptions"]) -> MetaOapg.properties.AllowedInstallmentOptions: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["Tags"]) -> MetaOapg.properties.Tags: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["ProcessingData"]) -> 'ProcessingData2': ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["FirstInstallmentDate"]) -> MetaOapg.properties.FirstInstallmentDate: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["TotalAmount", "NumberOfInstallments", "PurchaseMethod", "TerminalId", "FirstInstallmentAmount", "Currency", "RefOrderNumber", "AllowedInstallmentOptions", "Tags", "FirstInstallmentDate", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["TotalAmount", "NumberOfInstallments", "PurchaseMethod", "TerminalId", "FirstInstallmentAmount", "Currency", "RefOrderNumber", "AllowedInstallmentOptions", "Tags", "ProcessingData", "FirstInstallmentDate", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["TotalAmount"]) -> MetaOapg.properties.TotalAmount: ...
     
@@ -181,20 +189,23 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["AllowedInstallmentOptions"]) -> typing.Union[MetaOapg.properties.AllowedInstallmentOptions, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["Tags"]) -> typing.Union[MetaOapg.properties.Tags, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["ProcessingData"]) -> typing.Union['ProcessingData2', schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["FirstInstallmentDate"]) -> typing.Union[MetaOapg.properties.FirstInstallmentDate, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["TotalAmount", "NumberOfInstallments", "PurchaseMethod", "TerminalId", "FirstInstallmentAmount", "Currency", "RefOrderNumber", "AllowedInstallmentOptions", "Tags", "FirstInstallmentDate", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["TotalAmount", "NumberOfInstallments", "PurchaseMethod", "TerminalId", "FirstInstallmentAmount", "Currency", "RefOrderNumber", "AllowedInstallmentOptions", "Tags", "ProcessingData", "FirstInstallmentDate", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         PurchaseMethod: 'PurchaseMethod',
@@ -202,14 +213,15 @@
         NumberOfInstallments: typing.Union[MetaOapg.properties.NumberOfInstallments, decimal.Decimal, int, ],
         TerminalId: typing.Union[MetaOapg.properties.TerminalId, str, schemas.Unset] = schemas.unset,
         FirstInstallmentAmount: typing.Union[MetaOapg.properties.FirstInstallmentAmount, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         Currency: typing.Union[MetaOapg.properties.Currency, str, schemas.Unset] = schemas.unset,
         RefOrderNumber: typing.Union[MetaOapg.properties.RefOrderNumber, str, schemas.Unset] = schemas.unset,
         AllowedInstallmentOptions: typing.Union[MetaOapg.properties.AllowedInstallmentOptions, list, tuple, schemas.Unset] = schemas.unset,
         Tags: typing.Union[MetaOapg.properties.Tags, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
+        ProcessingData: typing.Union['ProcessingData2', schemas.Unset] = schemas.unset,
         FirstInstallmentDate: typing.Union[MetaOapg.properties.FirstInstallmentDate, str, datetime, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'PlanData':
         return super().__new__(
             cls,
             *args,
@@ -218,13 +230,15 @@
             NumberOfInstallments=NumberOfInstallments,
             TerminalId=TerminalId,
             FirstInstallmentAmount=FirstInstallmentAmount,
             Currency=Currency,
             RefOrderNumber=RefOrderNumber,
             AllowedInstallmentOptions=AllowedInstallmentOptions,
             Tags=Tags,
+            ProcessingData=ProcessingData,
             FirstInstallmentDate=FirstInstallmentDate,
             _configuration=_configuration,
             **kwargs,
         )
 
+from splitit_client.model.processing_data2 import ProcessingData2
 from splitit_client.model.purchase_method import PurchaseMethod
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/plan_data_model.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/plan_data_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/plan_data_model.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/plan_data_model.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/plan_error_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/plan_error_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/plan_error_response.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/plan_error_response.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/plan_status.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/plan_status.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/plan_status.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/plan_status.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/purchase_method.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/shipping_status.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,34 +19,34 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class PurchaseMethod(
+class ShippingStatus(
     schemas.EnumBase,
     schemas.StrSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         enum_value_to_name = {
-            "InStore": "IN_STORE",
-            "PhoneOrder": "PHONE_ORDER",
-            "ECommerce": "ECOMMERCE",
+            "Pending": "PENDING",
+            "Shipped": "SHIPPED",
+            "Delivered": "DELIVERED",
         }
     
     @schemas.classproperty
-    def IN_STORE(cls):
-        return cls("InStore")
+    def PENDING(cls):
+        return cls("Pending")
     
     @schemas.classproperty
-    def PHONE_ORDER(cls):
-        return cls("PhoneOrder")
+    def SHIPPED(cls):
+        return cls("Shipped")
     
     @schemas.classproperty
-    def ECOMMERCE(cls):
-        return cls("ECommerce")
+    def DELIVERED(cls):
+        return cls("Delivered")
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/purchase_method.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/purchase_method.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/redirection_endpoints_model.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/redirection_endpoints_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/redirection_endpoints_model.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/redirection_endpoints_model.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/refund_model.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/refund_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/refund_model.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/refund_model.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/refund_status.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/refund_status.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/refund_status.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/refund_status.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/refund_strategy.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/refund_strategy.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/refund_strategy.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/refund_strategy.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/refund_summary.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/refund_summary.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/refund_summary.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/refund_summary.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/search_installment_plan_response_item.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/search_installment_plan_response_item.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/search_installment_plan_response_item.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/search_installment_plan_response_item.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/shipping_status.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/shipping_status2.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,34 +19,29 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class ShippingStatus(
+class ShippingStatus2(
     schemas.EnumBase,
     schemas.StrSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         enum_value_to_name = {
-            "Pending": "PENDING",
             "Shipped": "SHIPPED",
             "Delivered": "DELIVERED",
         }
     
     @schemas.classproperty
-    def PENDING(cls):
-        return cls("Pending")
-    
-    @schemas.classproperty
     def SHIPPED(cls):
         return cls("Shipped")
     
     @schemas.classproperty
     def DELIVERED(cls):
         return cls("Delivered")
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/shipping_status.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/shipping_status2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -19,26 +19,22 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class ShippingStatus(
+class ShippingStatus2(
     schemas.EnumBase,
     schemas.StrSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
     
     @schemas.classproperty
-    def PENDING(cls):
-        return cls("Pending")
-    
-    @schemas.classproperty
     def SHIPPED(cls):
         return cls("Shipped")
     
     @schemas.classproperty
     def DELIVERED(cls):
         return cls("Delivered")
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/shipping_status2.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/test_modes.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -19,29 +19,30 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class ShippingStatus2(
+class TestModes(
     schemas.EnumBase,
     schemas.StrSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
-
-
-    class MetaOapg:
-        enum_value_to_name = {
-            "Shipped": "SHIPPED",
-            "Delivered": "DELIVERED",
-        }
     
     @schemas.classproperty
-    def SHIPPED(cls):
-        return cls("Shipped")
+    def NONE(cls):
+        return cls("None")
+    
+    @schemas.classproperty
+    def REGULAR(cls):
+        return cls("Regular")
+    
+    @schemas.classproperty
+    def FAST(cls):
+        return cls("Fast")
     
     @schemas.classproperty
-    def DELIVERED(cls):
-        return cls("Delivered")
+    def AUTOMATION(cls):
+        return cls("Automation")
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/shopper_data.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/update_order_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,88 +19,93 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class ShopperData(
+class UpdateOrderRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
-            FullName = schemas.StrSchema
-            Email = schemas.StrSchema
-            PhoneNumber = schemas.StrSchema
-            Culture = schemas.StrSchema
+            TrackingNumber = schemas.StrSchema
+            RefOrderNumber = schemas.StrSchema
+        
+            @staticmethod
+            def ShippingStatus() -> typing.Type['ShippingStatus']:
+                return ShippingStatus
+            Capture = schemas.BoolSchema
             __annotations__ = {
-                "FullName": FullName,
-                "Email": Email,
-                "PhoneNumber": PhoneNumber,
-                "Culture": Culture,
+                "TrackingNumber": TrackingNumber,
+                "RefOrderNumber": RefOrderNumber,
+                "ShippingStatus": ShippingStatus,
+                "Capture": Capture,
             }
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["FullName"]) -> MetaOapg.properties.FullName: ...
+    def __getitem__(self, name: typing_extensions.Literal["TrackingNumber"]) -> MetaOapg.properties.TrackingNumber: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Email"]) -> MetaOapg.properties.Email: ...
+    def __getitem__(self, name: typing_extensions.Literal["RefOrderNumber"]) -> MetaOapg.properties.RefOrderNumber: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["PhoneNumber"]) -> MetaOapg.properties.PhoneNumber: ...
+    def __getitem__(self, name: typing_extensions.Literal["ShippingStatus"]) -> 'ShippingStatus': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Culture"]) -> MetaOapg.properties.Culture: ...
+    def __getitem__(self, name: typing_extensions.Literal["Capture"]) -> MetaOapg.properties.Capture: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["FullName", "Email", "PhoneNumber", "Culture", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["TrackingNumber", "RefOrderNumber", "ShippingStatus", "Capture", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["FullName"]) -> typing.Union[MetaOapg.properties.FullName, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["TrackingNumber"]) -> typing.Union[MetaOapg.properties.TrackingNumber, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Email"]) -> typing.Union[MetaOapg.properties.Email, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["RefOrderNumber"]) -> typing.Union[MetaOapg.properties.RefOrderNumber, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["PhoneNumber"]) -> typing.Union[MetaOapg.properties.PhoneNumber, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["ShippingStatus"]) -> typing.Union['ShippingStatus', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Culture"]) -> typing.Union[MetaOapg.properties.Culture, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Capture"]) -> typing.Union[MetaOapg.properties.Capture, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["FullName", "Email", "PhoneNumber", "Culture", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["TrackingNumber", "RefOrderNumber", "ShippingStatus", "Capture", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        FullName: typing.Union[MetaOapg.properties.FullName, str, schemas.Unset] = schemas.unset,
-        Email: typing.Union[MetaOapg.properties.Email, str, schemas.Unset] = schemas.unset,
-        PhoneNumber: typing.Union[MetaOapg.properties.PhoneNumber, str, schemas.Unset] = schemas.unset,
-        Culture: typing.Union[MetaOapg.properties.Culture, str, schemas.Unset] = schemas.unset,
+        TrackingNumber: typing.Union[MetaOapg.properties.TrackingNumber, str, schemas.Unset] = schemas.unset,
+        RefOrderNumber: typing.Union[MetaOapg.properties.RefOrderNumber, str, schemas.Unset] = schemas.unset,
+        ShippingStatus: typing.Union['ShippingStatus', schemas.Unset] = schemas.unset,
+        Capture: typing.Union[MetaOapg.properties.Capture, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'ShopperData':
+    ) -> 'UpdateOrderRequest':
         return super().__new__(
             cls,
             *args,
-            FullName=FullName,
-            Email=Email,
-            PhoneNumber=PhoneNumber,
-            Culture=Culture,
+            TrackingNumber=TrackingNumber,
+            RefOrderNumber=RefOrderNumber,
+            ShippingStatus=ShippingStatus,
+            Capture=Capture,
             _configuration=_configuration,
             **kwargs,
         )
+
+from splitit_client.model.shipping_status import ShippingStatus
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/shopper_data.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/update_order_request.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -19,88 +19,93 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 
-class ShopperData(
+class UpdateOrderRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         class properties:
-            FullName = schemas.StrSchema
-            Email = schemas.StrSchema
-            PhoneNumber = schemas.StrSchema
-            Culture = schemas.StrSchema
+            TrackingNumber = schemas.StrSchema
+            RefOrderNumber = schemas.StrSchema
+        
+            @staticmethod
+            def ShippingStatus() -> typing.Type['ShippingStatus']:
+                return ShippingStatus
+            Capture = schemas.BoolSchema
             __annotations__ = {
-                "FullName": FullName,
-                "Email": Email,
-                "PhoneNumber": PhoneNumber,
-                "Culture": Culture,
+                "TrackingNumber": TrackingNumber,
+                "RefOrderNumber": RefOrderNumber,
+                "ShippingStatus": ShippingStatus,
+                "Capture": Capture,
             }
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["FullName"]) -> MetaOapg.properties.FullName: ...
+    def __getitem__(self, name: typing_extensions.Literal["TrackingNumber"]) -> MetaOapg.properties.TrackingNumber: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Email"]) -> MetaOapg.properties.Email: ...
+    def __getitem__(self, name: typing_extensions.Literal["RefOrderNumber"]) -> MetaOapg.properties.RefOrderNumber: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["PhoneNumber"]) -> MetaOapg.properties.PhoneNumber: ...
+    def __getitem__(self, name: typing_extensions.Literal["ShippingStatus"]) -> 'ShippingStatus': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["Culture"]) -> MetaOapg.properties.Culture: ...
+    def __getitem__(self, name: typing_extensions.Literal["Capture"]) -> MetaOapg.properties.Capture: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["FullName", "Email", "PhoneNumber", "Culture", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["TrackingNumber", "RefOrderNumber", "ShippingStatus", "Capture", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["FullName"]) -> typing.Union[MetaOapg.properties.FullName, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["TrackingNumber"]) -> typing.Union[MetaOapg.properties.TrackingNumber, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Email"]) -> typing.Union[MetaOapg.properties.Email, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["RefOrderNumber"]) -> typing.Union[MetaOapg.properties.RefOrderNumber, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["PhoneNumber"]) -> typing.Union[MetaOapg.properties.PhoneNumber, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["ShippingStatus"]) -> typing.Union['ShippingStatus', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["Culture"]) -> typing.Union[MetaOapg.properties.Culture, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["Capture"]) -> typing.Union[MetaOapg.properties.Capture, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["FullName", "Email", "PhoneNumber", "Culture", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["TrackingNumber", "RefOrderNumber", "ShippingStatus", "Capture", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        FullName: typing.Union[MetaOapg.properties.FullName, str, schemas.Unset] = schemas.unset,
-        Email: typing.Union[MetaOapg.properties.Email, str, schemas.Unset] = schemas.unset,
-        PhoneNumber: typing.Union[MetaOapg.properties.PhoneNumber, str, schemas.Unset] = schemas.unset,
-        Culture: typing.Union[MetaOapg.properties.Culture, str, schemas.Unset] = schemas.unset,
+        TrackingNumber: typing.Union[MetaOapg.properties.TrackingNumber, str, schemas.Unset] = schemas.unset,
+        RefOrderNumber: typing.Union[MetaOapg.properties.RefOrderNumber, str, schemas.Unset] = schemas.unset,
+        ShippingStatus: typing.Union['ShippingStatus', schemas.Unset] = schemas.unset,
+        Capture: typing.Union[MetaOapg.properties.Capture, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'ShopperData':
+    ) -> 'UpdateOrderRequest':
         return super().__new__(
             cls,
             *args,
-            FullName=FullName,
-            Email=Email,
-            PhoneNumber=PhoneNumber,
-            Culture=Culture,
+            TrackingNumber=TrackingNumber,
+            RefOrderNumber=RefOrderNumber,
+            ShippingStatus=ShippingStatus,
+            Capture=Capture,
             _configuration=_configuration,
             **kwargs,
         )
+
+from splitit_client.model.shipping_status import ShippingStatus
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/test_modes.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/test_modes.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/three_ds_redirect_data_v3.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/three_ds_redirect_data_v3.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/three_ds_redirect_data_v3.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/three_ds_redirect_data_v3.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/ux_settings_model.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/ux_settings_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/ux_settings_model.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/ux_settings_model.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/verify_authorization_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/model/verify_authorization_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/model/verify_authorization_response.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/model/verify_authorization_response.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/models/__init__.py` & `splitit_web_python_sdk-2.5.0/splitit_client/models/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,22 +10,24 @@
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
 from splitit_client.model.address_data import AddressData
 from splitit_client.model.address_data_model import AddressDataModel
 from splitit_client.model.authorization_model import AuthorizationModel
+from splitit_client.model.bluesnap_vaulted_shopper_token import BluesnapVaultedShopperToken
 from splitit_client.model.card_brand import CardBrand
 from splitit_client.model.card_data import CardData
 from splitit_client.model.card_type import CardType
 from splitit_client.model.check_installments_eligibility_request import CheckInstallmentsEligibilityRequest
 from splitit_client.model.error import Error
 from splitit_client.model.error_extended import ErrorExtended
 from splitit_client.model.events_endpoints_model import EventsEndpointsModel
 from splitit_client.model.failed_response import FailedResponse
+from splitit_client.model.gateway_token_data import GatewayTokenData
 from splitit_client.model.gw_authorization_status import GwAuthorizationStatus
 from splitit_client.model.identifier_contract import IdentifierContract
 from splitit_client.model.initiate_plan_response import InitiatePlanResponse
 from splitit_client.model.initiate_redirection_endpoints_model import InitiateRedirectionEndpointsModel
 from splitit_client.model.installment import Installment
 from splitit_client.model.installment_plan_cancel_response import InstallmentPlanCancelResponse
 from splitit_client.model.installment_plan_create_request import InstallmentPlanCreateRequest
@@ -38,29 +40,34 @@
 from splitit_client.model.installment_plan_update_request import InstallmentPlanUpdateRequest
 from splitit_client.model.installment_plan_update_request_by_identifier import InstallmentPlanUpdateRequestByIdentifier
 from splitit_client.model.installment_plan_update_response import InstallmentPlanUpdateResponse
 from splitit_client.model.installment_status import InstallmentStatus
 from splitit_client.model.installments_eligibility_response import InstallmentsEligibilityResponse
 from splitit_client.model.links_data import LinksData
 from splitit_client.model.links_model import LinksModel
+from splitit_client.model.mocker_shopper_token import MockerShopperToken
 from splitit_client.model.payment_method_model import PaymentMethodModel
 from splitit_client.model.payment_method_type import PaymentMethodType
 from splitit_client.model.payment_plan_option_model import PaymentPlanOptionModel
 from splitit_client.model.plan_data import PlanData
 from splitit_client.model.plan_data_model import PlanDataModel
 from splitit_client.model.plan_error_response import PlanErrorResponse
 from splitit_client.model.plan_status import PlanStatus
+from splitit_client.model.processing_data import ProcessingData
+from splitit_client.model.processing_data2 import ProcessingData2
 from splitit_client.model.purchase_method import PurchaseMethod
 from splitit_client.model.redirection_endpoints_model import RedirectionEndpointsModel
 from splitit_client.model.refund_model import RefundModel
 from splitit_client.model.refund_status import RefundStatus
 from splitit_client.model.refund_strategy import RefundStrategy
 from splitit_client.model.refund_summary import RefundSummary
 from splitit_client.model.search_installment_plan_response_item import SearchInstallmentPlanResponseItem
 from splitit_client.model.shipping_status import ShippingStatus
 from splitit_client.model.shipping_status2 import ShippingStatus2
 from splitit_client.model.shopper_data import ShopperData
 from splitit_client.model.test_modes import TestModes
+from splitit_client.model.three_ds_data import ThreeDSData
+from splitit_client.model.three_ds_data2 import ThreeDSData2
 from splitit_client.model.three_ds_redirect_data_v3 import ThreeDsRedirectDataV3
 from splitit_client.model.update_order_request import UpdateOrderRequest
 from splitit_client.model.ux_settings_model import UxSettingsModel
 from splitit_client.model.verify_authorization_response import VerifyAuthorizationResponse
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/paths/__init__.py` & `splitit_web_python_sdk-2.5.0/splitit_client/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans/post.py` & `splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans/post.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
+from splitit_client.model.processing_data import ProcessingData as ProcessingDataSchema
 from splitit_client.model.plan_error_response import PlanErrorResponse as PlanErrorResponseSchema
 from splitit_client.model.failed_response import FailedResponse as FailedResponseSchema
 from splitit_client.model.address_data_model import AddressDataModel as AddressDataModelSchema
 from splitit_client.model.installment_plan_create_response import InstallmentPlanCreateResponse as InstallmentPlanCreateResponseSchema
 from splitit_client.model.plan_data_model import PlanDataModel as PlanDataModelSchema
 from splitit_client.model.events_endpoints_model import EventsEndpointsModel as EventsEndpointsModelSchema
 from splitit_client.model.installment_plan_create_request import InstallmentPlanCreateRequest as InstallmentPlanCreateRequestSchema
@@ -42,14 +43,15 @@
 from splitit_client.model.redirection_endpoints_model import RedirectionEndpointsModel as RedirectionEndpointsModelSchema
 from splitit_client.model.shopper_data import ShopperData as ShopperDataSchema
 
 from splitit_client.type.failed_response import FailedResponse
 from splitit_client.type.address_data_model import AddressDataModel
 from splitit_client.type.plan_error_response import PlanErrorResponse
 from splitit_client.type.installment_plan_create_response import InstallmentPlanCreateResponse
+from splitit_client.type.processing_data import ProcessingData
 from splitit_client.type.installment_plan_create_request import InstallmentPlanCreateRequest
 from splitit_client.type.events_endpoints_model import EventsEndpointsModel
 from splitit_client.type.plan_data_model import PlanDataModel
 from splitit_client.type.shopper_data import ShopperData
 from splitit_client.type.payment_method_model import PaymentMethodModel
 from splitit_client.type.redirection_endpoints_model import RedirectionEndpointsModel
 
@@ -336,14 +338,15 @@
         x_splitit_touch_point: str,
         attempt3d_secure: typing.Optional[bool] = None,
         shopper: typing.Optional[ShopperData] = None,
         plan_data: typing.Optional[PlanDataModel] = None,
         billing_address: typing.Optional[AddressDataModel] = None,
         payment_method: typing.Optional[PaymentMethodModel] = None,
         redirect_urls: typing.Optional[RedirectionEndpointsModel] = None,
+        processing_data: typing.Optional[ProcessingData] = None,
         events_endpoints: typing.Optional[EventsEndpointsModel] = None,
         x_splitit_test_mode: typing.Optional[str] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _header_params = {}
         _body = {}
         if auto_capture is not None:
@@ -358,14 +361,16 @@
             _body["PlanData"] = plan_data
         if billing_address is not None:
             _body["BillingAddress"] = billing_address
         if payment_method is not None:
             _body["PaymentMethod"] = payment_method
         if redirect_urls is not None:
             _body["RedirectUrls"] = redirect_urls
+        if processing_data is not None:
+            _body["ProcessingData"] = processing_data
         if events_endpoints is not None:
             _body["EventsEndpoints"] = events_endpoints
         args.body = _body
         if x_splitit_test_mode is not None:
             _header_params["X-Splitit-TestMode"] = x_splitit_test_mode
         if x_splitit_idempotency_key is not None:
             _header_params["X-Splitit-IdempotencyKey"] = x_splitit_idempotency_key
@@ -602,14 +607,15 @@
         x_splitit_touch_point: str,
         attempt3d_secure: typing.Optional[bool] = None,
         shopper: typing.Optional[ShopperData] = None,
         plan_data: typing.Optional[PlanDataModel] = None,
         billing_address: typing.Optional[AddressDataModel] = None,
         payment_method: typing.Optional[PaymentMethodModel] = None,
         redirect_urls: typing.Optional[RedirectionEndpointsModel] = None,
+        processing_data: typing.Optional[ProcessingData] = None,
         events_endpoints: typing.Optional[EventsEndpointsModel] = None,
         x_splitit_test_mode: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
@@ -620,14 +626,15 @@
             x_splitit_touch_point=x_splitit_touch_point,
             attempt3d_secure=attempt3d_secure,
             shopper=shopper,
             plan_data=plan_data,
             billing_address=billing_address,
             payment_method=payment_method,
             redirect_urls=redirect_urls,
+            processing_data=processing_data,
             events_endpoints=events_endpoints,
             x_splitit_test_mode=x_splitit_test_mode,
         )
         return await self._apost2_oapg(
             body=args.body,
             header_params=args.header,
         )
@@ -640,14 +647,15 @@
         x_splitit_touch_point: str,
         attempt3d_secure: typing.Optional[bool] = None,
         shopper: typing.Optional[ShopperData] = None,
         plan_data: typing.Optional[PlanDataModel] = None,
         billing_address: typing.Optional[AddressDataModel] = None,
         payment_method: typing.Optional[PaymentMethodModel] = None,
         redirect_urls: typing.Optional[RedirectionEndpointsModel] = None,
+        processing_data: typing.Optional[ProcessingData] = None,
         events_endpoints: typing.Optional[EventsEndpointsModel] = None,
         x_splitit_test_mode: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post2_mapped_args(
@@ -657,14 +665,15 @@
             x_splitit_touch_point=x_splitit_touch_point,
             attempt3d_secure=attempt3d_secure,
             shopper=shopper,
             plan_data=plan_data,
             billing_address=billing_address,
             payment_method=payment_method,
             redirect_urls=redirect_urls,
+            processing_data=processing_data,
             events_endpoints=events_endpoints,
             x_splitit_test_mode=x_splitit_test_mode,
         )
         return self._post2_oapg(
             body=args.body,
             header_params=args.header,
         )
@@ -680,14 +689,15 @@
         x_splitit_touch_point: str,
         attempt3d_secure: typing.Optional[bool] = None,
         shopper: typing.Optional[ShopperData] = None,
         plan_data: typing.Optional[PlanDataModel] = None,
         billing_address: typing.Optional[AddressDataModel] = None,
         payment_method: typing.Optional[PaymentMethodModel] = None,
         redirect_urls: typing.Optional[RedirectionEndpointsModel] = None,
+        processing_data: typing.Optional[ProcessingData] = None,
         events_endpoints: typing.Optional[EventsEndpointsModel] = None,
         x_splitit_test_mode: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
@@ -698,14 +708,15 @@
             x_splitit_touch_point=x_splitit_touch_point,
             attempt3d_secure=attempt3d_secure,
             shopper=shopper,
             plan_data=plan_data,
             billing_address=billing_address,
             payment_method=payment_method,
             redirect_urls=redirect_urls,
+            processing_data=processing_data,
             events_endpoints=events_endpoints,
             x_splitit_test_mode=x_splitit_test_mode,
         )
         return await self._apost2_oapg(
             body=args.body,
             header_params=args.header,
         )
@@ -718,14 +729,15 @@
         x_splitit_touch_point: str,
         attempt3d_secure: typing.Optional[bool] = None,
         shopper: typing.Optional[ShopperData] = None,
         plan_data: typing.Optional[PlanDataModel] = None,
         billing_address: typing.Optional[AddressDataModel] = None,
         payment_method: typing.Optional[PaymentMethodModel] = None,
         redirect_urls: typing.Optional[RedirectionEndpointsModel] = None,
+        processing_data: typing.Optional[ProcessingData] = None,
         events_endpoints: typing.Optional[EventsEndpointsModel] = None,
         x_splitit_test_mode: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post2_mapped_args(
@@ -735,14 +747,15 @@
             x_splitit_touch_point=x_splitit_touch_point,
             attempt3d_secure=attempt3d_secure,
             shopper=shopper,
             plan_data=plan_data,
             billing_address=billing_address,
             payment_method=payment_method,
             redirect_urls=redirect_urls,
+            processing_data=processing_data,
             events_endpoints=events_endpoints,
             x_splitit_test_mode=x_splitit_test_mode,
         )
         return self._post2_oapg(
             body=args.body,
             header_params=args.header,
         )
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans/post.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans/post.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
+from splitit_client.model.processing_data import ProcessingData as ProcessingDataSchema
 from splitit_client.model.plan_error_response import PlanErrorResponse as PlanErrorResponseSchema
 from splitit_client.model.failed_response import FailedResponse as FailedResponseSchema
 from splitit_client.model.address_data_model import AddressDataModel as AddressDataModelSchema
 from splitit_client.model.installment_plan_create_response import InstallmentPlanCreateResponse as InstallmentPlanCreateResponseSchema
 from splitit_client.model.plan_data_model import PlanDataModel as PlanDataModelSchema
 from splitit_client.model.events_endpoints_model import EventsEndpointsModel as EventsEndpointsModelSchema
 from splitit_client.model.installment_plan_create_request import InstallmentPlanCreateRequest as InstallmentPlanCreateRequestSchema
@@ -42,14 +43,15 @@
 from splitit_client.model.redirection_endpoints_model import RedirectionEndpointsModel as RedirectionEndpointsModelSchema
 from splitit_client.model.shopper_data import ShopperData as ShopperDataSchema
 
 from splitit_client.type.failed_response import FailedResponse
 from splitit_client.type.address_data_model import AddressDataModel
 from splitit_client.type.plan_error_response import PlanErrorResponse
 from splitit_client.type.installment_plan_create_response import InstallmentPlanCreateResponse
+from splitit_client.type.processing_data import ProcessingData
 from splitit_client.type.installment_plan_create_request import InstallmentPlanCreateRequest
 from splitit_client.type.events_endpoints_model import EventsEndpointsModel
 from splitit_client.type.plan_data_model import PlanDataModel
 from splitit_client.type.shopper_data import ShopperData
 from splitit_client.type.payment_method_model import PaymentMethodModel
 from splitit_client.type.redirection_endpoints_model import RedirectionEndpointsModel
 
@@ -314,14 +316,15 @@
         x_splitit_touch_point: str,
         attempt3d_secure: typing.Optional[bool] = None,
         shopper: typing.Optional[ShopperData] = None,
         plan_data: typing.Optional[PlanDataModel] = None,
         billing_address: typing.Optional[AddressDataModel] = None,
         payment_method: typing.Optional[PaymentMethodModel] = None,
         redirect_urls: typing.Optional[RedirectionEndpointsModel] = None,
+        processing_data: typing.Optional[ProcessingData] = None,
         events_endpoints: typing.Optional[EventsEndpointsModel] = None,
         x_splitit_test_mode: typing.Optional[str] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _header_params = {}
         _body = {}
         if auto_capture is not None:
@@ -336,14 +339,16 @@
             _body["PlanData"] = plan_data
         if billing_address is not None:
             _body["BillingAddress"] = billing_address
         if payment_method is not None:
             _body["PaymentMethod"] = payment_method
         if redirect_urls is not None:
             _body["RedirectUrls"] = redirect_urls
+        if processing_data is not None:
+            _body["ProcessingData"] = processing_data
         if events_endpoints is not None:
             _body["EventsEndpoints"] = events_endpoints
         args.body = _body
         if x_splitit_test_mode is not None:
             _header_params["X-Splitit-TestMode"] = x_splitit_test_mode
         if x_splitit_idempotency_key is not None:
             _header_params["X-Splitit-IdempotencyKey"] = x_splitit_idempotency_key
@@ -580,14 +585,15 @@
         x_splitit_touch_point: str,
         attempt3d_secure: typing.Optional[bool] = None,
         shopper: typing.Optional[ShopperData] = None,
         plan_data: typing.Optional[PlanDataModel] = None,
         billing_address: typing.Optional[AddressDataModel] = None,
         payment_method: typing.Optional[PaymentMethodModel] = None,
         redirect_urls: typing.Optional[RedirectionEndpointsModel] = None,
+        processing_data: typing.Optional[ProcessingData] = None,
         events_endpoints: typing.Optional[EventsEndpointsModel] = None,
         x_splitit_test_mode: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
@@ -598,14 +604,15 @@
             x_splitit_touch_point=x_splitit_touch_point,
             attempt3d_secure=attempt3d_secure,
             shopper=shopper,
             plan_data=plan_data,
             billing_address=billing_address,
             payment_method=payment_method,
             redirect_urls=redirect_urls,
+            processing_data=processing_data,
             events_endpoints=events_endpoints,
             x_splitit_test_mode=x_splitit_test_mode,
         )
         return await self._apost2_oapg(
             body=args.body,
             header_params=args.header,
         )
@@ -618,14 +625,15 @@
         x_splitit_touch_point: str,
         attempt3d_secure: typing.Optional[bool] = None,
         shopper: typing.Optional[ShopperData] = None,
         plan_data: typing.Optional[PlanDataModel] = None,
         billing_address: typing.Optional[AddressDataModel] = None,
         payment_method: typing.Optional[PaymentMethodModel] = None,
         redirect_urls: typing.Optional[RedirectionEndpointsModel] = None,
+        processing_data: typing.Optional[ProcessingData] = None,
         events_endpoints: typing.Optional[EventsEndpointsModel] = None,
         x_splitit_test_mode: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post2_mapped_args(
@@ -635,14 +643,15 @@
             x_splitit_touch_point=x_splitit_touch_point,
             attempt3d_secure=attempt3d_secure,
             shopper=shopper,
             plan_data=plan_data,
             billing_address=billing_address,
             payment_method=payment_method,
             redirect_urls=redirect_urls,
+            processing_data=processing_data,
             events_endpoints=events_endpoints,
             x_splitit_test_mode=x_splitit_test_mode,
         )
         return self._post2_oapg(
             body=args.body,
             header_params=args.header,
         )
@@ -658,14 +667,15 @@
         x_splitit_touch_point: str,
         attempt3d_secure: typing.Optional[bool] = None,
         shopper: typing.Optional[ShopperData] = None,
         plan_data: typing.Optional[PlanDataModel] = None,
         billing_address: typing.Optional[AddressDataModel] = None,
         payment_method: typing.Optional[PaymentMethodModel] = None,
         redirect_urls: typing.Optional[RedirectionEndpointsModel] = None,
+        processing_data: typing.Optional[ProcessingData] = None,
         events_endpoints: typing.Optional[EventsEndpointsModel] = None,
         x_splitit_test_mode: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
@@ -676,14 +686,15 @@
             x_splitit_touch_point=x_splitit_touch_point,
             attempt3d_secure=attempt3d_secure,
             shopper=shopper,
             plan_data=plan_data,
             billing_address=billing_address,
             payment_method=payment_method,
             redirect_urls=redirect_urls,
+            processing_data=processing_data,
             events_endpoints=events_endpoints,
             x_splitit_test_mode=x_splitit_test_mode,
         )
         return await self._apost2_oapg(
             body=args.body,
             header_params=args.header,
         )
@@ -696,14 +707,15 @@
         x_splitit_touch_point: str,
         attempt3d_secure: typing.Optional[bool] = None,
         shopper: typing.Optional[ShopperData] = None,
         plan_data: typing.Optional[PlanDataModel] = None,
         billing_address: typing.Optional[AddressDataModel] = None,
         payment_method: typing.Optional[PaymentMethodModel] = None,
         redirect_urls: typing.Optional[RedirectionEndpointsModel] = None,
+        processing_data: typing.Optional[ProcessingData] = None,
         events_endpoints: typing.Optional[EventsEndpointsModel] = None,
         x_splitit_test_mode: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post2_mapped_args(
@@ -713,14 +725,15 @@
             x_splitit_touch_point=x_splitit_touch_point,
             attempt3d_secure=attempt3d_secure,
             shopper=shopper,
             plan_data=plan_data,
             billing_address=billing_address,
             payment_method=payment_method,
             redirect_urls=redirect_urls,
+            processing_data=processing_data,
             events_endpoints=events_endpoints,
             x_splitit_test_mode=x_splitit_test_mode,
         )
         return self._post2_oapg(
             body=args.body,
             header_params=args.header,
         )
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_check_eligibility/post.py` & `splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_check_eligibility/post.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_check_eligibility/post.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_check_eligibility/post.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_initiate/post.py` & `splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_initiate/post.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 from splitit_client.model.installment_plan_initiate_request import InstallmentPlanInitiateRequest as InstallmentPlanInitiateRequestSchema
+from splitit_client.model.processing_data import ProcessingData as ProcessingDataSchema
 from splitit_client.model.plan_error_response import PlanErrorResponse as PlanErrorResponseSchema
 from splitit_client.model.failed_response import FailedResponse as FailedResponseSchema
 from splitit_client.model.initiate_redirection_endpoints_model import InitiateRedirectionEndpointsModel as InitiateRedirectionEndpointsModelSchema
 from splitit_client.model.address_data_model import AddressDataModel as AddressDataModelSchema
 from splitit_client.model.plan_data_model import PlanDataModel as PlanDataModelSchema
 from splitit_client.model.events_endpoints_model import EventsEndpointsModel as EventsEndpointsModelSchema
 from splitit_client.model.ux_settings_model import UxSettingsModel as UxSettingsModelSchema
@@ -43,14 +44,15 @@
 from splitit_client.model.shopper_data import ShopperData as ShopperDataSchema
 
 from splitit_client.type.failed_response import FailedResponse
 from splitit_client.type.initiate_redirection_endpoints_model import InitiateRedirectionEndpointsModel
 from splitit_client.type.address_data_model import AddressDataModel
 from splitit_client.type.installment_plan_initiate_request import InstallmentPlanInitiateRequest
 from splitit_client.type.plan_error_response import PlanErrorResponse
+from splitit_client.type.processing_data import ProcessingData
 from splitit_client.type.events_endpoints_model import EventsEndpointsModel
 from splitit_client.type.initiate_plan_response import InitiatePlanResponse
 from splitit_client.type.plan_data_model import PlanDataModel
 from splitit_client.type.ux_settings_model import UxSettingsModel
 from splitit_client.type.shopper_data import ShopperData
 
 from . import path
@@ -336,14 +338,15 @@
         attempt3d_secure: typing.Optional[bool] = None,
         shopper: typing.Optional[ShopperData] = None,
         plan_data: typing.Optional[PlanDataModel] = None,
         billing_address: typing.Optional[AddressDataModel] = None,
         redirect_urls: typing.Optional[InitiateRedirectionEndpointsModel] = None,
         ux_settings: typing.Optional[UxSettingsModel] = None,
         events_endpoints: typing.Optional[EventsEndpointsModel] = None,
+        processing_data: typing.Optional[ProcessingData] = None,
         x_splitit_test_mode: typing.Optional[str] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _header_params = {}
         _body = {}
         if auto_capture is not None:
             _body["AutoCapture"] = auto_capture
@@ -357,14 +360,16 @@
             _body["BillingAddress"] = billing_address
         if redirect_urls is not None:
             _body["RedirectUrls"] = redirect_urls
         if ux_settings is not None:
             _body["UxSettings"] = ux_settings
         if events_endpoints is not None:
             _body["EventsEndpoints"] = events_endpoints
+        if processing_data is not None:
+            _body["ProcessingData"] = processing_data
         args.body = _body
         if x_splitit_test_mode is not None:
             _header_params["X-Splitit-TestMode"] = x_splitit_test_mode
         if x_splitit_idempotency_key is not None:
             _header_params["X-Splitit-IdempotencyKey"] = x_splitit_idempotency_key
         if x_splitit_touch_point is not None:
             _header_params["X-Splitit-TouchPoint"] = x_splitit_touch_point
@@ -599,14 +604,15 @@
         attempt3d_secure: typing.Optional[bool] = None,
         shopper: typing.Optional[ShopperData] = None,
         plan_data: typing.Optional[PlanDataModel] = None,
         billing_address: typing.Optional[AddressDataModel] = None,
         redirect_urls: typing.Optional[InitiateRedirectionEndpointsModel] = None,
         ux_settings: typing.Optional[UxSettingsModel] = None,
         events_endpoints: typing.Optional[EventsEndpointsModel] = None,
+        processing_data: typing.Optional[ProcessingData] = None,
         x_splitit_test_mode: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
@@ -616,14 +622,15 @@
             attempt3d_secure=attempt3d_secure,
             shopper=shopper,
             plan_data=plan_data,
             billing_address=billing_address,
             redirect_urls=redirect_urls,
             ux_settings=ux_settings,
             events_endpoints=events_endpoints,
+            processing_data=processing_data,
             x_splitit_test_mode=x_splitit_test_mode,
         )
         return await self._apost_oapg(
             body=args.body,
             header_params=args.header,
         )
     
@@ -635,14 +642,15 @@
         attempt3d_secure: typing.Optional[bool] = None,
         shopper: typing.Optional[ShopperData] = None,
         plan_data: typing.Optional[PlanDataModel] = None,
         billing_address: typing.Optional[AddressDataModel] = None,
         redirect_urls: typing.Optional[InitiateRedirectionEndpointsModel] = None,
         ux_settings: typing.Optional[UxSettingsModel] = None,
         events_endpoints: typing.Optional[EventsEndpointsModel] = None,
+        processing_data: typing.Optional[ProcessingData] = None,
         x_splitit_test_mode: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
             auto_capture=auto_capture,
@@ -651,14 +659,15 @@
             attempt3d_secure=attempt3d_secure,
             shopper=shopper,
             plan_data=plan_data,
             billing_address=billing_address,
             redirect_urls=redirect_urls,
             ux_settings=ux_settings,
             events_endpoints=events_endpoints,
+            processing_data=processing_data,
             x_splitit_test_mode=x_splitit_test_mode,
         )
         return self._post_oapg(
             body=args.body,
             header_params=args.header,
         )
 
@@ -673,14 +682,15 @@
         attempt3d_secure: typing.Optional[bool] = None,
         shopper: typing.Optional[ShopperData] = None,
         plan_data: typing.Optional[PlanDataModel] = None,
         billing_address: typing.Optional[AddressDataModel] = None,
         redirect_urls: typing.Optional[InitiateRedirectionEndpointsModel] = None,
         ux_settings: typing.Optional[UxSettingsModel] = None,
         events_endpoints: typing.Optional[EventsEndpointsModel] = None,
+        processing_data: typing.Optional[ProcessingData] = None,
         x_splitit_test_mode: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
@@ -690,14 +700,15 @@
             attempt3d_secure=attempt3d_secure,
             shopper=shopper,
             plan_data=plan_data,
             billing_address=billing_address,
             redirect_urls=redirect_urls,
             ux_settings=ux_settings,
             events_endpoints=events_endpoints,
+            processing_data=processing_data,
             x_splitit_test_mode=x_splitit_test_mode,
         )
         return await self._apost_oapg(
             body=args.body,
             header_params=args.header,
         )
     
@@ -709,14 +720,15 @@
         attempt3d_secure: typing.Optional[bool] = None,
         shopper: typing.Optional[ShopperData] = None,
         plan_data: typing.Optional[PlanDataModel] = None,
         billing_address: typing.Optional[AddressDataModel] = None,
         redirect_urls: typing.Optional[InitiateRedirectionEndpointsModel] = None,
         ux_settings: typing.Optional[UxSettingsModel] = None,
         events_endpoints: typing.Optional[EventsEndpointsModel] = None,
+        processing_data: typing.Optional[ProcessingData] = None,
         x_splitit_test_mode: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
             auto_capture=auto_capture,
@@ -725,14 +737,15 @@
             attempt3d_secure=attempt3d_secure,
             shopper=shopper,
             plan_data=plan_data,
             billing_address=billing_address,
             redirect_urls=redirect_urls,
             ux_settings=ux_settings,
             events_endpoints=events_endpoints,
+            processing_data=processing_data,
             x_splitit_test_mode=x_splitit_test_mode,
         )
         return self._post_oapg(
             body=args.body,
             header_params=args.header,
         )
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_initiate/post.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_initiate/post.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
 from splitit_client.model.installment_plan_initiate_request import InstallmentPlanInitiateRequest as InstallmentPlanInitiateRequestSchema
+from splitit_client.model.processing_data import ProcessingData as ProcessingDataSchema
 from splitit_client.model.plan_error_response import PlanErrorResponse as PlanErrorResponseSchema
 from splitit_client.model.failed_response import FailedResponse as FailedResponseSchema
 from splitit_client.model.initiate_redirection_endpoints_model import InitiateRedirectionEndpointsModel as InitiateRedirectionEndpointsModelSchema
 from splitit_client.model.address_data_model import AddressDataModel as AddressDataModelSchema
 from splitit_client.model.plan_data_model import PlanDataModel as PlanDataModelSchema
 from splitit_client.model.events_endpoints_model import EventsEndpointsModel as EventsEndpointsModelSchema
 from splitit_client.model.ux_settings_model import UxSettingsModel as UxSettingsModelSchema
@@ -43,14 +44,15 @@
 from splitit_client.model.shopper_data import ShopperData as ShopperDataSchema
 
 from splitit_client.type.failed_response import FailedResponse
 from splitit_client.type.initiate_redirection_endpoints_model import InitiateRedirectionEndpointsModel
 from splitit_client.type.address_data_model import AddressDataModel
 from splitit_client.type.installment_plan_initiate_request import InstallmentPlanInitiateRequest
 from splitit_client.type.plan_error_response import PlanErrorResponse
+from splitit_client.type.processing_data import ProcessingData
 from splitit_client.type.events_endpoints_model import EventsEndpointsModel
 from splitit_client.type.initiate_plan_response import InitiatePlanResponse
 from splitit_client.type.plan_data_model import PlanDataModel
 from splitit_client.type.ux_settings_model import UxSettingsModel
 from splitit_client.type.shopper_data import ShopperData
 
 # Header params
@@ -314,14 +316,15 @@
         attempt3d_secure: typing.Optional[bool] = None,
         shopper: typing.Optional[ShopperData] = None,
         plan_data: typing.Optional[PlanDataModel] = None,
         billing_address: typing.Optional[AddressDataModel] = None,
         redirect_urls: typing.Optional[InitiateRedirectionEndpointsModel] = None,
         ux_settings: typing.Optional[UxSettingsModel] = None,
         events_endpoints: typing.Optional[EventsEndpointsModel] = None,
+        processing_data: typing.Optional[ProcessingData] = None,
         x_splitit_test_mode: typing.Optional[str] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _header_params = {}
         _body = {}
         if auto_capture is not None:
             _body["AutoCapture"] = auto_capture
@@ -335,14 +338,16 @@
             _body["BillingAddress"] = billing_address
         if redirect_urls is not None:
             _body["RedirectUrls"] = redirect_urls
         if ux_settings is not None:
             _body["UxSettings"] = ux_settings
         if events_endpoints is not None:
             _body["EventsEndpoints"] = events_endpoints
+        if processing_data is not None:
+            _body["ProcessingData"] = processing_data
         args.body = _body
         if x_splitit_test_mode is not None:
             _header_params["X-Splitit-TestMode"] = x_splitit_test_mode
         if x_splitit_idempotency_key is not None:
             _header_params["X-Splitit-IdempotencyKey"] = x_splitit_idempotency_key
         if x_splitit_touch_point is not None:
             _header_params["X-Splitit-TouchPoint"] = x_splitit_touch_point
@@ -577,14 +582,15 @@
         attempt3d_secure: typing.Optional[bool] = None,
         shopper: typing.Optional[ShopperData] = None,
         plan_data: typing.Optional[PlanDataModel] = None,
         billing_address: typing.Optional[AddressDataModel] = None,
         redirect_urls: typing.Optional[InitiateRedirectionEndpointsModel] = None,
         ux_settings: typing.Optional[UxSettingsModel] = None,
         events_endpoints: typing.Optional[EventsEndpointsModel] = None,
+        processing_data: typing.Optional[ProcessingData] = None,
         x_splitit_test_mode: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
@@ -594,14 +600,15 @@
             attempt3d_secure=attempt3d_secure,
             shopper=shopper,
             plan_data=plan_data,
             billing_address=billing_address,
             redirect_urls=redirect_urls,
             ux_settings=ux_settings,
             events_endpoints=events_endpoints,
+            processing_data=processing_data,
             x_splitit_test_mode=x_splitit_test_mode,
         )
         return await self._apost_oapg(
             body=args.body,
             header_params=args.header,
         )
     
@@ -613,14 +620,15 @@
         attempt3d_secure: typing.Optional[bool] = None,
         shopper: typing.Optional[ShopperData] = None,
         plan_data: typing.Optional[PlanDataModel] = None,
         billing_address: typing.Optional[AddressDataModel] = None,
         redirect_urls: typing.Optional[InitiateRedirectionEndpointsModel] = None,
         ux_settings: typing.Optional[UxSettingsModel] = None,
         events_endpoints: typing.Optional[EventsEndpointsModel] = None,
+        processing_data: typing.Optional[ProcessingData] = None,
         x_splitit_test_mode: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
             auto_capture=auto_capture,
@@ -629,14 +637,15 @@
             attempt3d_secure=attempt3d_secure,
             shopper=shopper,
             plan_data=plan_data,
             billing_address=billing_address,
             redirect_urls=redirect_urls,
             ux_settings=ux_settings,
             events_endpoints=events_endpoints,
+            processing_data=processing_data,
             x_splitit_test_mode=x_splitit_test_mode,
         )
         return self._post_oapg(
             body=args.body,
             header_params=args.header,
         )
 
@@ -651,14 +660,15 @@
         attempt3d_secure: typing.Optional[bool] = None,
         shopper: typing.Optional[ShopperData] = None,
         plan_data: typing.Optional[PlanDataModel] = None,
         billing_address: typing.Optional[AddressDataModel] = None,
         redirect_urls: typing.Optional[InitiateRedirectionEndpointsModel] = None,
         ux_settings: typing.Optional[UxSettingsModel] = None,
         events_endpoints: typing.Optional[EventsEndpointsModel] = None,
+        processing_data: typing.Optional[ProcessingData] = None,
         x_splitit_test_mode: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
@@ -668,14 +678,15 @@
             attempt3d_secure=attempt3d_secure,
             shopper=shopper,
             plan_data=plan_data,
             billing_address=billing_address,
             redirect_urls=redirect_urls,
             ux_settings=ux_settings,
             events_endpoints=events_endpoints,
+            processing_data=processing_data,
             x_splitit_test_mode=x_splitit_test_mode,
         )
         return await self._apost_oapg(
             body=args.body,
             header_params=args.header,
         )
     
@@ -687,14 +698,15 @@
         attempt3d_secure: typing.Optional[bool] = None,
         shopper: typing.Optional[ShopperData] = None,
         plan_data: typing.Optional[PlanDataModel] = None,
         billing_address: typing.Optional[AddressDataModel] = None,
         redirect_urls: typing.Optional[InitiateRedirectionEndpointsModel] = None,
         ux_settings: typing.Optional[UxSettingsModel] = None,
         events_endpoints: typing.Optional[EventsEndpointsModel] = None,
+        processing_data: typing.Optional[ProcessingData] = None,
         x_splitit_test_mode: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
             auto_capture=auto_capture,
@@ -703,14 +715,15 @@
             attempt3d_secure=attempt3d_secure,
             shopper=shopper,
             plan_data=plan_data,
             billing_address=billing_address,
             redirect_urls=redirect_urls,
             ux_settings=ux_settings,
             events_endpoints=events_endpoints,
+            processing_data=processing_data,
             x_splitit_test_mode=x_splitit_test_mode,
         )
         return self._post_oapg(
             body=args.body,
             header_params=args.header,
         )
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.py` & `splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.py` & `splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.py` & `splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.py` & `splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.py` & `splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_search/get.py` & `splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_search/get.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_search/get.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_search/get.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_updateorder/put.py` & `splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_updateorder/put.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/paths/api_installmentplans_updateorder/put.pyi` & `splitit_web_python_sdk-2.5.0/splitit_client/paths/api_installmentplans_updateorder/put.pyi`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/request_after_hook.py` & `splitit_web_python_sdk-2.5.0/splitit_client/request_after_hook.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/request_before_hook.py` & `splitit_web_python_sdk-2.5.0/splitit_client/request_before_hook.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/rest.py` & `splitit_web_python_sdk-2.5.0/splitit_client/rest.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/schemas.py` & `splitit_web_python_sdk-2.5.0/splitit_client/schemas.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/address_data.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/address_data.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/address_data_model.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/address_data_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/authorization_model.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/authorization_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,9 +33,11 @@
 
     ThreeDSRedirect: ThreeDsRedirectDataV3
 
     CAVV: str
 
     ECI: str
 
+    GatewaySourceResponse: str
+
 class AuthorizationModel(RequiredAuthorizationModel, OptionalAuthorizationModel):
     pass
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/card_data.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/card_data.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/check_installments_eligibility_request.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/check_installments_eligibility_request.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/events_endpoints_model.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/events_endpoints_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/failed_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/failed_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/identifier_contract.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/identifier_contract.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/initiate_plan_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/initiate_plan_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/initiate_redirection_endpoints_model.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/initiate_redirection_endpoints_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/installment.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/installment.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_cancel_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_cancel_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_create_request.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_create_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from splitit_client.type.address_data_model import AddressDataModel
 from splitit_client.type.events_endpoints_model import EventsEndpointsModel
 from splitit_client.type.payment_method_model import PaymentMethodModel
 from splitit_client.type.plan_data_model import PlanDataModel
+from splitit_client.type.processing_data import ProcessingData
 from splitit_client.type.redirection_endpoints_model import RedirectionEndpointsModel
 from splitit_client.type.shopper_data import ShopperData
 
 class RequiredInstallmentPlanCreateRequest(TypedDict):
     AutoCapture: bool
 
     TermsAndConditionsAccepted: bool
@@ -35,11 +36,13 @@
 
     BillingAddress: AddressDataModel
 
     PaymentMethod: PaymentMethodModel
 
     RedirectUrls: RedirectionEndpointsModel
 
+    ProcessingData: ProcessingData
+
     EventsEndpoints: EventsEndpointsModel
 
 class InstallmentPlanCreateRequest(RequiredInstallmentPlanCreateRequest, OptionalInstallmentPlanCreateRequest):
     pass
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_create_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_create_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_get_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_get_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_initiate_request.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_initiate_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from splitit_client.type.address_data_model import AddressDataModel
 from splitit_client.type.events_endpoints_model import EventsEndpointsModel
 from splitit_client.type.initiate_redirection_endpoints_model import InitiateRedirectionEndpointsModel
 from splitit_client.type.plan_data_model import PlanDataModel
+from splitit_client.type.processing_data import ProcessingData
 from splitit_client.type.shopper_data import ShopperData
 from splitit_client.type.ux_settings_model import UxSettingsModel
 
 class RequiredInstallmentPlanInitiateRequest(TypedDict):
     AutoCapture: bool
 
 class OptionalInstallmentPlanInitiateRequest(TypedDict, total=False):
@@ -35,9 +36,11 @@
 
     RedirectUrls: InitiateRedirectionEndpointsModel
 
     UxSettings: UxSettingsModel
 
     EventsEndpoints: EventsEndpointsModel
 
+    ProcessingData: ProcessingData
+
 class InstallmentPlanInitiateRequest(RequiredInstallmentPlanInitiateRequest, OptionalInstallmentPlanInitiateRequest):
     pass
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_refund_request.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_refund_request.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_refund_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_refund_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_search_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_search_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_update_request.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_update_request.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_update_request_by_identifier.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_update_request_by_identifier.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/installment_plan_update_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/installment_plan_update_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/installments_eligibility_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/installments_eligibility_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/links_data.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/links_data.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/links_model.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/links_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/payment_method_model.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/payment_method_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,20 +10,26 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
+from splitit_client.type.bluesnap_vaulted_shopper_token import BluesnapVaultedShopperToken
 from splitit_client.type.card_data import CardData
+from splitit_client.type.mocker_shopper_token import MockerShopperToken
 from splitit_client.type.payment_method_type import PaymentMethodType
 
 class RequiredPaymentMethodModel(TypedDict):
     Type: PaymentMethodType
 
 class OptionalPaymentMethodModel(TypedDict, total=False):
     Card: CardData
 
     Token: str
 
+    BluesnapVaultedShopperToken: BluesnapVaultedShopperToken
+
+    MockerShopperToken: MockerShopperToken
+
 class PaymentMethodModel(RequiredPaymentMethodModel, OptionalPaymentMethodModel):
     pass
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/payment_plan_option_model.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/payment_plan_option_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/plan_data.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/plan_data_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,31 +12,29 @@
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from splitit_client.type.purchase_method import PurchaseMethod
 
-class RequiredPlanData(TypedDict):
+class RequiredPlanDataModel(TypedDict):
     TotalAmount: typing.Union[int, float]
 
-    NumberOfInstallments: int
-
     PurchaseMethod: PurchaseMethod
 
-class OptionalPlanData(TypedDict, total=False):
-    TerminalId: str
+class OptionalPlanDataModel(TypedDict, total=False):
+    Currency: str
 
-    FirstInstallmentAmount: typing.Union[int, float]
+    NumberOfInstallments: int
 
-    Currency: str
+    TerminalId: str
 
     RefOrderNumber: str
 
-    AllowedInstallmentOptions: typing.List[int]
+    ExtendedParams: typing.Dict[str, str]
 
-    Tags: typing.Dict[str, str]
+    FirstInstallmentAmount: typing.Union[int, float]
 
     FirstInstallmentDate: datetime
 
-class PlanData(RequiredPlanData, OptionalPlanData):
+class PlanDataModel(RequiredPlanDataModel, OptionalPlanDataModel):
     pass
```

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/redirection_endpoints_model.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/redirection_endpoints_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/refund_model.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/refund_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/refund_summary.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/refund_summary.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/search_installment_plan_response_item.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/search_installment_plan_response_item.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/shopper_data.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/shopper_data.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/three_ds_redirect_data_v3.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/three_ds_redirect_data_v3.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/update_order_request.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/update_order_request.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/ux_settings_model.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/ux_settings_model.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/type/verify_authorization_response.py` & `splitit_web_python_sdk-2.5.0/splitit_client/type/verify_authorization_response.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/splitit_client/validation_metadata.py` & `splitit_web_python_sdk-2.5.0/splitit_client/validation_metadata.py`

 * *Files identical despite different names*

### Comparing `splitit_web_python_sdk-2.4.0/PKG-INFO` & `splitit_web_python_sdk-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splitit-web-python-sdk
-Version: 2.4.0
+Version: 2.5.0
 Summary: Client for splitit-web-api-v3
 License: MIT
 Author: Konfig
 Author-email: engineering@konfigthis.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,26 +18,26 @@
 Requires-Dist: frozendict (>=2.3.4,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: typing_extensions (>=4.3.0,<5.0.0)
 Requires-Dist: urllib3 (>=1.26.7,<2.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
 
-# splitit-web-python-sdk@2.4.0
+# splitit-web-python-sdk@2.5.0
 Splitit's Web API
 
 
 ## Requirements
 
 Python >=3.7
 
 ## Installing
 
 ```sh
-pip install splitit-web-python-sdk==2.4.0
+pip install splitit-web-python-sdk==2.5.0
 ```
 
 ## Getting Started
 
 ```python
 from pprint import pprint
 from splitit_client import Splitit, ApiException
@@ -155,22 +155,24 @@
 *InstallmentPlanApi* | [**verify_authorization**](docs/apis/tags/InstallmentPlanApi.md#verify_authorization) | **get** /api/installmentplans/{installmentPlanNumber}/verifyauthorization | 
 
 ## Documentation For Models
 
  - [AddressData](docs/models/AddressData.md)
  - [AddressDataModel](docs/models/AddressDataModel.md)
  - [AuthorizationModel](docs/models/AuthorizationModel.md)
+ - [BluesnapVaultedShopperToken](docs/models/BluesnapVaultedShopperToken.md)
  - [CardBrand](docs/models/CardBrand.md)
  - [CardData](docs/models/CardData.md)
  - [CardType](docs/models/CardType.md)
  - [CheckInstallmentsEligibilityRequest](docs/models/CheckInstallmentsEligibilityRequest.md)
  - [Error](docs/models/Error.md)
  - [ErrorExtended](docs/models/ErrorExtended.md)
  - [EventsEndpointsModel](docs/models/EventsEndpointsModel.md)
  - [FailedResponse](docs/models/FailedResponse.md)
+ - [GatewayTokenData](docs/models/GatewayTokenData.md)
  - [GwAuthorizationStatus](docs/models/GwAuthorizationStatus.md)
  - [IdentifierContract](docs/models/IdentifierContract.md)
  - [InitiatePlanResponse](docs/models/InitiatePlanResponse.md)
  - [InitiateRedirectionEndpointsModel](docs/models/InitiateRedirectionEndpointsModel.md)
  - [Installment](docs/models/Installment.md)
  - [InstallmentPlanCancelResponse](docs/models/InstallmentPlanCancelResponse.md)
  - [InstallmentPlanCreateRequest](docs/models/InstallmentPlanCreateRequest.md)
@@ -183,32 +185,37 @@
  - [InstallmentPlanUpdateRequest](docs/models/InstallmentPlanUpdateRequest.md)
  - [InstallmentPlanUpdateRequestByIdentifier](docs/models/InstallmentPlanUpdateRequestByIdentifier.md)
  - [InstallmentPlanUpdateResponse](docs/models/InstallmentPlanUpdateResponse.md)
  - [InstallmentStatus](docs/models/InstallmentStatus.md)
  - [InstallmentsEligibilityResponse](docs/models/InstallmentsEligibilityResponse.md)
  - [LinksData](docs/models/LinksData.md)
  - [LinksModel](docs/models/LinksModel.md)
+ - [MockerShopperToken](docs/models/MockerShopperToken.md)
  - [PaymentMethodModel](docs/models/PaymentMethodModel.md)
  - [PaymentMethodType](docs/models/PaymentMethodType.md)
  - [PaymentPlanOptionModel](docs/models/PaymentPlanOptionModel.md)
  - [PlanData](docs/models/PlanData.md)
  - [PlanDataModel](docs/models/PlanDataModel.md)
  - [PlanErrorResponse](docs/models/PlanErrorResponse.md)
  - [PlanStatus](docs/models/PlanStatus.md)
+ - [ProcessingData](docs/models/ProcessingData.md)
+ - [ProcessingData2](docs/models/ProcessingData2.md)
  - [PurchaseMethod](docs/models/PurchaseMethod.md)
  - [RedirectionEndpointsModel](docs/models/RedirectionEndpointsModel.md)
  - [RefundModel](docs/models/RefundModel.md)
  - [RefundStatus](docs/models/RefundStatus.md)
  - [RefundStrategy](docs/models/RefundStrategy.md)
  - [RefundSummary](docs/models/RefundSummary.md)
  - [SearchInstallmentPlanResponseItem](docs/models/SearchInstallmentPlanResponseItem.md)
  - [ShippingStatus](docs/models/ShippingStatus.md)
  - [ShippingStatus2](docs/models/ShippingStatus2.md)
  - [ShopperData](docs/models/ShopperData.md)
  - [TestModes](docs/models/TestModes.md)
+ - [ThreeDSData](docs/models/ThreeDSData.md)
+ - [ThreeDSData2](docs/models/ThreeDSData2.md)
  - [ThreeDsRedirectDataV3](docs/models/ThreeDsRedirectDataV3.md)
  - [UpdateOrderRequest](docs/models/UpdateOrderRequest.md)
  - [UxSettingsModel](docs/models/UxSettingsModel.md)
  - [VerifyAuthorizationResponse](docs/models/VerifyAuthorizationResponse.md)
 
 
 ## Author
```

