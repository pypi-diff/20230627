# Comparing `tmp/equinix-metal-0.2.1.tar.gz` & `tmp/equinix-metal-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equinix-metal-0.2.1.tar", last modified: Fri Jun  9 09:19:47 2023, max compression
+gzip compressed data, was "equinix-metal-0.2.2.tar", last modified: Tue Jun 27 14:37:21 2023, max compression
```

## Comparing `equinix-metal-0.2.1.tar` & `equinix-metal-0.2.2.tar`

### file list

```diff
@@ -1,555 +1,563 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:47.644604 equinix-metal-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-09 09:19:47.644604 equinix-metal-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    51411 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:47.560603 equinix-metal-0.2.1/equinix_metal/
--rw-r--r--   0 runner    (1001) docker     (123)    24048 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:47.568603 equinix-metal-0.2.1/equinix_metal/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46223 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/authentication_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    35443 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/batches_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53275 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/bgp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    42522 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/capacity_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   139461 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/devices_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    32320 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/emails_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    79719 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30060 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/facilities_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    40324 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/hardware_reservations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/incidents_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   110259 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/interconnections_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/invitations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    58088 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/ip_addresses_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    42404 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/licenses_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26100 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    42371 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/metal_gateways_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16543 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/metros_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/operating_systems_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   126100 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/organizations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27611 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/otps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16686 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/password_reset_tokens_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26446 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/payment_methods_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21858 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/plans_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   109267 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/ports_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    88544 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/projects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26659 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/self_service_reservations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    57754 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/spot_market_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    65523 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/ssh_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/support_request_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25177 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/transfer_requests_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26624 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/two_factor_auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19788 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/usages_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17508 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/user_verification_tokens_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/userdata_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    58053 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    34054 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/vlans_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    99745 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api/vrfs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33612 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19317 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:47.600604 equinix-metal-0.2.1/equinix_metal/models/
--rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/activate_hardware_reservation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/auth_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/auth_token_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/auth_token_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/auth_token_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/auth_token_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/batches_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/bgp_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/bgp_config_request_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/bgp_dynamic_neighbor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/bgp_dynamic_neighbor_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/bgp_dynamic_neighbor_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/bgp_neighbor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/bgp_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/bgp_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/bgp_session_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/bgp_session_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/bgp_session_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/bond_port_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/capacity_check_per_facility_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/capacity_check_per_facility_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/capacity_check_per_metro_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/capacity_check_per_metro_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/capacity_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/capacity_level_per_baremetal.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/capacity_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/capacity_per_facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/capacity_per_metro_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/capacity_per_new_facility.py
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/capacity_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/create_device_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/create_email_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/create_metal_gateway_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/create_self_service_reservation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/create_self_service_reservation_request_period.py
--rw-r--r--   0 runner    (1001) docker     (123)    17473 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/device_action_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/device_actions_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/device_create_in_facility_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    16619 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/device_create_in_metro_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    16358 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/device_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/device_created_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/device_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/device_metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/device_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/device_project_lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/device_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/device_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/device_usage_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/email_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/entitlement.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/event_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/fabric_service_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/facility_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/facility_input_facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/facility_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/find_ip_address_by_id200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/find_metal_gateway_by_id200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/find_traffic_timeframe_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/global_bgp_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/global_bgp_range_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/hardware_reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/hardware_reservation_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/href.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/instances_batch_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    17728 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/instances_batch_create_input_batches_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/instances_batch_create_input_batches_inner_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/interconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/interconnection_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/interconnection_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/interconnection_metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/interconnection_port.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/interconnection_port_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/interconnection_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/invitation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/invitation_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/invitation_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/ip_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/ip_assignment_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/ip_assignment_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/ip_assignment_metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/ip_assignment_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/ip_availabilities_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/ip_reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/ip_reservation_facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/ip_reservation_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/ip_reservation_list_ip_addresses_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/ip_reservation_metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/ip_reservation_request_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/license.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/license_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/license_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/license_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/membership.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/membership_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/membership_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/metadata_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/metadata_network_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/metadata_network_network_bonding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/metal_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/metal_gateway_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/metal_gateway_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/metal_gateway_list_metal_gateways_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/metal_gateway_lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/metro_capacity_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/metro_capacity_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/metro_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/metro_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/metro_server_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/move_hardware_reservation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/new_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/operating_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/operating_system_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/organization_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/organization_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/parent_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/payment_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/payment_method_billing_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/payment_method_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/payment_method_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/payment_method_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/plan_available_in_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/plan_available_in_inner_price.py
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/plan_available_in_metros_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/plan_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/plan_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/plan_specs_cpus_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/plan_specs_drives_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/plan_specs_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/plan_specs_nics_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/port.py
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/port_assign_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/port_convert_layer3_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/port_convert_layer3_input_request_ips_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/port_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/port_vlan_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/port_vlan_assignment_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/port_vlan_assignment_batch_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/port_vlan_assignment_batch_create_input_vlan_assignments_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/port_vlan_assignment_batch_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/port_vlan_assignment_batch_vlan_assignments_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/port_vlan_assignment_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/project_create_from_root_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/project_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/project_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/project_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/project_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/project_usage_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/recovery_code_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/request_ip_reservation201_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/request_ip_reservation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/self_service_reservation_item_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/self_service_reservation_item_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/self_service_reservation_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/self_service_reservation_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/server_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/spot_market_prices_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/spot_market_prices_per_metro_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/spot_market_prices_per_metro_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/spot_market_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/spot_market_request_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/spot_market_request_create_input_instance_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6747 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/spot_market_request_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/spot_market_request_metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/spot_prices_datapoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/spot_prices_history_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/spot_prices_per_baremetal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/spot_prices_per_facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/spot_prices_per_new_facility.py
--rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/spot_prices_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/ssh_key_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/ssh_key_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/ssh_key_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/support_request_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/transfer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/transfer_request_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/transfer_request_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/update_email_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/user_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/user_limited.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/user_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/user_lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/user_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/userdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/verify_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/virtual_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/virtual_circuit_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/virtual_circuit_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/virtual_circuit_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/virtual_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/virtual_network_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/virtual_network_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    10895 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/vlan_virtual_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/vlan_virtual_circuit_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/vlan_virtual_circuit_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/vrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/vrf_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/vrf_ip_reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/vrf_ip_reservation_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/vrf_ip_reservation_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/vrf_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/vrf_metal_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/vrf_metal_gateway_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/vrf_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/vrf_route_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/vrf_route_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/vrf_route_metal_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/vrf_route_virtual_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/vrf_route_vrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/vrf_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/vrf_virtual_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/vrf_virtual_circuit_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/models/vrf_virtual_circuit_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/equinix_metal/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:47.560603 equinix-metal-0.2.1/equinix_metal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-09 09:19:47.000000 equinix-metal-0.2.1/equinix_metal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21108 2023-06-09 09:19:47.000000 equinix-metal-0.2.1/equinix_metal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:19:47.000000 equinix-metal-0.2.1/equinix_metal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 09:19:47.000000 equinix-metal-0.2.1/equinix_metal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-09 09:19:47.000000 equinix-metal-0.2.1/equinix_metal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-09 09:19:47.648604 equinix-metal-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:47.644604 equinix-metal-0.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_activate_hardware_reservation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_auth_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_auth_token_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_auth_token_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_auth_token_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_auth_token_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_authentication_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_batches_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_batches_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_bgp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_bgp_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_bgp_config_request_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_bgp_dynamic_neighbor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_bgp_dynamic_neighbor_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_bgp_dynamic_neighbor_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_bgp_neighbor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_bgp_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_bgp_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_bgp_session_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_bgp_session_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_bgp_session_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_bond_port_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_capacity_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_capacity_check_per_facility_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_capacity_check_per_facility_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_capacity_check_per_metro_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_capacity_check_per_metro_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_capacity_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_capacity_level_per_baremetal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_capacity_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_capacity_per_facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_capacity_per_metro_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_capacity_per_new_facility.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_capacity_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_create_device_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_create_email_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_create_metal_gateway_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_create_self_service_reservation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_create_self_service_reservation_request_period.py
--rw-r--r--   0 runner    (1001) docker     (123)    15802 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_device_action_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_device_actions_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_device_create_in_facility_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_device_create_in_metro_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_device_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_device_created_by.py
--rw-r--r--   0 runner    (1001) docker     (123)    17592 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_device_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_device_metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_device_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_device_project_lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_device_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_device_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_device_usage_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_devices_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_email_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_emails_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_entitlement.py
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_event_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_fabric_service_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_facilities_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_facility_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_facility_input_facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_facility_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    20932 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_find_ip_address_by_id200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    19764 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_find_metal_gateway_by_id200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_find_traffic_timeframe_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_global_bgp_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_global_bgp_range_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    21758 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_hardware_reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21406 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_hardware_reservation_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_hardware_reservations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_href.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_incidents_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_instances_batch_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_instances_batch_create_input_batches_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_instances_batch_create_input_batches_inner_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_interconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_interconnection_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_interconnection_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_interconnection_metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_interconnection_port.py
--rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_interconnection_port_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_interconnection_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_interconnections_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_invitation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_invitation_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_invitation_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_invitations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_ip_addresses_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_ip_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_ip_assignment_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_ip_assignment_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_ip_assignment_metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_ip_assignment_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_ip_availabilities_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_ip_reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_ip_reservation_facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_ip_reservation_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    20584 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_ip_reservation_list_ip_addresses_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_ip_reservation_metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_ip_reservation_request_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_license.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_license_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_license_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_license_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_licenses_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_membership_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_membership_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_metadata_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_metadata_network_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_metadata_network_network_bonding.py
--rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_metal_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_metal_gateway_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_metal_gateway_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    19800 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_metal_gateway_list_metal_gateways_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_metal_gateway_lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_metal_gateways_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_metro_capacity_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    20895 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_metro_capacity_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_metro_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_metro_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_metro_server_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_metros_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_move_hardware_reservation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_new_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_operating_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_operating_system_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_operating_systems_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7002 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_organization_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_organization_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_organizations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_otps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_parent_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_password_reset_tokens_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_payment_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_payment_method_billing_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_payment_method_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_payment_method_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_payment_method_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_payment_methods_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_plan_available_in_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_plan_available_in_inner_price.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_plan_available_in_metros_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_plan_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_plan_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_plan_specs_cpus_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_plan_specs_drives_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_plan_specs_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_plan_specs_nics_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_plans_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_port.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_port_assign_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_port_convert_layer3_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_port_convert_layer3_input_request_ips_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_port_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_port_vlan_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_port_vlan_assignment_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_port_vlan_assignment_batch_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_port_vlan_assignment_batch_create_input_vlan_assignments_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_port_vlan_assignment_batch_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_port_vlan_assignment_batch_vlan_assignments_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_port_vlan_assignment_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_ports_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_project_create_from_root_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_project_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_project_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_project_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_project_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_project_usage_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_projects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_recovery_code_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    20556 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_request_ip_reservation201_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_request_ip_reservation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_self_service_reservation_item_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_self_service_reservation_item_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_self_service_reservation_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_self_service_reservation_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_self_service_reservations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_server_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_spot_market_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_spot_market_prices_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_spot_market_prices_per_metro_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_spot_market_prices_per_metro_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_spot_market_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_spot_market_request_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_spot_market_request_create_input_instance_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_spot_market_request_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_spot_market_request_metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_spot_prices_datapoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_spot_prices_history_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_spot_prices_per_baremetal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_spot_prices_per_facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_spot_prices_per_new_facility.py
--rw-r--r--   0 runner    (1001) docker     (123)    11893 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_spot_prices_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_ssh_key_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_ssh_key_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_ssh_key_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_ssh_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_support_request_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_support_request_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_transfer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_transfer_request_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_transfer_request_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_transfer_requests_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_two_factor_auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_update_email_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_usages_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_user_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_user_limited.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_user_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_user_lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_user_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_user_verification_tokens_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_userdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_userdata_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_verify_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_virtual_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_virtual_circuit_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_virtual_circuit_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_virtual_circuit_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_virtual_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_virtual_network_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_virtual_network_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vlan_virtual_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vlan_virtual_circuit_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vlan_virtual_circuit_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vlans_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vrf_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    19965 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vrf_ip_reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vrf_ip_reservation_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vrf_ip_reservation_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vrf_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    19566 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vrf_metal_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vrf_metal_gateway_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vrf_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vrf_route_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vrf_route_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vrf_route_metal_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vrf_route_virtual_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vrf_route_vrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vrf_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vrf_virtual_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vrf_virtual_circuit_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vrf_virtual_circuit_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-06-09 09:19:38.000000 equinix-metal-0.2.1/test/test_vrfs_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:37:21.915559 equinix-metal-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-27 14:37:21.915559 equinix-metal-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    53051 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:37:21.767558 equinix-metal-0.2.2/equinix_metal/
+-rw-r--r--   0 runner    (1001) docker     (123)    24286 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:37:21.783558 equinix-metal-0.2.2/equinix_metal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46223 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/authentication_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35443 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/batches_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53275 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/bgp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42522 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/capacity_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   149000 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/devices_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32320 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/emails_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89081 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30060 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/facilities_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40324 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/hardware_reservations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/incidents_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110259 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/interconnections_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/invitations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/invoices_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58220 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/ip_addresses_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42404 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/licenses_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26100 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58972 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/metal_gateways_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16543 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/metros_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/operating_systems_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   128422 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/organizations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27611 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/otps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16686 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/password_reset_tokens_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26446 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/payment_methods_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22999 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/plans_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109267 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/ports_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90866 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27378 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/self_service_reservations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57754 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/spot_market_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65523 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/ssh_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/support_request_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25177 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/transfer_requests_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26624 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/two_factor_auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19788 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/usages_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17508 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/user_verification_tokens_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/userdata_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58053 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36376 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/vlans_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   140861 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api/vrfs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33612 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19317 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:37:21.847559 equinix-metal-0.2.2/equinix_metal/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    21522 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/activate_hardware_reservation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/auth_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/auth_token_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/auth_token_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/auth_token_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/auth_token_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/batches_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/bgp_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/bgp_config_request_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/bgp_dynamic_neighbor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/bgp_dynamic_neighbor_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/bgp_dynamic_neighbor_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/bgp_neighbor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/bgp_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/bgp_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/bgp_session_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/bgp_session_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/bgp_session_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/bond_port_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/capacity_check_per_facility_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/capacity_check_per_facility_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/capacity_check_per_metro_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/capacity_check_per_metro_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/capacity_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/capacity_level_per_baremetal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/capacity_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/capacity_per_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/capacity_per_metro_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/capacity_per_new_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/capacity_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/create_device_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/create_email_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/create_metal_gateway_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/create_self_service_reservation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/create_self_service_reservation_request_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17634 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/device_action_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/device_actions_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/device_create_in_facility_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/device_create_in_metro_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16915 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/device_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/device_created_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/device_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/device_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/device_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/device_project_lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/device_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/device_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/device_usage_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/email_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/entitlement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/event_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/fabric_service_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/facility_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/facility_input_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/facility_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/find_ip_address_by_id200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/find_metal_gateway_by_id200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/find_traffic_timeframe_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/global_bgp_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/global_bgp_range_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/hardware_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/hardware_reservation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/href.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/instances_batch_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/instances_batch_create_input_batches_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/instances_batch_create_input_batches_inner_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/interconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/interconnection_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/interconnection_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/interconnection_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/interconnection_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/interconnection_port_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/interconnection_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/invitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/invitation_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/invitation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/invoice_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/ip_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/ip_assignment_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/ip_assignment_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/ip_assignment_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/ip_assignment_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/ip_availabilities_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/ip_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/ip_reservation_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/ip_reservation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/ip_reservation_list_ip_addresses_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/ip_reservation_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/ip_reservation_request_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/license_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/license_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/license_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/membership_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/membership_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/metadata_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/metadata_network_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/metadata_network_network_bonding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/metal_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/metal_gateway_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/metal_gateway_elastic_ip_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/metal_gateway_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/metal_gateway_list_metal_gateways_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/metal_gateway_lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/metro_capacity_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/metro_capacity_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/metro_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/metro_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/metro_server_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/move_hardware_reservation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/new_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/operating_system_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/organization_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/organization_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/parent_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/payment_method_billing_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/payment_method_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/payment_method_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/payment_method_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/plan_available_in_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/plan_available_in_inner_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/plan_available_in_metros_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/plan_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/plan_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/plan_specs_cpus_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/plan_specs_drives_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/plan_specs_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/plan_specs_nics_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/port_assign_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/port_convert_layer3_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/port_convert_layer3_input_request_ips_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/port_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/port_vlan_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/port_vlan_assignment_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/port_vlan_assignment_batch_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/port_vlan_assignment_batch_create_input_vlan_assignments_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/port_vlan_assignment_batch_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/port_vlan_assignment_batch_vlan_assignments_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/port_vlan_assignment_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/project_create_from_root_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/project_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/project_id_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/project_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/project_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/project_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/project_usage_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/recovery_code_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/request_ip_reservation201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/request_ip_reservation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/self_service_reservation_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/self_service_reservation_item_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/self_service_reservation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/self_service_reservation_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/server_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/spot_market_prices_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/spot_market_prices_per_metro_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/spot_market_prices_per_metro_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/spot_market_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/spot_market_request_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/spot_market_request_create_input_instance_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6747 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/spot_market_request_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/spot_market_request_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/spot_prices_datapoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/spot_prices_history_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/spot_prices_per_baremetal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/spot_prices_per_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/spot_prices_per_new_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/spot_prices_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/ssh_key_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/ssh_key_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/ssh_key_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/support_request_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/transfer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/transfer_request_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/transfer_request_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/update_email_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/user_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/user_limited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/user_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/user_lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/user_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/userdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/verify_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/virtual_circuit_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/virtual_circuit_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/virtual_circuit_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/virtual_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/virtual_network_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/virtual_network_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10895 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/vlan_virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/vlan_virtual_circuit_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/vlan_virtual_circuit_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/vrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/vrf_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/vrf_ip_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/vrf_ip_reservation_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/vrf_ip_reservation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/vrf_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/vrf_metal_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/vrf_metal_gateway_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/vrf_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/vrf_route_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/vrf_route_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/vrf_route_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/vrf_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/vrf_virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/vrf_virtual_circuit_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/models/vrf_virtual_circuit_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/equinix_metal/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:37:21.771558 equinix-metal-0.2.2/equinix_metal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-27 14:37:21.000000 equinix-metal-0.2.2/equinix_metal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21367 2023-06-27 14:37:21.000000 equinix-metal-0.2.2/equinix_metal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:37:21.000000 equinix-metal-0.2.2/equinix_metal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 14:37:21.000000 equinix-metal-0.2.2/equinix_metal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 14:37:21.000000 equinix-metal-0.2.2/equinix_metal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-27 14:37:21.915559 equinix-metal-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:37:21.915559 equinix-metal-0.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_activate_hardware_reservation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_auth_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_auth_token_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_auth_token_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_auth_token_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_auth_token_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_authentication_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_batches_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_batches_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_bgp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_bgp_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_bgp_config_request_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_bgp_dynamic_neighbor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_bgp_dynamic_neighbor_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_bgp_dynamic_neighbor_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_bgp_neighbor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_bgp_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_bgp_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_bgp_session_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_bgp_session_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_bgp_session_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_bond_port_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_capacity_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_capacity_check_per_facility_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_capacity_check_per_facility_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_capacity_check_per_metro_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_capacity_check_per_metro_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_capacity_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_capacity_level_per_baremetal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_capacity_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_capacity_per_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_capacity_per_metro_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_capacity_per_new_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_capacity_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_create_device_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_create_email_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_create_metal_gateway_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_create_self_service_reservation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_create_self_service_reservation_request_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15937 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_device_action_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_device_actions_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_device_create_in_facility_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_device_create_in_metro_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_device_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_device_created_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17759 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_device_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_device_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_device_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_device_project_lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_device_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_device_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_device_usage_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_devices_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_email_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_emails_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_entitlement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_event_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_fabric_service_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_facilities_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_facility_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_facility_input_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_facility_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21174 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_find_ip_address_by_id200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_find_metal_gateway_by_id200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_find_traffic_timeframe_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_global_bgp_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_global_bgp_range_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21960 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_hardware_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21589 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_hardware_reservation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_hardware_reservations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_href.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_incidents_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_instances_batch_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_instances_batch_create_input_batches_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_instances_batch_create_input_batches_inner_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_interconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_interconnection_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_interconnection_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_interconnection_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_interconnection_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_interconnection_port_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_interconnection_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_interconnections_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_invitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_invitation_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_invitation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_invitations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_invoice_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_invoices_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_ip_addresses_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_ip_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_ip_assignment_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_ip_assignment_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_ip_assignment_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_ip_assignment_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_ip_availabilities_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_ip_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_ip_reservation_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_ip_reservation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20794 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_ip_reservation_list_ip_addresses_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_ip_reservation_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_ip_reservation_request_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_license_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_license_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_license_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_licenses_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_membership_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_membership_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_metadata_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_metadata_network_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_metadata_network_network_bonding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_metal_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_metal_gateway_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_metal_gateway_elastic_ip_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_metal_gateway_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19905 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_metal_gateway_list_metal_gateways_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_metal_gateway_lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_metal_gateways_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_metro_capacity_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20895 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_metro_capacity_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_metro_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_metro_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_metro_server_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_metros_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_move_hardware_reservation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_new_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_operating_system_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_operating_systems_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7002 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_organization_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_organization_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_organizations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_otps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_parent_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_password_reset_tokens_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_payment_method_billing_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_payment_method_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_payment_method_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_payment_method_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_payment_methods_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_plan_available_in_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_plan_available_in_inner_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_plan_available_in_metros_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_plan_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_plan_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_plan_specs_cpus_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_plan_specs_drives_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_plan_specs_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_plan_specs_nics_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_plans_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_port_assign_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_port_convert_layer3_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_port_convert_layer3_input_request_ips_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_port_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_port_vlan_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_port_vlan_assignment_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_port_vlan_assignment_batch_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_port_vlan_assignment_batch_create_input_vlan_assignments_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_port_vlan_assignment_batch_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_port_vlan_assignment_batch_vlan_assignments_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_port_vlan_assignment_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_ports_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_project_create_from_root_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_project_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_project_id_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_project_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_project_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_project_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_project_usage_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_recovery_code_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20766 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_request_ip_reservation201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_request_ip_reservation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_self_service_reservation_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_self_service_reservation_item_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_self_service_reservation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_self_service_reservation_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_self_service_reservations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_server_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_spot_market_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_spot_market_prices_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_spot_market_prices_per_metro_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_spot_market_prices_per_metro_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_spot_market_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_spot_market_request_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_spot_market_request_create_input_instance_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_spot_market_request_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_spot_market_request_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_spot_prices_datapoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_spot_prices_history_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_spot_prices_per_baremetal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_spot_prices_per_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_spot_prices_per_new_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11893 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_spot_prices_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_ssh_key_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_ssh_key_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_ssh_key_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_ssh_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_support_request_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_support_request_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_transfer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_transfer_request_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_transfer_request_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_transfer_requests_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_two_factor_auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_update_email_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_usages_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_user_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_user_limited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_user_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_user_lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_user_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_user_verification_tokens_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_userdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_userdata_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_verify_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12194 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_virtual_circuit_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_virtual_circuit_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_virtual_circuit_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_virtual_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_virtual_network_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_virtual_network_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_vlan_virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_vlan_virtual_circuit_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_vlan_virtual_circuit_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_vlans_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12995 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_vrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_vrf_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20175 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_vrf_ip_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_vrf_ip_reservation_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_vrf_ip_reservation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11869 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_vrf_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_vrf_metal_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_vrf_metal_gateway_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21831 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_vrf_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_vrf_route_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_vrf_route_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_vrf_route_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_vrf_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_vrf_virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_vrf_virtual_circuit_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_vrf_virtual_circuit_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-06-27 14:37:08.000000 equinix-metal-0.2.2/test/test_vrfs_api.py
```

### Comparing `equinix-metal-0.2.1/PKG-INFO` & `equinix-metal-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equinix-metal
-Version: 0.2.1
+Version: 0.2.2
 Summary: Metal API
 Home-page: 
 Author: Equinix Metal API Team
 Author-email: support@equinixmetal.com
 License: Equinix Metal
 Keywords: OpenAPI,OpenAPI-Generator,Metal API
 Description-Content-Type: text/markdown
```

### Comparing `equinix-metal-0.2.1/README.md` & `equinix-metal-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 To exclude resources, and optimize response delivery, use the `exclude` query parameter. The `exclude` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests for fields with nested object responses. When excluded, these fields will be replaced with an object that contains only an `href` field.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 0.2.1
+- Package version: 0.2.2
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -225,15 +225,16 @@
 *EventsApi* | [**find_device_events**](docs/EventsApi.md#find_device_events) | **GET** /devices/{id}/events | Retrieve device&#39;s events
 *EventsApi* | [**find_event_by_id**](docs/EventsApi.md#find_event_by_id) | **GET** /events/{id} | Retrieve an event
 *EventsApi* | [**find_events**](docs/EventsApi.md#find_events) | **GET** /events | Retrieve current user&#39;s events
 *EventsApi* | [**find_interconnection_events**](docs/EventsApi.md#find_interconnection_events) | **GET** /connections/{connection_id}/events | Retrieve interconnection events
 *EventsApi* | [**find_interconnection_port_events**](docs/EventsApi.md#find_interconnection_port_events) | **GET** /connections/{connection_id}/ports/{id}/events | Retrieve interconnection port events
 *EventsApi* | [**find_organization_events**](docs/EventsApi.md#find_organization_events) | **GET** /organizations/{id}/events | Retrieve organization&#39;s events
 *EventsApi* | [**find_project_events**](docs/EventsApi.md#find_project_events) | **GET** /projects/{id}/events | Retrieve project&#39;s events
-*EventsApi* | [**find_virtual_circuit_events**](docs/EventsApi.md#find_virtual_circuit_events) | **GET** /virtual-circuits/{id}/events | Retrieve interconnection events
+*EventsApi* | [**find_virtual_circuit_events**](docs/EventsApi.md#find_virtual_circuit_events) | **GET** /virtual-circuits/{id}/events | Retrieve virtual circuit events
+*EventsApi* | [**find_vrf_route_events**](docs/EventsApi.md#find_vrf_route_events) | **GET** /routes/{id}/events | Retrieve VRF route events
 *FacilitiesApi* | [**find_facilities**](docs/FacilitiesApi.md#find_facilities) | **GET** /facilities | Retrieve all facilities
 *FacilitiesApi* | [**find_facilities_by_organization**](docs/FacilitiesApi.md#find_facilities_by_organization) | **GET** /organizations/{id}/facilities | Retrieve all facilities visible by the organization
 *FacilitiesApi* | [**find_facilities_by_project**](docs/FacilitiesApi.md#find_facilities_by_project) | **GET** /projects/{id}/facilities | Retrieve all facilities visible by the project
 *HardwareReservationsApi* | [**activate_hardware_reservation**](docs/HardwareReservationsApi.md#activate_hardware_reservation) | **POST** /hardware-reservations/{id}/activate | Activate a spare hardware reservation
 *HardwareReservationsApi* | [**find_hardware_reservation_by_id**](docs/HardwareReservationsApi.md#find_hardware_reservation_by_id) | **GET** /hardware-reservations/{id} | Retrieve a hardware reservation
 *HardwareReservationsApi* | [**find_project_hardware_reservations**](docs/HardwareReservationsApi.md#find_project_hardware_reservations) | **GET** /projects/{id}/hardware-reservations | Retrieve all hardware reservations for a given project
 *HardwareReservationsApi* | [**move_hardware_reservation**](docs/HardwareReservationsApi.md#move_hardware_reservation) | **POST** /hardware-reservations/{id}/move | Move a hardware reservation
@@ -259,26 +260,30 @@
 *InterconnectionsApi* | [**organization_list_interconnections**](docs/InterconnectionsApi.md#organization_list_interconnections) | **GET** /organizations/{organization_id}/connections | List organization connections
 *InterconnectionsApi* | [**project_list_interconnections**](docs/InterconnectionsApi.md#project_list_interconnections) | **GET** /projects/{project_id}/connections | List project connections
 *InterconnectionsApi* | [**update_interconnection**](docs/InterconnectionsApi.md#update_interconnection) | **PUT** /connections/{connection_id} | Update interconnection
 *InterconnectionsApi* | [**update_virtual_circuit**](docs/InterconnectionsApi.md#update_virtual_circuit) | **PUT** /virtual-circuits/{id} | Update a virtual circuit
 *InvitationsApi* | [**accept_invitation**](docs/InvitationsApi.md#accept_invitation) | **PUT** /invitations/{id} | Accept an invitation
 *InvitationsApi* | [**decline_invitation**](docs/InvitationsApi.md#decline_invitation) | **DELETE** /invitations/{id} | Decline an invitation
 *InvitationsApi* | [**find_invitation_by_id**](docs/InvitationsApi.md#find_invitation_by_id) | **GET** /invitations/{id} | View an invitation
+*InvoicesApi* | [**find_organization_invoices**](docs/InvoicesApi.md#find_organization_invoices) | **GET** /organizations/{id}/invoices | Retrieve all invoices for an organization
+*InvoicesApi* | [**get_invoice_by_id**](docs/InvoicesApi.md#get_invoice_by_id) | **GET** /invoices/{id} | Retrieve an invoice
 *LicensesApi* | [**create_license**](docs/LicensesApi.md#create_license) | **POST** /projects/{id}/licenses | Create a License
 *LicensesApi* | [**delete_license**](docs/LicensesApi.md#delete_license) | **DELETE** /licenses/{id} | Delete the license
 *LicensesApi* | [**find_license_by_id**](docs/LicensesApi.md#find_license_by_id) | **GET** /licenses/{id} | Retrieve a license
 *LicensesApi* | [**find_project_licenses**](docs/LicensesApi.md#find_project_licenses) | **GET** /projects/{id}/licenses | Retrieve all licenses
 *LicensesApi* | [**update_license**](docs/LicensesApi.md#update_license) | **PUT** /licenses/{id} | Update the license
 *MembershipsApi* | [**delete_membership**](docs/MembershipsApi.md#delete_membership) | **DELETE** /memberships/{id} | Delete the membership
 *MembershipsApi* | [**find_membership_by_id**](docs/MembershipsApi.md#find_membership_by_id) | **GET** /memberships/{id} | Retrieve a membership
 *MembershipsApi* | [**update_membership**](docs/MembershipsApi.md#update_membership) | **PUT** /memberships/{id} | Update the membership
 *MetalGatewaysApi* | [**create_metal_gateway**](docs/MetalGatewaysApi.md#create_metal_gateway) | **POST** /projects/{project_id}/metal-gateways | Create a metal gateway
+*MetalGatewaysApi* | [**create_metal_gateway_elastic_ip**](docs/MetalGatewaysApi.md#create_metal_gateway_elastic_ip) | **POST** /metal-gateways/{id}/ips | Create a Metal Gateway Elastic IP
 *MetalGatewaysApi* | [**delete_metal_gateway**](docs/MetalGatewaysApi.md#delete_metal_gateway) | **DELETE** /metal-gateways/{id} | Deletes the metal gateway
 *MetalGatewaysApi* | [**find_metal_gateway_by_id**](docs/MetalGatewaysApi.md#find_metal_gateway_by_id) | **GET** /metal-gateways/{id} | Returns the metal gateway
 *MetalGatewaysApi* | [**find_metal_gateways_by_project**](docs/MetalGatewaysApi.md#find_metal_gateways_by_project) | **GET** /projects/{project_id}/metal-gateways | Returns all metal gateways for a project
+*MetalGatewaysApi* | [**get_metal_gateway_elastic_ips**](docs/MetalGatewaysApi.md#get_metal_gateway_elastic_ips) | **GET** /metal-gateways/{id}/ips | List Metal Gateway Elastic IPs
 *MetrosApi* | [**find_metros**](docs/MetrosApi.md#find_metros) | **GET** /locations/metros | Retrieve all metros
 *MetrosApi* | [**get_metro**](docs/MetrosApi.md#get_metro) | **GET** /locations/metros/{id} | Retrieve a specific Metro&#39;s details
 *OTPsApi* | [**find_ensure_otp**](docs/OTPsApi.md#find_ensure_otp) | **POST** /user/otp/verify/{otp} | Verify user by providing an OTP
 *OTPsApi* | [**find_recovery_codes**](docs/OTPsApi.md#find_recovery_codes) | **GET** /user/otp/recovery-codes | Retrieve my recovery codes
 *OTPsApi* | [**receive_codes**](docs/OTPsApi.md#receive_codes) | **POST** /user/otp/sms/receive | Receive an OTP per sms
 *OTPsApi* | [**regenerate_codes**](docs/OTPsApi.md#regenerate_codes) | **POST** /user/otp/recovery-codes | Generate new recovery codes
 *OperatingSystemsApi* | [**find_operating_system_version**](docs/OperatingSystemsApi.md#find_operating_system_version) | **GET** /operating-system-versions | Retrieve all operating system versions
@@ -368,23 +373,27 @@
 *UsersApi* | [**find_user_customdata**](docs/UsersApi.md#find_user_customdata) | **GET** /users/{id}/customdata | Retrieve the custom metadata of a user
 *UsersApi* | [**find_users**](docs/UsersApi.md#find_users) | **GET** /users | Retrieve all users
 *UsersApi* | [**update_current_user**](docs/UsersApi.md#update_current_user) | **PUT** /user | Update the current user
 *VLANsApi* | [**create_virtual_network**](docs/VLANsApi.md#create_virtual_network) | **POST** /projects/{id}/virtual-networks | Create a virtual network
 *VLANsApi* | [**delete_virtual_network**](docs/VLANsApi.md#delete_virtual_network) | **DELETE** /virtual-networks/{id} | Delete a virtual network
 *VLANsApi* | [**find_virtual_networks**](docs/VLANsApi.md#find_virtual_networks) | **GET** /projects/{id}/virtual-networks | Retrieve all virtual networks
 *VLANsApi* | [**get_virtual_network**](docs/VLANsApi.md#get_virtual_network) | **GET** /virtual-networks/{id} | Get a virtual network
+*VRFsApi* | [**bgp_dynamic_neighbors_id_get**](docs/VRFsApi.md#bgp_dynamic_neighbors_id_get) | **GET** /bgp-dynamic-neighbors/{id} | Retrieve a BGP Dynamic Neighbor
+*VRFsApi* | [**create_bgp_dynamic_neighbor**](docs/VRFsApi.md#create_bgp_dynamic_neighbor) | **POST** /metal-gateways/{id}/bgp-dynamic-neighbors | Create a VRF BGP Dynamic Neighbor range
 *VRFsApi* | [**create_vrf**](docs/VRFsApi.md#create_vrf) | **POST** /projects/{id}/vrfs | Create a new VRF in the specified project
 *VRFsApi* | [**create_vrf_route**](docs/VRFsApi.md#create_vrf_route) | **POST** /vrfs/{id}/routes | Create a VRF route
+*VRFsApi* | [**delete_bgp_dynamic_neighbor_by_id**](docs/VRFsApi.md#delete_bgp_dynamic_neighbor_by_id) | **DELETE** /bgp-dynamic-neighbors/{id} | Delete a VRF BGP Dynamic Neighbor
 *VRFsApi* | [**delete_vrf**](docs/VRFsApi.md#delete_vrf) | **DELETE** /vrfs/{id} | Delete the VRF
 *VRFsApi* | [**delete_vrf_route_by_id**](docs/VRFsApi.md#delete_vrf_route_by_id) | **DELETE** /routes/{id} | Delete a VRF Route
 *VRFsApi* | [**find_vrf_by_id**](docs/VRFsApi.md#find_vrf_by_id) | **GET** /vrfs/{id} | Retrieve a VRF
 *VRFsApi* | [**find_vrf_ip_reservation**](docs/VRFsApi.md#find_vrf_ip_reservation) | **GET** /vrfs/{vrf_id}/ips/{id} | Retrieve all VRF IP Reservations in the VRF
 *VRFsApi* | [**find_vrf_ip_reservations**](docs/VRFsApi.md#find_vrf_ip_reservations) | **GET** /vrfs/{id}/ips | Retrieve all VRF IP Reservations in the VRF
 *VRFsApi* | [**find_vrf_route_by_id**](docs/VRFsApi.md#find_vrf_route_by_id) | **GET** /routes/{id} | Retrieve a VRF Route
 *VRFsApi* | [**find_vrfs**](docs/VRFsApi.md#find_vrfs) | **GET** /projects/{id}/vrfs | Retrieve all VRFs in the project
+*VRFsApi* | [**get_bgp_dynamic_neighbors**](docs/VRFsApi.md#get_bgp_dynamic_neighbors) | **GET** /metal-gateways/{id}/bgp-dynamic-neighbors | List BGP Dynamic Neighbors
 *VRFsApi* | [**get_vrf_routes**](docs/VRFsApi.md#get_vrf_routes) | **GET** /vrfs/{id}/routes | Retrieve all routes in the VRF
 *VRFsApi* | [**update_vrf**](docs/VRFsApi.md#update_vrf) | **PUT** /vrfs/{id} | Update the VRF
 *VRFsApi* | [**update_vrf_route_by_id**](docs/VRFsApi.md#update_vrf_route_by_id) | **PUT** /routes/{id} | Update a VRF Route
 
 
 ## Documentation For Models
 
@@ -481,28 +490,32 @@
  - [InterconnectionMetro](docs/InterconnectionMetro.md)
  - [InterconnectionPort](docs/InterconnectionPort.md)
  - [InterconnectionPortList](docs/InterconnectionPortList.md)
  - [InterconnectionUpdateInput](docs/InterconnectionUpdateInput.md)
  - [Invitation](docs/Invitation.md)
  - [InvitationInput](docs/InvitationInput.md)
  - [InvitationList](docs/InvitationList.md)
+ - [Invoice](docs/Invoice.md)
+ - [InvoiceList](docs/InvoiceList.md)
  - [License](docs/License.md)
  - [LicenseCreateInput](docs/LicenseCreateInput.md)
  - [LicenseList](docs/LicenseList.md)
  - [LicenseUpdateInput](docs/LicenseUpdateInput.md)
+ - [LineItem](docs/LineItem.md)
  - [Membership](docs/Membership.md)
  - [MembershipInput](docs/MembershipInput.md)
  - [MembershipList](docs/MembershipList.md)
  - [Meta](docs/Meta.md)
  - [Metadata](docs/Metadata.md)
  - [MetadataNetwork](docs/MetadataNetwork.md)
  - [MetadataNetworkNetwork](docs/MetadataNetworkNetwork.md)
  - [MetadataNetworkNetworkBonding](docs/MetadataNetworkNetworkBonding.md)
  - [MetalGateway](docs/MetalGateway.md)
  - [MetalGatewayCreateInput](docs/MetalGatewayCreateInput.md)
+ - [MetalGatewayElasticIpCreateInput](docs/MetalGatewayElasticIpCreateInput.md)
  - [MetalGatewayList](docs/MetalGatewayList.md)
  - [MetalGatewayListMetalGatewaysInner](docs/MetalGatewayListMetalGatewaysInner.md)
  - [MetalGatewayLite](docs/MetalGatewayLite.md)
  - [Metro](docs/Metro.md)
  - [MetroCapacityList](docs/MetroCapacityList.md)
  - [MetroCapacityReport](docs/MetroCapacityReport.md)
  - [MetroInput](docs/MetroInput.md)
@@ -542,14 +555,15 @@
  - [PortVlanAssignmentBatchCreateInputVlanAssignmentsInner](docs/PortVlanAssignmentBatchCreateInputVlanAssignmentsInner.md)
  - [PortVlanAssignmentBatchList](docs/PortVlanAssignmentBatchList.md)
  - [PortVlanAssignmentBatchVlanAssignmentsInner](docs/PortVlanAssignmentBatchVlanAssignmentsInner.md)
  - [PortVlanAssignmentList](docs/PortVlanAssignmentList.md)
  - [Project](docs/Project.md)
  - [ProjectCreateFromRootInput](docs/ProjectCreateFromRootInput.md)
  - [ProjectCreateInput](docs/ProjectCreateInput.md)
+ - [ProjectIdName](docs/ProjectIdName.md)
  - [ProjectList](docs/ProjectList.md)
  - [ProjectUpdateInput](docs/ProjectUpdateInput.md)
  - [ProjectUsage](docs/ProjectUsage.md)
  - [ProjectUsageList](docs/ProjectUsageList.md)
  - [RecoveryCodeList](docs/RecoveryCodeList.md)
  - [RequestIPReservation201Response](docs/RequestIPReservation201Response.md)
  - [RequestIPReservationRequest](docs/RequestIPReservationRequest.md)
@@ -606,17 +620,15 @@
  - [VrfIpReservationList](docs/VrfIpReservationList.md)
  - [VrfList](docs/VrfList.md)
  - [VrfMetalGateway](docs/VrfMetalGateway.md)
  - [VrfMetalGatewayCreateInput](docs/VrfMetalGatewayCreateInput.md)
  - [VrfRoute](docs/VrfRoute.md)
  - [VrfRouteCreateInput](docs/VrfRouteCreateInput.md)
  - [VrfRouteList](docs/VrfRouteList.md)
- - [VrfRouteMetalGateway](docs/VrfRouteMetalGateway.md)
- - [VrfRouteVirtualNetwork](docs/VrfRouteVirtualNetwork.md)
- - [VrfRouteVrf](docs/VrfRouteVrf.md)
+ - [VrfRouteUpdateInput](docs/VrfRouteUpdateInput.md)
  - [VrfUpdateInput](docs/VrfUpdateInput.md)
  - [VrfVirtualCircuit](docs/VrfVirtualCircuit.md)
  - [VrfVirtualCircuitCreateInput](docs/VrfVirtualCircuitCreateInput.md)
  - [VrfVirtualCircuitUpdateInput](docs/VrfVirtualCircuitUpdateInput.md)
 
 
 ## Documentation For Authorization
```

### Comparing `equinix-metal-0.2.1/equinix_metal/__init__.py` & `equinix-metal-0.2.2/equinix_metal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     Do not edit the class manually.
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 # import apis into sdk package
 from equinix_metal.api.authentication_api import AuthenticationApi
 from equinix_metal.api.bgp_api import BGPApi
 from equinix_metal.api.batches_api import BatchesApi
 from equinix_metal.api.capacity_api import CapacityApi
 from equinix_metal.api.devices_api import DevicesApi
@@ -29,14 +29,15 @@
 from equinix_metal.api.events_api import EventsApi
 from equinix_metal.api.facilities_api import FacilitiesApi
 from equinix_metal.api.hardware_reservations_api import HardwareReservationsApi
 from equinix_metal.api.ip_addresses_api import IPAddressesApi
 from equinix_metal.api.incidents_api import IncidentsApi
 from equinix_metal.api.interconnections_api import InterconnectionsApi
 from equinix_metal.api.invitations_api import InvitationsApi
+from equinix_metal.api.invoices_api import InvoicesApi
 from equinix_metal.api.licenses_api import LicensesApi
 from equinix_metal.api.memberships_api import MembershipsApi
 from equinix_metal.api.metal_gateways_api import MetalGatewaysApi
 from equinix_metal.api.metros_api import MetrosApi
 from equinix_metal.api.otps_api import OTPsApi
 from equinix_metal.api.operating_systems_api import OperatingSystemsApi
 from equinix_metal.api.organizations_api import OrganizationsApi
@@ -161,28 +162,32 @@
 from equinix_metal.models.interconnection_metro import InterconnectionMetro
 from equinix_metal.models.interconnection_port import InterconnectionPort
 from equinix_metal.models.interconnection_port_list import InterconnectionPortList
 from equinix_metal.models.interconnection_update_input import InterconnectionUpdateInput
 from equinix_metal.models.invitation import Invitation
 from equinix_metal.models.invitation_input import InvitationInput
 from equinix_metal.models.invitation_list import InvitationList
+from equinix_metal.models.invoice import Invoice
+from equinix_metal.models.invoice_list import InvoiceList
 from equinix_metal.models.license import License
 from equinix_metal.models.license_create_input import LicenseCreateInput
 from equinix_metal.models.license_list import LicenseList
 from equinix_metal.models.license_update_input import LicenseUpdateInput
+from equinix_metal.models.line_item import LineItem
 from equinix_metal.models.membership import Membership
 from equinix_metal.models.membership_input import MembershipInput
 from equinix_metal.models.membership_list import MembershipList
 from equinix_metal.models.meta import Meta
 from equinix_metal.models.metadata import Metadata
 from equinix_metal.models.metadata_network import MetadataNetwork
 from equinix_metal.models.metadata_network_network import MetadataNetworkNetwork
 from equinix_metal.models.metadata_network_network_bonding import MetadataNetworkNetworkBonding
 from equinix_metal.models.metal_gateway import MetalGateway
 from equinix_metal.models.metal_gateway_create_input import MetalGatewayCreateInput
+from equinix_metal.models.metal_gateway_elastic_ip_create_input import MetalGatewayElasticIpCreateInput
 from equinix_metal.models.metal_gateway_list import MetalGatewayList
 from equinix_metal.models.metal_gateway_list_metal_gateways_inner import MetalGatewayListMetalGatewaysInner
 from equinix_metal.models.metal_gateway_lite import MetalGatewayLite
 from equinix_metal.models.metro import Metro
 from equinix_metal.models.metro_capacity_list import MetroCapacityList
 from equinix_metal.models.metro_capacity_report import MetroCapacityReport
 from equinix_metal.models.metro_input import MetroInput
@@ -222,14 +227,15 @@
 from equinix_metal.models.port_vlan_assignment_batch_create_input_vlan_assignments_inner import PortVlanAssignmentBatchCreateInputVlanAssignmentsInner
 from equinix_metal.models.port_vlan_assignment_batch_list import PortVlanAssignmentBatchList
 from equinix_metal.models.port_vlan_assignment_batch_vlan_assignments_inner import PortVlanAssignmentBatchVlanAssignmentsInner
 from equinix_metal.models.port_vlan_assignment_list import PortVlanAssignmentList
 from equinix_metal.models.project import Project
 from equinix_metal.models.project_create_from_root_input import ProjectCreateFromRootInput
 from equinix_metal.models.project_create_input import ProjectCreateInput
+from equinix_metal.models.project_id_name import ProjectIdName
 from equinix_metal.models.project_list import ProjectList
 from equinix_metal.models.project_update_input import ProjectUpdateInput
 from equinix_metal.models.project_usage import ProjectUsage
 from equinix_metal.models.project_usage_list import ProjectUsageList
 from equinix_metal.models.recovery_code_list import RecoveryCodeList
 from equinix_metal.models.request_ip_reservation201_response import RequestIPReservation201Response
 from equinix_metal.models.request_ip_reservation_request import RequestIPReservationRequest
@@ -286,14 +292,12 @@
 from equinix_metal.models.vrf_ip_reservation_list import VrfIpReservationList
 from equinix_metal.models.vrf_list import VrfList
 from equinix_metal.models.vrf_metal_gateway import VrfMetalGateway
 from equinix_metal.models.vrf_metal_gateway_create_input import VrfMetalGatewayCreateInput
 from equinix_metal.models.vrf_route import VrfRoute
 from equinix_metal.models.vrf_route_create_input import VrfRouteCreateInput
 from equinix_metal.models.vrf_route_list import VrfRouteList
-from equinix_metal.models.vrf_route_metal_gateway import VrfRouteMetalGateway
-from equinix_metal.models.vrf_route_virtual_network import VrfRouteVirtualNetwork
-from equinix_metal.models.vrf_route_vrf import VrfRouteVrf
+from equinix_metal.models.vrf_route_update_input import VrfRouteUpdateInput
 from equinix_metal.models.vrf_update_input import VrfUpdateInput
 from equinix_metal.models.vrf_virtual_circuit import VrfVirtualCircuit
 from equinix_metal.models.vrf_virtual_circuit_create_input import VrfVirtualCircuitCreateInput
 from equinix_metal.models.vrf_virtual_circuit_update_input import VrfVirtualCircuitUpdateInput
```

### Comparing `equinix-metal-0.2.1/equinix_metal/api/__init__.py` & `equinix-metal-0.2.2/equinix_metal/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from equinix_metal.api.events_api import EventsApi
 from equinix_metal.api.facilities_api import FacilitiesApi
 from equinix_metal.api.hardware_reservations_api import HardwareReservationsApi
 from equinix_metal.api.ip_addresses_api import IPAddressesApi
 from equinix_metal.api.incidents_api import IncidentsApi
 from equinix_metal.api.interconnections_api import InterconnectionsApi
 from equinix_metal.api.invitations_api import InvitationsApi
+from equinix_metal.api.invoices_api import InvoicesApi
 from equinix_metal.api.licenses_api import LicensesApi
 from equinix_metal.api.memberships_api import MembershipsApi
 from equinix_metal.api.metal_gateways_api import MetalGatewaysApi
 from equinix_metal.api.metros_api import MetrosApi
 from equinix_metal.api.otps_api import OTPsApi
 from equinix_metal.api.operating_systems_api import OperatingSystemsApi
 from equinix_metal.api.organizations_api import OrganizationsApi
```

### Comparing `equinix-metal-0.2.1/equinix_metal/api/authentication_api.py` & `equinix-metal-0.2.2/equinix_metal/api/authentication_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/batches_api.py` & `equinix-metal-0.2.2/equinix_metal/api/batches_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/bgp_api.py` & `equinix-metal-0.2.2/equinix_metal/api/bgp_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/capacity_api.py` & `equinix-metal-0.2.2/equinix_metal/api/capacity_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/devices_api.py` & `equinix-metal-0.2.2/equinix_metal/api/devices_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import Field, StrictBool, StrictStr, conint, conlist
+from pydantic import Field, StrictBool, StrictStr, conint, conlist, validator
 
 from typing import Dict, Optional
 
 from equinix_metal.models.bgp_session_input import BGPSessionInput
 from equinix_metal.models.bgp_session import BgpSession
 from equinix_metal.models.bgp_session_list import BgpSessionList
 from equinix_metal.models.bgp_session_neighbors import BgpSessionNeighbors
@@ -213,28 +213,32 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def create_device(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], create_device_request : Annotated[CreateDeviceRequest, Field(..., description="Device to create")], **kwargs) -> Device:  # noqa: E501
+    def create_device(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], create_device_request : Annotated[CreateDeviceRequest, Field(..., description="Device to create")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> Device:  # noqa: E501
         """Create a device  # noqa: E501
 
         Creates a new device and provisions it in the specified location.  Device type-specific options are accepted.  For example, `baremetal` devices accept `operating_system`, `hostname`, and `plan`. These parameters may not be accepted for other device types. The default device type is `baremetal`.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_device(id, create_device_request, async_req=True)
+        >>> thread = api.create_device(id, create_device_request, include, exclude, async_req=True)
         >>> result = thread.get()
 
         :param id: Project UUID (required)
         :type id: str
         :param create_device_request: Device to create (required)
         :type create_device_request: CreateDeviceRequest
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -243,31 +247,35 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: Device
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_device_with_http_info(id, create_device_request, **kwargs)  # noqa: E501
+        return self.create_device_with_http_info(id, create_device_request, include, exclude, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_device_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], create_device_request : Annotated[CreateDeviceRequest, Field(..., description="Device to create")], **kwargs):  # noqa: E501
+    def create_device_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], create_device_request : Annotated[CreateDeviceRequest, Field(..., description="Device to create")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
         """Create a device  # noqa: E501
 
         Creates a new device and provisions it in the specified location.  Device type-specific options are accepted.  For example, `baremetal` devices accept `operating_system`, `hostname`, and `plan`. These parameters may not be accepted for other device types. The default device type is `baremetal`.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_device_with_http_info(id, create_device_request, async_req=True)
+        >>> thread = api.create_device_with_http_info(id, create_device_request, include, exclude, async_req=True)
         >>> result = thread.get()
 
         :param id: Project UUID (required)
         :type id: str
         :param create_device_request: Device to create (required)
         :type create_device_request: CreateDeviceRequest
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -288,15 +296,17 @@
         :rtype: tuple(Device, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
-            'create_device_request'
+            'create_device_request',
+            'include',
+            'exclude'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -322,14 +332,22 @@
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
 
         # process the query parameters
         _query_params = []
+        if _params.get('include') is not None:  # noqa: E501
+            _query_params.append(('include', _params['include']))
+            _collection_formats['include'] = 'csv'
+
+        if _params.get('exclude') is not None:  # noqa: E501
+            _query_params.append(('exclude', _params['exclude']))
+            _collection_formats['exclude'] = 'csv'
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
@@ -372,28 +390,32 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def create_ip_assignment(self, id : Annotated[StrictStr, Field(..., description="Device UUID")], ip_assignment_input : Annotated[IPAssignmentInput, Field(..., description="IPAssignment to create")], **kwargs) -> IPAssignment:  # noqa: E501
+    def create_ip_assignment(self, id : Annotated[StrictStr, Field(..., description="Device UUID")], ip_assignment_input : Annotated[IPAssignmentInput, Field(..., description="IPAssignment to create")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> IPAssignment:  # noqa: E501
         """Create an ip assignment  # noqa: E501
 
         Creates an ip assignment for a device.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_ip_assignment(id, ip_assignment_input, async_req=True)
+        >>> thread = api.create_ip_assignment(id, ip_assignment_input, include, exclude, async_req=True)
         >>> result = thread.get()
 
         :param id: Device UUID (required)
         :type id: str
         :param ip_assignment_input: IPAssignment to create (required)
         :type ip_assignment_input: IPAssignmentInput
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -402,31 +424,35 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: IPAssignment
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_ip_assignment_with_http_info(id, ip_assignment_input, **kwargs)  # noqa: E501
+        return self.create_ip_assignment_with_http_info(id, ip_assignment_input, include, exclude, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_ip_assignment_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Device UUID")], ip_assignment_input : Annotated[IPAssignmentInput, Field(..., description="IPAssignment to create")], **kwargs):  # noqa: E501
+    def create_ip_assignment_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Device UUID")], ip_assignment_input : Annotated[IPAssignmentInput, Field(..., description="IPAssignment to create")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
         """Create an ip assignment  # noqa: E501
 
         Creates an ip assignment for a device.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_ip_assignment_with_http_info(id, ip_assignment_input, async_req=True)
+        >>> thread = api.create_ip_assignment_with_http_info(id, ip_assignment_input, include, exclude, async_req=True)
         >>> result = thread.get()
 
         :param id: Device UUID (required)
         :type id: str
         :param ip_assignment_input: IPAssignment to create (required)
         :type ip_assignment_input: IPAssignmentInput
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -447,15 +473,17 @@
         :rtype: tuple(IPAssignment, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
-            'ip_assignment_input'
+            'ip_assignment_input',
+            'include',
+            'exclude'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -481,14 +509,22 @@
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
 
         # process the query parameters
         _query_params = []
+        if _params.get('include') is not None:  # noqa: E501
+            _query_params.append(('include', _params['include']))
+            _collection_formats['include'] = 'csv'
+
+        if _params.get('exclude') is not None:  # noqa: E501
+            _query_params.append(('exclude', _params['exclude']))
+            _collection_formats['exclude'] = 'csv'
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
@@ -1863,36 +1899,40 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def find_organization_devices(self, id : Annotated[StrictStr, Field(..., description="Organization UUID")], facility : Annotated[Optional[StrictStr], Field(description="Filter by device facility")] = None, hostname : Annotated[Optional[StrictStr], Field(description="Filter by partial hostname")] = None, reserved : Annotated[Optional[StrictBool], Field(description="Filter only reserved instances")] = None, tag : Annotated[Optional[StrictStr], Field(description="Filter by device tag")] = None, type : Annotated[Optional[StrictStr], Field(description="Filter by instance type (ondemand,spot,reserved)")] = None, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs) -> DeviceList:  # noqa: E501
+    def find_organization_devices(self, id : Annotated[StrictStr, Field(..., description="Organization UUID")], categories : Annotated[Optional[conlist(StrictStr)], Field(description="Filter by plan category")] = None, facility : Annotated[Optional[StrictStr], Field(description="Filter by device facility")] = None, hostname : Annotated[Optional[StrictStr], Field(description="Filter by partial hostname")] = None, reserved : Annotated[Optional[StrictBool], Field(description="Filter only reserved instances. When set to true, only include reserved instances. When set to false, only include on-demand instances.")] = None, tag : Annotated[Optional[StrictStr], Field(description="Filter by device tag")] = None, type : Annotated[Optional[StrictStr], Field(description="Filter by instance type (ondemand,spot,reserved)")] = None, has_termination_time : Annotated[Optional[StrictBool], Field(description="Filter only instances marked for termination. When set to true, only include instances that have a termination time. When set to false, only include instances that do not have a termination time.")] = None, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs) -> DeviceList:  # noqa: E501
         """Retrieve all devices of an organization  # noqa: E501
 
         Provides a collection of devices for a given organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_organization_devices(id, facility, hostname, reserved, tag, type, include, exclude, page, per_page, async_req=True)
+        >>> thread = api.find_organization_devices(id, categories, facility, hostname, reserved, tag, type, has_termination_time, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
         :param id: Organization UUID (required)
         :type id: str
+        :param categories: Filter by plan category
+        :type categories: List[str]
         :param facility: Filter by device facility
         :type facility: str
         :param hostname: Filter by partial hostname
         :type hostname: str
-        :param reserved: Filter only reserved instances
+        :param reserved: Filter only reserved instances. When set to true, only include reserved instances. When set to false, only include on-demand instances.
         :type reserved: bool
         :param tag: Filter by device tag
         :type tag: str
         :param type: Filter by instance type (ondemand,spot,reserved)
         :type type: str
+        :param has_termination_time: Filter only instances marked for termination. When set to true, only include instances that have a termination time. When set to false, only include instances that do not have a termination time.
+        :type has_termination_time: bool
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
         :param page: Page to return
         :type page: int
         :param per_page: Items returned per page
@@ -1909,39 +1949,43 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: DeviceList
         """
         kwargs['_return_http_data_only'] = True
-        return self.find_organization_devices_with_http_info(id, facility, hostname, reserved, tag, type, include, exclude, page, per_page, **kwargs)  # noqa: E501
+        return self.find_organization_devices_with_http_info(id, categories, facility, hostname, reserved, tag, type, has_termination_time, include, exclude, page, per_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def find_organization_devices_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Organization UUID")], facility : Annotated[Optional[StrictStr], Field(description="Filter by device facility")] = None, hostname : Annotated[Optional[StrictStr], Field(description="Filter by partial hostname")] = None, reserved : Annotated[Optional[StrictBool], Field(description="Filter only reserved instances")] = None, tag : Annotated[Optional[StrictStr], Field(description="Filter by device tag")] = None, type : Annotated[Optional[StrictStr], Field(description="Filter by instance type (ondemand,spot,reserved)")] = None, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs):  # noqa: E501
+    def find_organization_devices_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Organization UUID")], categories : Annotated[Optional[conlist(StrictStr)], Field(description="Filter by plan category")] = None, facility : Annotated[Optional[StrictStr], Field(description="Filter by device facility")] = None, hostname : Annotated[Optional[StrictStr], Field(description="Filter by partial hostname")] = None, reserved : Annotated[Optional[StrictBool], Field(description="Filter only reserved instances. When set to true, only include reserved instances. When set to false, only include on-demand instances.")] = None, tag : Annotated[Optional[StrictStr], Field(description="Filter by device tag")] = None, type : Annotated[Optional[StrictStr], Field(description="Filter by instance type (ondemand,spot,reserved)")] = None, has_termination_time : Annotated[Optional[StrictBool], Field(description="Filter only instances marked for termination. When set to true, only include instances that have a termination time. When set to false, only include instances that do not have a termination time.")] = None, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs):  # noqa: E501
         """Retrieve all devices of an organization  # noqa: E501
 
         Provides a collection of devices for a given organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_organization_devices_with_http_info(id, facility, hostname, reserved, tag, type, include, exclude, page, per_page, async_req=True)
+        >>> thread = api.find_organization_devices_with_http_info(id, categories, facility, hostname, reserved, tag, type, has_termination_time, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
         :param id: Organization UUID (required)
         :type id: str
+        :param categories: Filter by plan category
+        :type categories: List[str]
         :param facility: Filter by device facility
         :type facility: str
         :param hostname: Filter by partial hostname
         :type hostname: str
-        :param reserved: Filter only reserved instances
+        :param reserved: Filter only reserved instances. When set to true, only include reserved instances. When set to false, only include on-demand instances.
         :type reserved: bool
         :param tag: Filter by device tag
         :type tag: str
         :param type: Filter by instance type (ondemand,spot,reserved)
         :type type: str
+        :param has_termination_time: Filter only instances marked for termination. When set to true, only include instances that have a termination time. When set to false, only include instances that do not have a termination time.
+        :type has_termination_time: bool
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
         :param page: Page to return
         :type page: int
         :param per_page: Items returned per page
@@ -1970,19 +2014,21 @@
         :rtype: tuple(DeviceList, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'categories',
             'facility',
             'hostname',
             'reserved',
             'tag',
             'type',
+            'has_termination_time',
             'include',
             'exclude',
             'page',
             'per_page'
         ]
         _all_params.extend(
             [
@@ -2012,14 +2058,18 @@
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
 
         # process the query parameters
         _query_params = []
+        if _params.get('categories') is not None:  # noqa: E501
+            _query_params.append(('categories', _params['categories']))
+            _collection_formats['categories'] = 'multi'
+
         if _params.get('facility') is not None:  # noqa: E501
             _query_params.append(('facility', _params['facility']))
 
         if _params.get('hostname') is not None:  # noqa: E501
             _query_params.append(('hostname', _params['hostname']))
 
         if _params.get('reserved') is not None:  # noqa: E501
@@ -2027,14 +2077,17 @@
 
         if _params.get('tag') is not None:  # noqa: E501
             _query_params.append(('tag', _params['tag']))
 
         if _params.get('type') is not None:  # noqa: E501
             _query_params.append(('type', _params['type']))
 
+        if _params.get('has_termination_time') is not None:  # noqa: E501
+            _query_params.append(('has_termination_time', _params['has_termination_time']))
+
         if _params.get('include') is not None:  # noqa: E501
             _query_params.append(('include', _params['include']))
             _collection_formats['include'] = 'csv'
 
         if _params.get('exclude') is not None:  # noqa: E501
             _query_params.append(('exclude', _params['exclude']))
             _collection_formats['exclude'] = 'csv'
@@ -2080,36 +2133,40 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def find_project_devices(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], facility : Annotated[Optional[StrictStr], Field(description="Filter by device facility")] = None, hostname : Annotated[Optional[StrictStr], Field(description="Filter by partial hostname")] = None, reserved : Annotated[Optional[StrictBool], Field(description="Filter only reserved instances")] = None, tag : Annotated[Optional[StrictStr], Field(description="Filter by device tag")] = None, type : Annotated[Optional[StrictStr], Field(description="Filter by instance type (ondemand,spot,reserved)")] = None, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs) -> DeviceList:  # noqa: E501
+    def find_project_devices(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], categories : Annotated[Optional[conlist(StrictStr)], Field(description="Filter by plan category")] = None, facility : Annotated[Optional[StrictStr], Field(description="Filter by device facility")] = None, hostname : Annotated[Optional[StrictStr], Field(description="Filter by partial hostname")] = None, reserved : Annotated[Optional[StrictBool], Field(description="Filter only reserved instances. When set to true, only include reserved instances. When set to false, only include on-demand instances.")] = None, tag : Annotated[Optional[StrictStr], Field(description="Filter by device tag")] = None, type : Annotated[Optional[StrictStr], Field(description="Filter by instance type (ondemand,spot,reserved)")] = None, has_termination_time : Annotated[Optional[StrictBool], Field(description="Filter only instances marked for termination. When set to true, only include instances that have a termination time. When set to false, only include instances that do not have a termination time.")] = None, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs) -> DeviceList:  # noqa: E501
         """Retrieve all devices of a project  # noqa: E501
 
         Provides a collection of devices for a given project.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_project_devices(id, facility, hostname, reserved, tag, type, include, exclude, page, per_page, async_req=True)
+        >>> thread = api.find_project_devices(id, categories, facility, hostname, reserved, tag, type, has_termination_time, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
         :param id: Project UUID (required)
         :type id: str
+        :param categories: Filter by plan category
+        :type categories: List[str]
         :param facility: Filter by device facility
         :type facility: str
         :param hostname: Filter by partial hostname
         :type hostname: str
-        :param reserved: Filter only reserved instances
+        :param reserved: Filter only reserved instances. When set to true, only include reserved instances. When set to false, only include on-demand instances.
         :type reserved: bool
         :param tag: Filter by device tag
         :type tag: str
         :param type: Filter by instance type (ondemand,spot,reserved)
         :type type: str
+        :param has_termination_time: Filter only instances marked for termination. When set to true, only include instances that have a termination time. When set to false, only include instances that do not have a termination time.
+        :type has_termination_time: bool
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
         :param page: Page to return
         :type page: int
         :param per_page: Items returned per page
@@ -2126,39 +2183,43 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: DeviceList
         """
         kwargs['_return_http_data_only'] = True
-        return self.find_project_devices_with_http_info(id, facility, hostname, reserved, tag, type, include, exclude, page, per_page, **kwargs)  # noqa: E501
+        return self.find_project_devices_with_http_info(id, categories, facility, hostname, reserved, tag, type, has_termination_time, include, exclude, page, per_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def find_project_devices_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], facility : Annotated[Optional[StrictStr], Field(description="Filter by device facility")] = None, hostname : Annotated[Optional[StrictStr], Field(description="Filter by partial hostname")] = None, reserved : Annotated[Optional[StrictBool], Field(description="Filter only reserved instances")] = None, tag : Annotated[Optional[StrictStr], Field(description="Filter by device tag")] = None, type : Annotated[Optional[StrictStr], Field(description="Filter by instance type (ondemand,spot,reserved)")] = None, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs):  # noqa: E501
+    def find_project_devices_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], categories : Annotated[Optional[conlist(StrictStr)], Field(description="Filter by plan category")] = None, facility : Annotated[Optional[StrictStr], Field(description="Filter by device facility")] = None, hostname : Annotated[Optional[StrictStr], Field(description="Filter by partial hostname")] = None, reserved : Annotated[Optional[StrictBool], Field(description="Filter only reserved instances. When set to true, only include reserved instances. When set to false, only include on-demand instances.")] = None, tag : Annotated[Optional[StrictStr], Field(description="Filter by device tag")] = None, type : Annotated[Optional[StrictStr], Field(description="Filter by instance type (ondemand,spot,reserved)")] = None, has_termination_time : Annotated[Optional[StrictBool], Field(description="Filter only instances marked for termination. When set to true, only include instances that have a termination time. When set to false, only include instances that do not have a termination time.")] = None, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs):  # noqa: E501
         """Retrieve all devices of a project  # noqa: E501
 
         Provides a collection of devices for a given project.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_project_devices_with_http_info(id, facility, hostname, reserved, tag, type, include, exclude, page, per_page, async_req=True)
+        >>> thread = api.find_project_devices_with_http_info(id, categories, facility, hostname, reserved, tag, type, has_termination_time, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
         :param id: Project UUID (required)
         :type id: str
+        :param categories: Filter by plan category
+        :type categories: List[str]
         :param facility: Filter by device facility
         :type facility: str
         :param hostname: Filter by partial hostname
         :type hostname: str
-        :param reserved: Filter only reserved instances
+        :param reserved: Filter only reserved instances. When set to true, only include reserved instances. When set to false, only include on-demand instances.
         :type reserved: bool
         :param tag: Filter by device tag
         :type tag: str
         :param type: Filter by instance type (ondemand,spot,reserved)
         :type type: str
+        :param has_termination_time: Filter only instances marked for termination. When set to true, only include instances that have a termination time. When set to false, only include instances that do not have a termination time.
+        :type has_termination_time: bool
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
         :param page: Page to return
         :type page: int
         :param per_page: Items returned per page
@@ -2187,19 +2248,21 @@
         :rtype: tuple(DeviceList, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'categories',
             'facility',
             'hostname',
             'reserved',
             'tag',
             'type',
+            'has_termination_time',
             'include',
             'exclude',
             'page',
             'per_page'
         ]
         _all_params.extend(
             [
@@ -2229,14 +2292,18 @@
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
 
         # process the query parameters
         _query_params = []
+        if _params.get('categories') is not None:  # noqa: E501
+            _query_params.append(('categories', _params['categories']))
+            _collection_formats['categories'] = 'multi'
+
         if _params.get('facility') is not None:  # noqa: E501
             _query_params.append(('facility', _params['facility']))
 
         if _params.get('hostname') is not None:  # noqa: E501
             _query_params.append(('hostname', _params['hostname']))
 
         if _params.get('reserved') is not None:  # noqa: E501
@@ -2244,14 +2311,17 @@
 
         if _params.get('tag') is not None:  # noqa: E501
             _query_params.append(('tag', _params['tag']))
 
         if _params.get('type') is not None:  # noqa: E501
             _query_params.append(('type', _params['type']))
 
+        if _params.get('has_termination_time') is not None:  # noqa: E501
+            _query_params.append(('has_termination_time', _params['has_termination_time']))
+
         if _params.get('include') is not None:  # noqa: E501
             _query_params.append(('include', _params['include']))
             _collection_formats['include'] = 'csv'
 
         if _params.get('exclude') is not None:  # noqa: E501
             _query_params.append(('exclude', _params['exclude']))
             _collection_formats['exclude'] = 'csv'
```

### Comparing `equinix-metal-0.2.1/equinix_metal/api/emails_api.py` & `equinix-metal-0.2.2/equinix_metal/api/emails_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/events_api.py` & `equinix-metal-0.2.2/equinix_metal/api/events_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1265,15 +1265,15 @@
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
     def find_virtual_circuit_events(self, id : Annotated[StrictStr, Field(..., description="Virtual Circuit UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs) -> Event:  # noqa: E501
-        """Retrieve interconnection events  # noqa: E501
+        """Retrieve virtual circuit events  # noqa: E501
 
         Returns a list of the virtual circuit events  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.find_virtual_circuit_events(id, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
@@ -1304,15 +1304,15 @@
         :rtype: Event
         """
         kwargs['_return_http_data_only'] = True
         return self.find_virtual_circuit_events_with_http_info(id, include, exclude, page, per_page, **kwargs)  # noqa: E501
 
     @validate_arguments
     def find_virtual_circuit_events_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Virtual Circuit UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs):  # noqa: E501
-        """Retrieve interconnection events  # noqa: E501
+        """Retrieve virtual circuit events  # noqa: E501
 
         Returns a list of the virtual circuit events  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.find_virtual_circuit_events_with_http_info(id, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
@@ -1432,14 +1432,191 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def find_vrf_route_events(self, id : Annotated[StrictStr, Field(..., description="VRF Route UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs) -> Event:  # noqa: E501
+        """Retrieve VRF route events  # noqa: E501
+
+        Returns a list of the VRF route events  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.find_vrf_route_events(id, include, exclude, page, per_page, async_req=True)
+        >>> result = thread.get()
+
+        :param id: VRF Route UUID (required)
+        :type id: str
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param page: Page to return
+        :type page: int
+        :param per_page: Items returned per page
+        :type per_page: int
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: Event
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.find_vrf_route_events_with_http_info(id, include, exclude, page, per_page, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def find_vrf_route_events_with_http_info(self, id : Annotated[StrictStr, Field(..., description="VRF Route UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs):  # noqa: E501
+        """Retrieve VRF route events  # noqa: E501
+
+        Returns a list of the VRF route events  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.find_vrf_route_events_with_http_info(id, include, exclude, page, per_page, async_req=True)
+        >>> result = thread.get()
+
+        :param id: VRF Route UUID (required)
+        :type id: str
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param page: Page to return
+        :type page: int
+        :param per_page: Items returned per page
+        :type per_page: int
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(Event, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'id',
+            'include',
+            'exclude',
+            'page',
+            'per_page'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method find_vrf_route_events" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['id']:
+            _path_params['id'] = _params['id']
+
+
+        # process the query parameters
+        _query_params = []
+        if _params.get('include') is not None:  # noqa: E501
+            _query_params.append(('include', _params['include']))
+            _collection_formats['include'] = 'csv'
+
+        if _params.get('exclude') is not None:  # noqa: E501
+            _query_params.append(('exclude', _params['exclude']))
+            _collection_formats['exclude'] = 'csv'
+
+        if _params.get('page') is not None:  # noqa: E501
+            _query_params.append(('page', _params['page']))
+
+        if _params.get('per_page') is not None:  # noqa: E501
+            _query_params.append(('per_page', _params['per_page']))
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['x_auth_token']  # noqa: E501
+
+        _response_types_map = {
+            '200': "Event",
+            '401': "Error",
+            '403': "Error",
+            '404': "Error",
+        }
+
+        return self.api_client.call_api(
+            '/routes/{id}/events', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `equinix-metal-0.2.1/equinix_metal/api/facilities_api.py` & `equinix-metal-0.2.2/equinix_metal/api/facilities_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/hardware_reservations_api.py` & `equinix-metal-0.2.2/equinix_metal/api/hardware_reservations_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/incidents_api.py` & `equinix-metal-0.2.2/equinix_metal/api/incidents_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/interconnections_api.py` & `equinix-metal-0.2.2/equinix_metal/api/interconnections_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/invitations_api.py` & `equinix-metal-0.2.2/equinix_metal/api/invitations_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/ip_addresses_api.py` & `equinix-metal-0.2.2/equinix_metal/api/ip_addresses_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
     def delete_ip_address(self, id : Annotated[StrictStr, Field(..., description="IP Address UUID")], **kwargs) -> None:  # noqa: E501
         """Unassign an ip address  # noqa: E501
 
-        Note! This call can be used to un-assign an IP assignment or delete an IP reservation. Un-assign an IP address record. Use the assignment UUID you get after attaching the IP. This will remove the relationship between an IP and the device and will make the IP address available to be assigned to another device. Delete and IP reservation. Use the reservation UUID you get after adding the IP to the project. This will permanently delete the IP block reservation from the project.  # noqa: E501
+        This call can be used to un-assign an IP assignment or delete an IP reservation.  Un-assign an IP address record. Use the assignment UUID you get after attaching the IP. This will remove the relationship between an IP and the device or metal gateway and will make the IP address available to be assigned to another device, once the IP has been un-configured from the network.  Delete an IP reservation. Use the reservation UUID you get after adding the IP to the project. This will permanently delete the IP block reservation from the project.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_ip_address(id, async_req=True)
         >>> result = thread.get()
 
         :param id: IP Address UUID (required)
@@ -81,15 +81,15 @@
         kwargs['_return_http_data_only'] = True
         return self.delete_ip_address_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def delete_ip_address_with_http_info(self, id : Annotated[StrictStr, Field(..., description="IP Address UUID")], **kwargs):  # noqa: E501
         """Unassign an ip address  # noqa: E501
 
-        Note! This call can be used to un-assign an IP assignment or delete an IP reservation. Un-assign an IP address record. Use the assignment UUID you get after attaching the IP. This will remove the relationship between an IP and the device and will make the IP address available to be assigned to another device. Delete and IP reservation. Use the reservation UUID you get after adding the IP to the project. This will permanently delete the IP block reservation from the project.  # noqa: E501
+        This call can be used to un-assign an IP assignment or delete an IP reservation.  Un-assign an IP address record. Use the assignment UUID you get after attaching the IP. This will remove the relationship between an IP and the device or metal gateway and will make the IP address available to be assigned to another device, once the IP has been un-configured from the network.  Delete an IP reservation. Use the reservation UUID you get after adding the IP to the project. This will permanently delete the IP block reservation from the project.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_ip_address_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: IP Address UUID (required)
```

### Comparing `equinix-metal-0.2.1/equinix_metal/api/licenses_api.py` & `equinix-metal-0.2.2/equinix_metal/api/licenses_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/memberships_api.py` & `equinix-metal-0.2.2/equinix_metal/api/memberships_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/metal_gateways_api.py` & `equinix-metal-0.2.2/equinix_metal/api/metal_gateways_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
 from pydantic import Field, StrictStr, conint, conlist
 
 from typing import Optional
 
 from equinix_metal.models.create_metal_gateway_request import CreateMetalGatewayRequest
 from equinix_metal.models.find_metal_gateway_by_id200_response import FindMetalGatewayById200Response
+from equinix_metal.models.ip_assignment import IPAssignment
+from equinix_metal.models.ip_assignment_list import IPAssignmentList
+from equinix_metal.models.metal_gateway_elastic_ip_create_input import MetalGatewayElasticIpCreateInput
 from equinix_metal.models.metal_gateway_list import MetalGatewayList
 
 from equinix_metal.api_client import ApiClient
 from equinix_metal.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
@@ -236,18 +239,177 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def create_metal_gateway_elastic_ip(self, id : Annotated[StrictStr, Field(..., description="Metal Gateway UUID")], metal_gateway_elastic_ip_create_input : MetalGatewayElasticIpCreateInput, **kwargs) -> IPAssignment:  # noqa: E501
+        """Create a Metal Gateway Elastic IP  # noqa: E501
+
+        Create a new Elastic IP on this Metal Gateway.  Assign an IPv4 range as an elastic IP to the Metal Gateway, with a specified next-hop address contained within the Metal Gateway.  Notice: Elastic IPs on Metal Gateways are a test feature currently under active development, and only available to certain users. Please contact Customer Success for more information.   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_metal_gateway_elastic_ip(id, metal_gateway_elastic_ip_create_input, async_req=True)
+        >>> result = thread.get()
+
+        :param id: Metal Gateway UUID (required)
+        :type id: str
+        :param metal_gateway_elastic_ip_create_input: (required)
+        :type metal_gateway_elastic_ip_create_input: MetalGatewayElasticIpCreateInput
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: IPAssignment
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.create_metal_gateway_elastic_ip_with_http_info(id, metal_gateway_elastic_ip_create_input, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def create_metal_gateway_elastic_ip_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Metal Gateway UUID")], metal_gateway_elastic_ip_create_input : MetalGatewayElasticIpCreateInput, **kwargs):  # noqa: E501
+        """Create a Metal Gateway Elastic IP  # noqa: E501
+
+        Create a new Elastic IP on this Metal Gateway.  Assign an IPv4 range as an elastic IP to the Metal Gateway, with a specified next-hop address contained within the Metal Gateway.  Notice: Elastic IPs on Metal Gateways are a test feature currently under active development, and only available to certain users. Please contact Customer Success for more information.   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_metal_gateway_elastic_ip_with_http_info(id, metal_gateway_elastic_ip_create_input, async_req=True)
+        >>> result = thread.get()
+
+        :param id: Metal Gateway UUID (required)
+        :type id: str
+        :param metal_gateway_elastic_ip_create_input: (required)
+        :type metal_gateway_elastic_ip_create_input: MetalGatewayElasticIpCreateInput
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(IPAssignment, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'id',
+            'metal_gateway_elastic_ip_create_input'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method create_metal_gateway_elastic_ip" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['id']:
+            _path_params['id'] = _params['id']
+
+
+        # process the query parameters
+        _query_params = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        if _params['metal_gateway_elastic_ip_create_input']:
+            _body_params = _params['metal_gateway_elastic_ip_create_input']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['x_auth_token']  # noqa: E501
+
+        _response_types_map = {
+            '201': "IPAssignment",
+            '401': "Error",
+            '403': "Error",
+            '404': "Error",
+            '422': "Error",
+        }
+
+        return self.api_client.call_api(
+            '/metal-gateways/{id}/ips', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def delete_metal_gateway(self, id : Annotated[StrictStr, Field(..., description="Metal Gateway UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> FindMetalGatewayById200Response:  # noqa: E501
         """Deletes the metal gateway  # noqa: E501
 
-        Deletes a specific metal gateway  # noqa: E501
+        Deletes a metal gateway and any elastic IP assignments associated with this metal gateway.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_metal_gateway(id, include, exclude, async_req=True)
         >>> result = thread.get()
 
         :param id: Metal Gateway UUID (required)
@@ -274,15 +436,15 @@
         kwargs['_return_http_data_only'] = True
         return self.delete_metal_gateway_with_http_info(id, include, exclude, **kwargs)  # noqa: E501
 
     @validate_arguments
     def delete_metal_gateway_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Metal Gateway UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
         """Deletes the metal gateway  # noqa: E501
 
-        Deletes a specific metal gateway  # noqa: E501
+        Deletes a metal gateway and any elastic IP assignments associated with this metal gateway.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_metal_gateway_with_http_info(id, include, exclude, async_req=True)
         >>> result = thread.get()
 
         :param id: Metal Gateway UUID (required)
@@ -723,14 +885,174 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def get_metal_gateway_elastic_ips(self, id : Annotated[StrictStr, Field(..., description="Metal Gateway UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> IPAssignmentList:  # noqa: E501
+        """List Metal Gateway Elastic IPs  # noqa: E501
+
+        Returns the list of Elastic IPs assigned to this Metal Gateway  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_metal_gateway_elastic_ips(id, include, exclude, async_req=True)
+        >>> result = thread.get()
+
+        :param id: Metal Gateway UUID (required)
+        :type id: str
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: IPAssignmentList
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.get_metal_gateway_elastic_ips_with_http_info(id, include, exclude, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def get_metal_gateway_elastic_ips_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Metal Gateway UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
+        """List Metal Gateway Elastic IPs  # noqa: E501
+
+        Returns the list of Elastic IPs assigned to this Metal Gateway  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_metal_gateway_elastic_ips_with_http_info(id, include, exclude, async_req=True)
+        >>> result = thread.get()
+
+        :param id: Metal Gateway UUID (required)
+        :type id: str
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(IPAssignmentList, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'id',
+            'include',
+            'exclude'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_metal_gateway_elastic_ips" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['id']:
+            _path_params['id'] = _params['id']
+
+
+        # process the query parameters
+        _query_params = []
+        if _params.get('include') is not None:  # noqa: E501
+            _query_params.append(('include', _params['include']))
+            _collection_formats['include'] = 'csv'
+
+        if _params.get('exclude') is not None:  # noqa: E501
+            _query_params.append(('exclude', _params['exclude']))
+            _collection_formats['exclude'] = 'csv'
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['x_auth_token']  # noqa: E501
+
+        _response_types_map = {
+            '200': "IPAssignmentList",
+            '401': "Error",
+            '404': "Error",
+        }
+
+        return self.api_client.call_api(
+            '/metal-gateways/{id}/ips', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `equinix-metal-0.2.1/equinix_metal/api/metros_api.py` & `equinix-metal-0.2.2/equinix_metal/api/metros_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/operating_systems_api.py` & `equinix-metal-0.2.2/equinix_metal/api/operating_systems_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/organizations_api.py` & `equinix-metal-0.2.2/equinix_metal/api/organizations_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,26 +56,30 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_organization(self, organization_input : Annotated[OrganizationInput, Field(..., description="Organization to create")], **kwargs) -> Organization:  # noqa: E501
+    def create_organization(self, organization_input : Annotated[OrganizationInput, Field(..., description="Organization to create")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> Organization:  # noqa: E501
         """Create an organization  # noqa: E501
 
         Creates an organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_organization(organization_input, async_req=True)
+        >>> thread = api.create_organization(organization_input, include, exclude, async_req=True)
         >>> result = thread.get()
 
         :param organization_input: Organization to create (required)
         :type organization_input: OrganizationInput
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -84,29 +88,33 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: Organization
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_organization_with_http_info(organization_input, **kwargs)  # noqa: E501
+        return self.create_organization_with_http_info(organization_input, include, exclude, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_organization_with_http_info(self, organization_input : Annotated[OrganizationInput, Field(..., description="Organization to create")], **kwargs):  # noqa: E501
+    def create_organization_with_http_info(self, organization_input : Annotated[OrganizationInput, Field(..., description="Organization to create")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
         """Create an organization  # noqa: E501
 
         Creates an organization.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_organization_with_http_info(organization_input, async_req=True)
+        >>> thread = api.create_organization_with_http_info(organization_input, include, exclude, async_req=True)
         >>> result = thread.get()
 
         :param organization_input: Organization to create (required)
         :type organization_input: OrganizationInput
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -126,15 +134,17 @@
                  returns the request thread.
         :rtype: tuple(Organization, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'organization_input'
+            'organization_input',
+            'include',
+            'exclude'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -157,14 +167,22 @@
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
+        if _params.get('include') is not None:  # noqa: E501
+            _query_params.append(('include', _params['include']))
+            _collection_formats['include'] = 'csv'
+
+        if _params.get('exclude') is not None:  # noqa: E501
+            _query_params.append(('exclude', _params['exclude']))
+            _collection_formats['exclude'] = 'csv'
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
```

### Comparing `equinix-metal-0.2.1/equinix_metal/api/otps_api.py` & `equinix-metal-0.2.2/equinix_metal/api/otps_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/password_reset_tokens_api.py` & `equinix-metal-0.2.2/equinix_metal/api/password_reset_tokens_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/payment_methods_api.py` & `equinix-metal-0.2.2/equinix_metal/api/payment_methods_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/plans_api.py` & `equinix-metal-0.2.2/equinix_metal/api/plans_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import Field, StrictStr, conlist
+from pydantic import Field, StrictStr, conlist, validator
 
 from typing import Optional
 
 from equinix_metal.models.plan_list import PlanList
 
 from equinix_metal.api_client import ApiClient
 from equinix_metal.exceptions import (  # noqa: F401
@@ -42,26 +42,30 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def find_plans(self, type : Annotated[Optional[StrictStr], Field(description="Filter plans by its plan type")] = None, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> PlanList:  # noqa: E501
+    def find_plans(self, categories : Annotated[Optional[conlist(StrictStr)], Field(description="Filter plans by its category")] = None, type : Annotated[Optional[StrictStr], Field(description="Filter plans by its plan type")] = None, slug : Annotated[Optional[StrictStr], Field(description="Filter plans by slug")] = None, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> PlanList:  # noqa: E501
         """Retrieve all plans  # noqa: E501
 
         Provides a listing of available plans to provision your device on.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_plans(type, include, exclude, async_req=True)
+        >>> thread = api.find_plans(categories, type, slug, include, exclude, async_req=True)
         >>> result = thread.get()
 
+        :param categories: Filter plans by its category
+        :type categories: List[str]
         :param type: Filter plans by its plan type
         :type type: str
+        :param slug: Filter plans by slug
+        :type slug: str
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -74,29 +78,33 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: PlanList
         """
         kwargs['_return_http_data_only'] = True
-        return self.find_plans_with_http_info(type, include, exclude, **kwargs)  # noqa: E501
+        return self.find_plans_with_http_info(categories, type, slug, include, exclude, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def find_plans_with_http_info(self, type : Annotated[Optional[StrictStr], Field(description="Filter plans by its plan type")] = None, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
+    def find_plans_with_http_info(self, categories : Annotated[Optional[conlist(StrictStr)], Field(description="Filter plans by its category")] = None, type : Annotated[Optional[StrictStr], Field(description="Filter plans by its plan type")] = None, slug : Annotated[Optional[StrictStr], Field(description="Filter plans by slug")] = None, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
         """Retrieve all plans  # noqa: E501
 
         Provides a listing of available plans to provision your device on.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_plans_with_http_info(type, include, exclude, async_req=True)
+        >>> thread = api.find_plans_with_http_info(categories, type, slug, include, exclude, async_req=True)
         >>> result = thread.get()
 
+        :param categories: Filter plans by its category
+        :type categories: List[str]
         :param type: Filter plans by its plan type
         :type type: str
+        :param slug: Filter plans by slug
+        :type slug: str
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -120,15 +128,17 @@
                  returns the request thread.
         :rtype: tuple(PlanList, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'categories',
             'type',
+            'slug',
             'include',
             'exclude'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -153,17 +163,24 @@
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
+        if _params.get('categories') is not None:  # noqa: E501
+            _query_params.append(('categories', _params['categories']))
+            _collection_formats['categories'] = 'multi'
+
         if _params.get('type') is not None:  # noqa: E501
             _query_params.append(('type', _params['type']))
 
+        if _params.get('slug') is not None:  # noqa: E501
+            _query_params.append(('slug', _params['slug']))
+
         if _params.get('include') is not None:  # noqa: E501
             _query_params.append(('include', _params['include']))
             _collection_formats['include'] = 'csv'
 
         if _params.get('exclude') is not None:  # noqa: E501
             _query_params.append(('exclude', _params['exclude']))
             _collection_formats['exclude'] = 'csv'
```

### Comparing `equinix-metal-0.2.1/equinix_metal/api/ports_api.py` & `equinix-metal-0.2.2/equinix_metal/api/ports_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/projects_api.py` & `equinix-metal-0.2.2/equinix_metal/api/projects_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,26 +51,30 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_project(self, project_create_from_root_input : Annotated[ProjectCreateFromRootInput, Field(..., description="Project to create")], **kwargs) -> Project:  # noqa: E501
+    def create_project(self, project_create_from_root_input : Annotated[ProjectCreateFromRootInput, Field(..., description="Project to create")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> Project:  # noqa: E501
         """Create a project  # noqa: E501
 
         Creates a new project for the user default organization. If the user don't have an organization, a new one will be created.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_project(project_create_from_root_input, async_req=True)
+        >>> thread = api.create_project(project_create_from_root_input, include, exclude, async_req=True)
         >>> result = thread.get()
 
         :param project_create_from_root_input: Project to create (required)
         :type project_create_from_root_input: ProjectCreateFromRootInput
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -79,29 +83,33 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: Project
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_project_with_http_info(project_create_from_root_input, **kwargs)  # noqa: E501
+        return self.create_project_with_http_info(project_create_from_root_input, include, exclude, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_project_with_http_info(self, project_create_from_root_input : Annotated[ProjectCreateFromRootInput, Field(..., description="Project to create")], **kwargs):  # noqa: E501
+    def create_project_with_http_info(self, project_create_from_root_input : Annotated[ProjectCreateFromRootInput, Field(..., description="Project to create")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
         """Create a project  # noqa: E501
 
         Creates a new project for the user default organization. If the user don't have an organization, a new one will be created.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_project_with_http_info(project_create_from_root_input, async_req=True)
+        >>> thread = api.create_project_with_http_info(project_create_from_root_input, include, exclude, async_req=True)
         >>> result = thread.get()
 
         :param project_create_from_root_input: Project to create (required)
         :type project_create_from_root_input: ProjectCreateFromRootInput
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -121,15 +129,17 @@
                  returns the request thread.
         :rtype: tuple(Project, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'project_create_from_root_input'
+            'project_create_from_root_input',
+            'include',
+            'exclude'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -152,14 +162,22 @@
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
+        if _params.get('include') is not None:  # noqa: E501
+            _query_params.append(('include', _params['include']))
+            _collection_formats['include'] = 'csv'
+
+        if _params.get('exclude') is not None:  # noqa: E501
+            _query_params.append(('exclude', _params['exclude']))
+            _collection_formats['exclude'] = 'csv'
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
```

### Comparing `equinix-metal-0.2.1/equinix_metal/api/self_service_reservations_api.py` & `equinix-metal-0.2.2/equinix_metal/api/self_service_reservations_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import Field, StrictStr, conint
+from pydantic import Field, StrictStr, conint, conlist, validator
 
 from typing import Optional
 
 from equinix_metal.models.create_self_service_reservation_request import CreateSelfServiceReservationRequest
 from equinix_metal.models.self_service_reservation_list import SelfServiceReservationList
 from equinix_metal.models.self_service_reservation_response import SelfServiceReservationResponse
 
@@ -351,30 +351,32 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def find_self_service_reservations(self, project_id : Annotated[StrictStr, Field(..., description="Project UUID")], page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs) -> SelfServiceReservationList:  # noqa: E501
+    def find_self_service_reservations(self, project_id : Annotated[StrictStr, Field(..., description="Project UUID")], page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, categories : Annotated[Optional[conlist(StrictStr)], Field(description="Filter reservations by items category")] = None, **kwargs) -> SelfServiceReservationList:  # noqa: E501
         """Retrieve all reservations  # noqa: E501
 
         Returns all reservations.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_self_service_reservations(project_id, page, per_page, async_req=True)
+        >>> thread = api.find_self_service_reservations(project_id, page, per_page, categories, async_req=True)
         >>> result = thread.get()
 
         :param project_id: Project UUID (required)
         :type project_id: str
         :param page: Page to return
         :type page: int
         :param per_page: Items returned per page
         :type per_page: int
+        :param categories: Filter reservations by items category
+        :type categories: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -383,33 +385,35 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: SelfServiceReservationList
         """
         kwargs['_return_http_data_only'] = True
-        return self.find_self_service_reservations_with_http_info(project_id, page, per_page, **kwargs)  # noqa: E501
+        return self.find_self_service_reservations_with_http_info(project_id, page, per_page, categories, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def find_self_service_reservations_with_http_info(self, project_id : Annotated[StrictStr, Field(..., description="Project UUID")], page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs):  # noqa: E501
+    def find_self_service_reservations_with_http_info(self, project_id : Annotated[StrictStr, Field(..., description="Project UUID")], page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, categories : Annotated[Optional[conlist(StrictStr)], Field(description="Filter reservations by items category")] = None, **kwargs):  # noqa: E501
         """Retrieve all reservations  # noqa: E501
 
         Returns all reservations.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_self_service_reservations_with_http_info(project_id, page, per_page, async_req=True)
+        >>> thread = api.find_self_service_reservations_with_http_info(project_id, page, per_page, categories, async_req=True)
         >>> result = thread.get()
 
         :param project_id: Project UUID (required)
         :type project_id: str
         :param page: Page to return
         :type page: int
         :param per_page: Items returned per page
         :type per_page: int
+        :param categories: Filter reservations by items category
+        :type categories: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -431,15 +435,16 @@
         """
 
         _params = locals()
 
         _all_params = [
             'project_id',
             'page',
-            'per_page'
+            'per_page',
+            'categories'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -471,14 +476,18 @@
         _query_params = []
         if _params.get('page') is not None:  # noqa: E501
             _query_params.append(('page', _params['page']))
 
         if _params.get('per_page') is not None:  # noqa: E501
             _query_params.append(('per_page', _params['per_page']))
 
+        if _params.get('categories') is not None:  # noqa: E501
+            _query_params.append(('categories', _params['categories']))
+            _collection_formats['categories'] = 'multi'
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
```

### Comparing `equinix-metal-0.2.1/equinix_metal/api/spot_market_api.py` & `equinix-metal-0.2.2/equinix_metal/api/spot_market_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/ssh_keys_api.py` & `equinix-metal-0.2.2/equinix_metal/api/ssh_keys_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/support_request_api.py` & `equinix-metal-0.2.2/equinix_metal/api/support_request_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/transfer_requests_api.py` & `equinix-metal-0.2.2/equinix_metal/api/transfer_requests_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/two_factor_auth_api.py` & `equinix-metal-0.2.2/equinix_metal/api/two_factor_auth_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/usages_api.py` & `equinix-metal-0.2.2/equinix_metal/api/usages_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/user_verification_tokens_api.py` & `equinix-metal-0.2.2/equinix_metal/api/user_verification_tokens_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/userdata_api.py` & `equinix-metal-0.2.2/equinix_metal/api/userdata_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/users_api.py` & `equinix-metal-0.2.2/equinix_metal/api/users_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/api/vlans_api.py` & `equinix-metal-0.2.2/equinix_metal/api/vlans_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,28 +44,32 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_virtual_network(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], virtual_network_create_input : Annotated[VirtualNetworkCreateInput, Field(..., description="Virtual Network to create")], **kwargs) -> VirtualNetwork:  # noqa: E501
+    def create_virtual_network(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], virtual_network_create_input : Annotated[VirtualNetworkCreateInput, Field(..., description="Virtual Network to create")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> VirtualNetwork:  # noqa: E501
         """Create a virtual network  # noqa: E501
 
         Creates an virtual network.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_virtual_network(id, virtual_network_create_input, async_req=True)
+        >>> thread = api.create_virtual_network(id, virtual_network_create_input, include, exclude, async_req=True)
         >>> result = thread.get()
 
         :param id: Project UUID (required)
         :type id: str
         :param virtual_network_create_input: Virtual Network to create (required)
         :type virtual_network_create_input: VirtualNetworkCreateInput
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -74,31 +78,35 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: VirtualNetwork
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_virtual_network_with_http_info(id, virtual_network_create_input, **kwargs)  # noqa: E501
+        return self.create_virtual_network_with_http_info(id, virtual_network_create_input, include, exclude, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_virtual_network_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], virtual_network_create_input : Annotated[VirtualNetworkCreateInput, Field(..., description="Virtual Network to create")], **kwargs):  # noqa: E501
+    def create_virtual_network_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], virtual_network_create_input : Annotated[VirtualNetworkCreateInput, Field(..., description="Virtual Network to create")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
         """Create a virtual network  # noqa: E501
 
         Creates an virtual network.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_virtual_network_with_http_info(id, virtual_network_create_input, async_req=True)
+        >>> thread = api.create_virtual_network_with_http_info(id, virtual_network_create_input, include, exclude, async_req=True)
         >>> result = thread.get()
 
         :param id: Project UUID (required)
         :type id: str
         :param virtual_network_create_input: Virtual Network to create (required)
         :type virtual_network_create_input: VirtualNetworkCreateInput
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -119,15 +127,17 @@
         :rtype: tuple(VirtualNetwork, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
-            'virtual_network_create_input'
+            'virtual_network_create_input',
+            'include',
+            'exclude'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -153,14 +163,22 @@
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
 
         # process the query parameters
         _query_params = []
+        if _params.get('include') is not None:  # noqa: E501
+            _query_params.append(('include', _params['include']))
+            _collection_formats['include'] = 'csv'
+
+        if _params.get('exclude') is not None:  # noqa: E501
+            _query_params.append(('exclude', _params['exclude']))
+            _collection_formats['exclude'] = 'csv'
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
```

### Comparing `equinix-metal-0.2.1/equinix_metal/api/vrfs_api.py` & `equinix-metal-0.2.2/equinix_metal/api/vrfs_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,22 +20,26 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr, conlist
 
 from typing import Optional
 
+from equinix_metal.models.bgp_dynamic_neighbor import BgpDynamicNeighbor
+from equinix_metal.models.bgp_dynamic_neighbor_create_input import BgpDynamicNeighborCreateInput
+from equinix_metal.models.bgp_dynamic_neighbor_list import BgpDynamicNeighborList
 from equinix_metal.models.vrf import Vrf
 from equinix_metal.models.vrf_create_input import VrfCreateInput
 from equinix_metal.models.vrf_ip_reservation import VrfIpReservation
 from equinix_metal.models.vrf_ip_reservation_list import VrfIpReservationList
 from equinix_metal.models.vrf_list import VrfList
 from equinix_metal.models.vrf_route import VrfRoute
 from equinix_metal.models.vrf_route_create_input import VrfRouteCreateInput
 from equinix_metal.models.vrf_route_list import VrfRouteList
+from equinix_metal.models.vrf_route_update_input import VrfRouteUpdateInput
 from equinix_metal.models.vrf_update_input import VrfUpdateInput
 
 from equinix_metal.api_client import ApiClient
 from equinix_metal.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
@@ -50,28 +54,369 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_vrf(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], vrf_create_input : Annotated[VrfCreateInput, Field(..., description="VRF to create")], **kwargs) -> Vrf:  # noqa: E501
+    def bgp_dynamic_neighbors_id_get(self, id : Annotated[StrictStr, Field(..., description="BGP Dynamic Neighbor UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> BgpDynamicNeighbor:  # noqa: E501
+        """Retrieve a BGP Dynamic Neighbor  # noqa: E501
+
+        Return a single BGP Dynamic Neighbor resource  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.bgp_dynamic_neighbors_id_get(id, include, exclude, async_req=True)
+        >>> result = thread.get()
+
+        :param id: BGP Dynamic Neighbor UUID (required)
+        :type id: str
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: BgpDynamicNeighbor
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.bgp_dynamic_neighbors_id_get_with_http_info(id, include, exclude, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def bgp_dynamic_neighbors_id_get_with_http_info(self, id : Annotated[StrictStr, Field(..., description="BGP Dynamic Neighbor UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
+        """Retrieve a BGP Dynamic Neighbor  # noqa: E501
+
+        Return a single BGP Dynamic Neighbor resource  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.bgp_dynamic_neighbors_id_get_with_http_info(id, include, exclude, async_req=True)
+        >>> result = thread.get()
+
+        :param id: BGP Dynamic Neighbor UUID (required)
+        :type id: str
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(BgpDynamicNeighbor, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'id',
+            'include',
+            'exclude'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method bgp_dynamic_neighbors_id_get" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['id']:
+            _path_params['id'] = _params['id']
+
+
+        # process the query parameters
+        _query_params = []
+        if _params.get('include') is not None:  # noqa: E501
+            _query_params.append(('include', _params['include']))
+            _collection_formats['include'] = 'csv'
+
+        if _params.get('exclude') is not None:  # noqa: E501
+            _query_params.append(('exclude', _params['exclude']))
+            _collection_formats['exclude'] = 'csv'
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['x_auth_token']  # noqa: E501
+
+        _response_types_map = {
+            '200': "BgpDynamicNeighbor",
+            '401': "Error",
+            '404': "Error",
+        }
+
+        return self.api_client.call_api(
+            '/bgp-dynamic-neighbors/{id}', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def create_bgp_dynamic_neighbor(self, id : Annotated[StrictStr, Field(..., description="Metal Gateway UUID")], bgp_dynamic_neighbor_create_input : BgpDynamicNeighborCreateInput, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> BgpDynamicNeighbor:  # noqa: E501
+        """Create a VRF BGP Dynamic Neighbor range  # noqa: E501
+
+        Create a VRF BGP Dynamic Neighbor range.  BGP Dynamic Neighbor records are limited to 2 per Virtual Network.  Notice: VRFs are a test feature currently under active development, and only available to certain users. Please contact Customer Success for more information.   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_bgp_dynamic_neighbor(id, bgp_dynamic_neighbor_create_input, include, exclude, async_req=True)
+        >>> result = thread.get()
+
+        :param id: Metal Gateway UUID (required)
+        :type id: str
+        :param bgp_dynamic_neighbor_create_input: (required)
+        :type bgp_dynamic_neighbor_create_input: BgpDynamicNeighborCreateInput
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: BgpDynamicNeighbor
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.create_bgp_dynamic_neighbor_with_http_info(id, bgp_dynamic_neighbor_create_input, include, exclude, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def create_bgp_dynamic_neighbor_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Metal Gateway UUID")], bgp_dynamic_neighbor_create_input : BgpDynamicNeighborCreateInput, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
+        """Create a VRF BGP Dynamic Neighbor range  # noqa: E501
+
+        Create a VRF BGP Dynamic Neighbor range.  BGP Dynamic Neighbor records are limited to 2 per Virtual Network.  Notice: VRFs are a test feature currently under active development, and only available to certain users. Please contact Customer Success for more information.   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_bgp_dynamic_neighbor_with_http_info(id, bgp_dynamic_neighbor_create_input, include, exclude, async_req=True)
+        >>> result = thread.get()
+
+        :param id: Metal Gateway UUID (required)
+        :type id: str
+        :param bgp_dynamic_neighbor_create_input: (required)
+        :type bgp_dynamic_neighbor_create_input: BgpDynamicNeighborCreateInput
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(BgpDynamicNeighbor, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'id',
+            'bgp_dynamic_neighbor_create_input',
+            'include',
+            'exclude'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method create_bgp_dynamic_neighbor" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['id']:
+            _path_params['id'] = _params['id']
+
+
+        # process the query parameters
+        _query_params = []
+        if _params.get('include') is not None:  # noqa: E501
+            _query_params.append(('include', _params['include']))
+            _collection_formats['include'] = 'csv'
+
+        if _params.get('exclude') is not None:  # noqa: E501
+            _query_params.append(('exclude', _params['exclude']))
+            _collection_formats['exclude'] = 'csv'
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        if _params['bgp_dynamic_neighbor_create_input']:
+            _body_params = _params['bgp_dynamic_neighbor_create_input']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['x_auth_token']  # noqa: E501
+
+        _response_types_map = {
+            '201': "BgpDynamicNeighbor",
+            '401': "Error",
+            '403': "Error",
+            '404': "Error",
+            '422': "Error",
+        }
+
+        return self.api_client.call_api(
+            '/metal-gateways/{id}/bgp-dynamic-neighbors', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def create_vrf(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], vrf_create_input : Annotated[VrfCreateInput, Field(..., description="VRF to create")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> Vrf:  # noqa: E501
         """Create a new VRF in the specified project  # noqa: E501
 
         Creates a new VRF in the specified project  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_vrf(id, vrf_create_input, async_req=True)
+        >>> thread = api.create_vrf(id, vrf_create_input, include, exclude, async_req=True)
         >>> result = thread.get()
 
         :param id: Project UUID (required)
         :type id: str
         :param vrf_create_input: VRF to create (required)
         :type vrf_create_input: VrfCreateInput
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -80,31 +425,35 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: Vrf
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_vrf_with_http_info(id, vrf_create_input, **kwargs)  # noqa: E501
+        return self.create_vrf_with_http_info(id, vrf_create_input, include, exclude, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_vrf_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], vrf_create_input : Annotated[VrfCreateInput, Field(..., description="VRF to create")], **kwargs):  # noqa: E501
+    def create_vrf_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], vrf_create_input : Annotated[VrfCreateInput, Field(..., description="VRF to create")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
         """Create a new VRF in the specified project  # noqa: E501
 
         Creates a new VRF in the specified project  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_vrf_with_http_info(id, vrf_create_input, async_req=True)
+        >>> thread = api.create_vrf_with_http_info(id, vrf_create_input, include, exclude, async_req=True)
         >>> result = thread.get()
 
         :param id: Project UUID (required)
         :type id: str
         :param vrf_create_input: VRF to create (required)
         :type vrf_create_input: VrfCreateInput
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -125,15 +474,17 @@
         :rtype: tuple(Vrf, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
-            'vrf_create_input'
+            'vrf_create_input',
+            'include',
+            'exclude'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -159,14 +510,22 @@
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
 
         # process the query parameters
         _query_params = []
+        if _params.get('include') is not None:  # noqa: E501
+            _query_params.append(('include', _params['include']))
+            _collection_formats['include'] = 'csv'
+
+        if _params.get('exclude') is not None:  # noqa: E501
+            _query_params.append(('exclude', _params['exclude']))
+            _collection_formats['exclude'] = 'csv'
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
@@ -208,28 +567,32 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def create_vrf_route(self, id : Annotated[StrictStr, Field(..., description="VRF UUID")], vrf_route_create_input : VrfRouteCreateInput, **kwargs) -> VrfRoute:  # noqa: E501
+    def create_vrf_route(self, id : Annotated[StrictStr, Field(..., description="VRF UUID")], vrf_route_create_input : VrfRouteCreateInput, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> VrfRoute:  # noqa: E501
         """Create a VRF route  # noqa: E501
 
         Create a route in a VRF. Currently only static default routes are supported.  Notice: VRFs are a test feature currently under active development, and only available to certain users. Please contact Customer Success for more information.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_vrf_route(id, vrf_route_create_input, async_req=True)
+        >>> thread = api.create_vrf_route(id, vrf_route_create_input, include, exclude, async_req=True)
         >>> result = thread.get()
 
         :param id: VRF UUID (required)
         :type id: str
         :param vrf_route_create_input: (required)
         :type vrf_route_create_input: VrfRouteCreateInput
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -238,31 +601,35 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: VrfRoute
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_vrf_route_with_http_info(id, vrf_route_create_input, **kwargs)  # noqa: E501
+        return self.create_vrf_route_with_http_info(id, vrf_route_create_input, include, exclude, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_vrf_route_with_http_info(self, id : Annotated[StrictStr, Field(..., description="VRF UUID")], vrf_route_create_input : VrfRouteCreateInput, **kwargs):  # noqa: E501
+    def create_vrf_route_with_http_info(self, id : Annotated[StrictStr, Field(..., description="VRF UUID")], vrf_route_create_input : VrfRouteCreateInput, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
         """Create a VRF route  # noqa: E501
 
         Create a route in a VRF. Currently only static default routes are supported.  Notice: VRFs are a test feature currently under active development, and only available to certain users. Please contact Customer Success for more information.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_vrf_route_with_http_info(id, vrf_route_create_input, async_req=True)
+        >>> thread = api.create_vrf_route_with_http_info(id, vrf_route_create_input, include, exclude, async_req=True)
         >>> result = thread.get()
 
         :param id: VRF UUID (required)
         :type id: str
         :param vrf_route_create_input: (required)
         :type vrf_route_create_input: VrfRouteCreateInput
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -283,15 +650,17 @@
         :rtype: tuple(VrfRoute, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
-            'vrf_route_create_input'
+            'vrf_route_create_input',
+            'include',
+            'exclude'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -317,14 +686,22 @@
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
 
         # process the query parameters
         _query_params = []
+        if _params.get('include') is not None:  # noqa: E501
+            _query_params.append(('include', _params['include']))
+            _collection_formats['include'] = 'csv'
+
+        if _params.get('exclude') is not None:  # noqa: E501
+            _query_params.append(('exclude', _params['exclude']))
+            _collection_formats['exclude'] = 'csv'
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
@@ -367,14 +744,175 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def delete_bgp_dynamic_neighbor_by_id(self, id : Annotated[StrictStr, Field(..., description="BGP Dynamic Neighbor UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> BgpDynamicNeighbor:  # noqa: E501
+        """Delete a VRF BGP Dynamic Neighbor  # noqa: E501
+
+        Trigger the removal of a BGP Neighbor range from a VRF  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_bgp_dynamic_neighbor_by_id(id, include, exclude, async_req=True)
+        >>> result = thread.get()
+
+        :param id: BGP Dynamic Neighbor UUID (required)
+        :type id: str
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: BgpDynamicNeighbor
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.delete_bgp_dynamic_neighbor_by_id_with_http_info(id, include, exclude, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def delete_bgp_dynamic_neighbor_by_id_with_http_info(self, id : Annotated[StrictStr, Field(..., description="BGP Dynamic Neighbor UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
+        """Delete a VRF BGP Dynamic Neighbor  # noqa: E501
+
+        Trigger the removal of a BGP Neighbor range from a VRF  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_bgp_dynamic_neighbor_by_id_with_http_info(id, include, exclude, async_req=True)
+        >>> result = thread.get()
+
+        :param id: BGP Dynamic Neighbor UUID (required)
+        :type id: str
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(BgpDynamicNeighbor, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'id',
+            'include',
+            'exclude'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method delete_bgp_dynamic_neighbor_by_id" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['id']:
+            _path_params['id'] = _params['id']
+
+
+        # process the query parameters
+        _query_params = []
+        if _params.get('include') is not None:  # noqa: E501
+            _query_params.append(('include', _params['include']))
+            _collection_formats['include'] = 'csv'
+
+        if _params.get('exclude') is not None:  # noqa: E501
+            _query_params.append(('exclude', _params['exclude']))
+            _collection_formats['exclude'] = 'csv'
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['x_auth_token']  # noqa: E501
+
+        _response_types_map = {
+            '202': "BgpDynamicNeighbor",
+            '401': "Error",
+            '403': "Error",
+            '404': "Error",
+        }
+
+        return self.api_client.call_api(
+            '/bgp-dynamic-neighbors/{id}', 'DELETE',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def delete_vrf(self, id : Annotated[StrictStr, Field(..., description="VRF UUID")], **kwargs) -> None:  # noqa: E501
         """Delete the VRF  # noqa: E501
 
         Deletes the VRF  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
@@ -1483,14 +2021,174 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def get_bgp_dynamic_neighbors(self, id : Annotated[StrictStr, Field(..., description="Metal Gateway UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> BgpDynamicNeighborList:  # noqa: E501
+        """List BGP Dynamic Neighbors  # noqa: E501
+
+        Returns the list of VRF BGP Dynamic Neighbors for this Metal Gateway  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_bgp_dynamic_neighbors(id, include, exclude, async_req=True)
+        >>> result = thread.get()
+
+        :param id: Metal Gateway UUID (required)
+        :type id: str
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: BgpDynamicNeighborList
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.get_bgp_dynamic_neighbors_with_http_info(id, include, exclude, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def get_bgp_dynamic_neighbors_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Metal Gateway UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
+        """List BGP Dynamic Neighbors  # noqa: E501
+
+        Returns the list of VRF BGP Dynamic Neighbors for this Metal Gateway  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_bgp_dynamic_neighbors_with_http_info(id, include, exclude, async_req=True)
+        >>> result = thread.get()
+
+        :param id: Metal Gateway UUID (required)
+        :type id: str
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(BgpDynamicNeighborList, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'id',
+            'include',
+            'exclude'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_bgp_dynamic_neighbors" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['id']:
+            _path_params['id'] = _params['id']
+
+
+        # process the query parameters
+        _query_params = []
+        if _params.get('include') is not None:  # noqa: E501
+            _query_params.append(('include', _params['include']))
+            _collection_formats['include'] = 'csv'
+
+        if _params.get('exclude') is not None:  # noqa: E501
+            _query_params.append(('exclude', _params['exclude']))
+            _collection_formats['exclude'] = 'csv'
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['x_auth_token']  # noqa: E501
+
+        _response_types_map = {
+            '200': "BgpDynamicNeighborList",
+            '401': "Error",
+            '404': "Error",
+        }
+
+        return self.api_client.call_api(
+            '/metal-gateways/{id}/bgp-dynamic-neighbors', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def get_vrf_routes(self, id : Annotated[StrictStr, Field(..., description="VRF UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> VrfRouteList:  # noqa: E501
         """Retrieve all routes in the VRF  # noqa: E501
 
         Returns the list of routes for the VRF  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
@@ -1802,26 +2500,28 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_vrf_route_by_id(self, id : Annotated[StrictStr, Field(..., description="VRF Route UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> VrfRoute:  # noqa: E501
+    def update_vrf_route_by_id(self, id : Annotated[StrictStr, Field(..., description="VRF Route UUID")], vrf_route_update_input : VrfRouteUpdateInput, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> VrfRoute:  # noqa: E501
         """Update a VRF Route  # noqa: E501
 
         Requests a VRF Route be redeployed across the network. Updating the prefix or next-hop address on a route is not currently supported.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_vrf_route_by_id(id, include, exclude, async_req=True)
+        >>> thread = api.update_vrf_route_by_id(id, vrf_route_update_input, include, exclude, async_req=True)
         >>> result = thread.get()
 
         :param id: VRF Route UUID (required)
         :type id: str
+        :param vrf_route_update_input: (required)
+        :type vrf_route_update_input: VrfRouteUpdateInput
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -1834,29 +2534,31 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: VrfRoute
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_vrf_route_by_id_with_http_info(id, include, exclude, **kwargs)  # noqa: E501
+        return self.update_vrf_route_by_id_with_http_info(id, vrf_route_update_input, include, exclude, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_vrf_route_by_id_with_http_info(self, id : Annotated[StrictStr, Field(..., description="VRF Route UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
+    def update_vrf_route_by_id_with_http_info(self, id : Annotated[StrictStr, Field(..., description="VRF Route UUID")], vrf_route_update_input : VrfRouteUpdateInput, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
         """Update a VRF Route  # noqa: E501
 
         Requests a VRF Route be redeployed across the network. Updating the prefix or next-hop address on a route is not currently supported.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_vrf_route_by_id_with_http_info(id, include, exclude, async_req=True)
+        >>> thread = api.update_vrf_route_by_id_with_http_info(id, vrf_route_update_input, include, exclude, async_req=True)
         >>> result = thread.get()
 
         :param id: VRF Route UUID (required)
         :type id: str
+        :param vrf_route_update_input: (required)
+        :type vrf_route_update_input: VrfRouteUpdateInput
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -1881,14 +2583,15 @@
         :rtype: tuple(VrfRoute, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'vrf_route_update_input',
             'include',
             'exclude'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -1931,18 +2634,28 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
+        if _params['vrf_route_update_input']:
+            _body_params = _params['vrf_route_update_input']
+
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
         # authentication setting
         _auth_settings = ['x_auth_token']  # noqa: E501
 
         _response_types_map = {
             '202': "VrfRoute",
             '401': "Error",
             '403': "Error",
```

### Comparing `equinix-metal-0.2.1/equinix_metal/api_client.py` & `equinix-metal-0.2.2/equinix_metal/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'metal-python/0.2.1'
+        self.user_agent = 'metal-python/0.2.2'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `equinix-metal-0.2.1/equinix_metal/configuration.py` & `equinix-metal-0.2.2/equinix_metal/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,15 +392,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 0.2.1".\
+               "SDK Package Version: 0.2.2".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `equinix-metal-0.2.1/equinix_metal/exceptions.py` & `equinix-metal-0.2.2/equinix_metal/exceptions.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/__init__.py` & `equinix-metal-0.2.2/equinix_metal/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,28 +110,32 @@
 from equinix_metal.models.interconnection_metro import InterconnectionMetro
 from equinix_metal.models.interconnection_port import InterconnectionPort
 from equinix_metal.models.interconnection_port_list import InterconnectionPortList
 from equinix_metal.models.interconnection_update_input import InterconnectionUpdateInput
 from equinix_metal.models.invitation import Invitation
 from equinix_metal.models.invitation_input import InvitationInput
 from equinix_metal.models.invitation_list import InvitationList
+from equinix_metal.models.invoice import Invoice
+from equinix_metal.models.invoice_list import InvoiceList
 from equinix_metal.models.license import License
 from equinix_metal.models.license_create_input import LicenseCreateInput
 from equinix_metal.models.license_list import LicenseList
 from equinix_metal.models.license_update_input import LicenseUpdateInput
+from equinix_metal.models.line_item import LineItem
 from equinix_metal.models.membership import Membership
 from equinix_metal.models.membership_input import MembershipInput
 from equinix_metal.models.membership_list import MembershipList
 from equinix_metal.models.meta import Meta
 from equinix_metal.models.metadata import Metadata
 from equinix_metal.models.metadata_network import MetadataNetwork
 from equinix_metal.models.metadata_network_network import MetadataNetworkNetwork
 from equinix_metal.models.metadata_network_network_bonding import MetadataNetworkNetworkBonding
 from equinix_metal.models.metal_gateway import MetalGateway
 from equinix_metal.models.metal_gateway_create_input import MetalGatewayCreateInput
+from equinix_metal.models.metal_gateway_elastic_ip_create_input import MetalGatewayElasticIpCreateInput
 from equinix_metal.models.metal_gateway_list import MetalGatewayList
 from equinix_metal.models.metal_gateway_list_metal_gateways_inner import MetalGatewayListMetalGatewaysInner
 from equinix_metal.models.metal_gateway_lite import MetalGatewayLite
 from equinix_metal.models.metro import Metro
 from equinix_metal.models.metro_capacity_list import MetroCapacityList
 from equinix_metal.models.metro_capacity_report import MetroCapacityReport
 from equinix_metal.models.metro_input import MetroInput
@@ -171,14 +175,15 @@
 from equinix_metal.models.port_vlan_assignment_batch_create_input_vlan_assignments_inner import PortVlanAssignmentBatchCreateInputVlanAssignmentsInner
 from equinix_metal.models.port_vlan_assignment_batch_list import PortVlanAssignmentBatchList
 from equinix_metal.models.port_vlan_assignment_batch_vlan_assignments_inner import PortVlanAssignmentBatchVlanAssignmentsInner
 from equinix_metal.models.port_vlan_assignment_list import PortVlanAssignmentList
 from equinix_metal.models.project import Project
 from equinix_metal.models.project_create_from_root_input import ProjectCreateFromRootInput
 from equinix_metal.models.project_create_input import ProjectCreateInput
+from equinix_metal.models.project_id_name import ProjectIdName
 from equinix_metal.models.project_list import ProjectList
 from equinix_metal.models.project_update_input import ProjectUpdateInput
 from equinix_metal.models.project_usage import ProjectUsage
 from equinix_metal.models.project_usage_list import ProjectUsageList
 from equinix_metal.models.recovery_code_list import RecoveryCodeList
 from equinix_metal.models.request_ip_reservation201_response import RequestIPReservation201Response
 from equinix_metal.models.request_ip_reservation_request import RequestIPReservationRequest
@@ -235,14 +240,12 @@
 from equinix_metal.models.vrf_ip_reservation_list import VrfIpReservationList
 from equinix_metal.models.vrf_list import VrfList
 from equinix_metal.models.vrf_metal_gateway import VrfMetalGateway
 from equinix_metal.models.vrf_metal_gateway_create_input import VrfMetalGatewayCreateInput
 from equinix_metal.models.vrf_route import VrfRoute
 from equinix_metal.models.vrf_route_create_input import VrfRouteCreateInput
 from equinix_metal.models.vrf_route_list import VrfRouteList
-from equinix_metal.models.vrf_route_metal_gateway import VrfRouteMetalGateway
-from equinix_metal.models.vrf_route_virtual_network import VrfRouteVirtualNetwork
-from equinix_metal.models.vrf_route_vrf import VrfRouteVrf
+from equinix_metal.models.vrf_route_update_input import VrfRouteUpdateInput
 from equinix_metal.models.vrf_update_input import VrfUpdateInput
 from equinix_metal.models.vrf_virtual_circuit import VrfVirtualCircuit
 from equinix_metal.models.vrf_virtual_circuit_create_input import VrfVirtualCircuitCreateInput
 from equinix_metal.models.vrf_virtual_circuit_update_input import VrfVirtualCircuitUpdateInput
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/activate_hardware_reservation_request.py` & `equinix-metal-0.2.2/equinix_metal/models/activate_hardware_reservation_request.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/address.py` & `equinix-metal-0.2.2/equinix_metal/models/address.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,22 +24,22 @@
 from pydantic import BaseModel, StrictStr
 from equinix_metal.models.coordinates import Coordinates
 
 class Address(BaseModel):
     """
     Address
     """
-    address: StrictStr = ...
+    address: Optional[StrictStr] = None
     address2: Optional[StrictStr] = None
     city: Optional[StrictStr] = None
     coordinates: Optional[Coordinates] = None
-    country: StrictStr = ...
+    country: Optional[StrictStr] = None
     href: Optional[StrictStr] = None
     state: Optional[StrictStr] = None
-    zip_code: StrictStr = ...
+    zip_code: Optional[StrictStr] = None
     __properties = ["address", "address2", "city", "coordinates", "country", "href", "state", "zip_code"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/auth_token.py` & `equinix-metal-0.2.2/equinix_metal/models/auth_token.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/auth_token_input.py` & `equinix-metal-0.2.2/equinix_metal/models/auth_token_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/auth_token_list.py` & `equinix-metal-0.2.2/equinix_metal/models/auth_token_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/auth_token_project.py` & `equinix-metal-0.2.2/equinix_metal/models/auth_token_project.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/auth_token_user.py` & `equinix-metal-0.2.2/equinix_metal/models/auth_token_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     """
     AuthTokenUser
     """
     avatar_thumb_url: Optional[StrictStr] = None
     avatar_url: Optional[StrictStr] = None
     created_at: Optional[datetime] = None
     customdata: Optional[Dict[str, Any]] = None
+    default_organization_id: Optional[StrictStr] = None
+    default_project_id: Optional[StrictStr] = None
     email: Optional[StrictStr] = None
     emails: Optional[conlist(Href)] = None
     first_name: Optional[StrictStr] = None
     fraud_score: Optional[StrictStr] = None
     full_name: Optional[StrictStr] = None
     href: Optional[StrictStr] = None
     id: Optional[StrictStr] = None
@@ -44,15 +46,15 @@
     max_organizations: Optional[StrictInt] = None
     max_projects: Optional[StrictInt] = None
     phone_number: Optional[StrictStr] = None
     short_id: Optional[StrictStr] = None
     timezone: Optional[StrictStr] = None
     two_factor_auth: Optional[StrictStr] = None
     updated_at: Optional[datetime] = None
-    __properties = ["avatar_thumb_url", "avatar_url", "created_at", "customdata", "email", "emails", "first_name", "fraud_score", "full_name", "href", "id", "last_login_at", "last_name", "max_organizations", "max_projects", "phone_number", "short_id", "timezone", "two_factor_auth", "updated_at"]
+    __properties = ["avatar_thumb_url", "avatar_url", "created_at", "customdata", "default_organization_id", "default_project_id", "email", "emails", "first_name", "fraud_score", "full_name", "href", "id", "last_login_at", "last_name", "max_organizations", "max_projects", "phone_number", "short_id", "timezone", "two_factor_auth", "updated_at"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -92,14 +94,16 @@
             return AuthTokenUser.parse_obj(obj)
 
         _obj = AuthTokenUser.parse_obj({
             "avatar_thumb_url": obj.get("avatar_thumb_url"),
             "avatar_url": obj.get("avatar_url"),
             "created_at": obj.get("created_at"),
             "customdata": obj.get("customdata"),
+            "default_organization_id": obj.get("default_organization_id"),
+            "default_project_id": obj.get("default_project_id"),
             "email": obj.get("email"),
             "emails": [Href.from_dict(_item) for _item in obj.get("emails")] if obj.get("emails") is not None else None,
             "first_name": obj.get("first_name"),
             "fraud_score": obj.get("fraud_score"),
             "full_name": obj.get("full_name"),
             "href": obj.get("href"),
             "id": obj.get("id"),
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/batch.py` & `equinix-metal-0.2.2/equinix_metal/models/batch.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/batches_list.py` & `equinix-metal-0.2.2/equinix_metal/models/batches_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/bgp_config.py` & `equinix-metal-0.2.2/equinix_metal/models/bgp_config.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/bgp_config_request_input.py` & `equinix-metal-0.2.2/equinix_metal/models/bgp_config_request_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/bgp_dynamic_neighbor.py` & `equinix-metal-0.2.2/equinix_metal/models/bgp_dynamic_neighbor.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/bgp_dynamic_neighbor_create_input.py` & `equinix-metal-0.2.2/equinix_metal/models/bgp_dynamic_neighbor_create_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr
 
 class BgpDynamicNeighborCreateInput(BaseModel):
     """
     BgpDynamicNeighborCreateInput
     """
-    bgp_neighbor_asn: Optional[StrictInt] = Field(None, description="The ASN of the dynamic BGP neighbor")
-    bgp_neighbor_range: Optional[StrictStr] = Field(None, description="Network range of the dynamic BGP neighbor in CIDR format")
+    bgp_neighbor_asn: StrictInt = Field(..., description="The ASN of the dynamic BGP neighbor")
+    bgp_neighbor_range: StrictStr = Field(..., description="Network range of the dynamic BGP neighbor in CIDR format")
     href: Optional[StrictStr] = None
     __properties = ["bgp_neighbor_asn", "bgp_neighbor_range", "href"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/bgp_dynamic_neighbor_list.py` & `equinix-metal-0.2.2/equinix_metal/models/bgp_dynamic_neighbor_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/bgp_neighbor_data.py` & `equinix-metal-0.2.2/equinix_metal/models/bgp_neighbor_data.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/bgp_route.py` & `equinix-metal-0.2.2/equinix_metal/models/bgp_route.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/bgp_session.py` & `equinix-metal-0.2.2/equinix_metal/models/bgp_session.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/bgp_session_input.py` & `equinix-metal-0.2.2/equinix_metal/models/bgp_session_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/bgp_session_list.py` & `equinix-metal-0.2.2/equinix_metal/models/bgp_session_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/bgp_session_neighbors.py` & `equinix-metal-0.2.2/equinix_metal/models/bgp_session_neighbors.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/bond_port_data.py` & `equinix-metal-0.2.2/equinix_metal/models/bond_port_data.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/capacity_check_per_facility_info.py` & `equinix-metal-0.2.2/equinix_metal/models/capacity_check_per_facility_info.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/capacity_check_per_facility_list.py` & `equinix-metal-0.2.2/equinix_metal/models/capacity_check_per_facility_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/capacity_check_per_metro_info.py` & `equinix-metal-0.2.2/equinix_metal/models/capacity_check_per_metro_info.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/capacity_check_per_metro_list.py` & `equinix-metal-0.2.2/equinix_metal/models/capacity_check_per_metro_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/capacity_input.py` & `equinix-metal-0.2.2/equinix_metal/models/capacity_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/capacity_level_per_baremetal.py` & `equinix-metal-0.2.2/equinix_metal/models/capacity_level_per_baremetal.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/capacity_list.py` & `equinix-metal-0.2.2/equinix_metal/models/capacity_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/capacity_per_facility.py` & `equinix-metal-0.2.2/equinix_metal/models/capacity_per_facility.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/capacity_per_metro_input.py` & `equinix-metal-0.2.2/equinix_metal/models/capacity_per_metro_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/capacity_per_new_facility.py` & `equinix-metal-0.2.2/equinix_metal/models/capacity_per_new_facility.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/capacity_report.py` & `equinix-metal-0.2.2/equinix_metal/models/capacity_report.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/coordinates.py` & `equinix-metal-0.2.2/equinix_metal/models/coordinates.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/create_device_request.py` & `equinix-metal-0.2.2/equinix_metal/models/create_device_request.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/create_email_input.py` & `equinix-metal-0.2.2/equinix_metal/models/create_email_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/create_metal_gateway_request.py` & `equinix-metal-0.2.2/equinix_metal/models/create_metal_gateway_request.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/create_self_service_reservation_request.py` & `equinix-metal-0.2.2/equinix_metal/models/create_self_service_reservation_request.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/create_self_service_reservation_request_period.py` & `equinix-metal-0.2.2/equinix_metal/models/create_self_service_reservation_request_period.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/device.py` & `equinix-metal-0.2.2/equinix_metal/models/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     hostname: Optional[StrictStr] = None
     href: Optional[StrictStr] = None
     id: Optional[StrictStr] = None
     image_url: Optional[StrictStr] = None
     ip_addresses: Optional[conlist(IPAssignment)] = None
     ipxe_script_url: Optional[StrictStr] = None
     iqn: Optional[StrictStr] = None
-    locked: Optional[StrictBool] = None
+    locked: Optional[StrictBool] = Field(None, description="Prevents accidental deletion of this resource when set to true.")
     metro: Optional[DeviceMetro] = None
     network_ports: Optional[conlist(Port)] = Field(None, description="By default, servers at Equinix Metal are configured in a “bonded” mode using LACP (Link Aggregation Control Protocol). Each 2-NIC server is configured with a single bond (namely bond0) with both interfaces eth0 and eth1 as members of the bond in a default Layer 3 mode. Some device plans may have a different number of ports and bonds available.")
     operating_system: Optional[OperatingSystem] = None
     plan: Optional[Plan] = None
     project: Optional[DeviceProject] = None
     project_lite: Optional[DeviceProjectLite] = None
     provisioning_events: Optional[conlist(Event)] = None
@@ -70,15 +70,15 @@
     sos: Optional[StrictStr] = Field(None, description="Hostname used to connect to the instance via the SOS (Serial over SSH) out-of-band console.")
     spot_instance: Optional[StrictBool] = Field(None, description="Whether or not the device is a spot instance.")
     spot_price_max: Optional[StrictFloat] = Field(None, description="The maximum price per hour you are willing to pay to keep this spot instance.  If you are outbid, the termination will be set allowing two minutes before shutdown.")
     ssh_keys: Optional[conlist(Href)] = None
     state: Optional[StrictStr] = None
     switch_uuid: Optional[StrictStr] = Field(None, description="Switch short id. This can be used to determine if two devices are connected to the same switch, for example.")
     tags: Optional[conlist(StrictStr)] = None
-    termination_time: Optional[datetime] = Field(None, description="When the device will be terminated. This is commonly set in advance for ephemeral spot market instances but this field may also be set with on-demand and reservation instances to automatically delete the resource at a given time. The termination time can also be used to release a hardware reservation instance at a given time, keeping the reservation open for other uses.  On a spot market device, the termination time will be set automatically when outbid.")
+    termination_time: Optional[datetime] = Field(None, description="When the device will be terminated. If you don't supply timezone info, the timestamp is assumed to be in UTC.  This is commonly set in advance for ephemeral spot market instances but this field may also be set with on-demand and reservation instances to automatically delete the resource at a given time. The termination time can also be used to release a hardware reservation instance at a given time, keeping the reservation open for other uses.  On a spot market device, the termination time will be set automatically when outbid.")
     updated_at: Optional[datetime] = None
     user: Optional[StrictStr] = None
     userdata: Optional[StrictStr] = None
     volumes: Optional[conlist(Href)] = None
     __properties = ["actions", "always_pxe", "billing_cycle", "bonding_mode", "created_at", "created_by", "customdata", "description", "facility", "hardware_reservation", "hostname", "href", "id", "image_url", "ip_addresses", "ipxe_script_url", "iqn", "locked", "metro", "network_ports", "operating_system", "plan", "project", "project_lite", "provisioning_events", "provisioning_percentage", "root_password", "short_id", "sos", "spot_instance", "spot_price_max", "ssh_keys", "state", "switch_uuid", "tags", "termination_time", "updated_at", "user", "userdata", "volumes"]
 
     @validator('state')
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/device_action_input.py` & `equinix-metal-0.2.2/equinix_metal/models/device_action_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/device_actions_inner.py` & `equinix-metal-0.2.2/equinix_metal/models/device_actions_inner.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/device_create_in_facility_input.py` & `equinix-metal-0.2.2/equinix_metal/models/device_create_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,48 +18,46 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, StrictStr, conlist, validator
-from equinix_metal.models.facility_input_facility import FacilityInputFacility
 from equinix_metal.models.ip_address import IPAddress
 from equinix_metal.models.ssh_key_input import SSHKeyInput
 
-class DeviceCreateInFacilityInput(BaseModel):
+class DeviceCreateInput(BaseModel):
     """
-    DeviceCreateInFacilityInput
+    DeviceCreateInput
     """
-    facility: FacilityInputFacility = ...
-    href: Optional[StrictStr] = None
     always_pxe: Optional[StrictBool] = Field(None, description="When true, devices with a `custom_ipxe` OS will always boot to iPXE. The default setting of false ensures that iPXE will be used on only the first boot.")
     billing_cycle: Optional[StrictStr] = Field(None, description="The billing cycle of the device.")
     customdata: Optional[Dict[str, Any]] = Field(None, description="Customdata is an arbitrary JSON value that can be accessed via the metadata service.")
     description: Optional[StrictStr] = Field(None, description="Any description of the device or how it will be used. This may be used to inform other API consumers with project access.")
     features: Optional[conlist(StrictStr)] = Field(None, description="The features attribute allows you to optionally specify what features your server should have.  In the API shorthand syntax, all features listed are `required`:  ``` { \"features\": [\"tpm\"] } ```  Alternatively, if you do not require a certain feature, but would prefer to be assigned a server with that feature if there are any available, you may specify that feature with a `preferred` value. The request will not fail if we have no servers with that feature in our inventory. The API offers an alternative syntax for mixing preferred and required features:  ``` { \"features\": { \"tpm\": \"required\", \"raid\": \"preferred\" } } ```  The request will only fail if there are no available servers matching the required `tpm` criteria.")
     hardware_reservation_id: Optional[StrictStr] = Field(None, description="The Hardware Reservation UUID to provision. Alternatively, `next-available` can be specified to select from any of the available hardware reservations. An error will be returned if the requested reservation option is not available.  See [Reserved Hardware](https://metal.equinix.com/developers/docs/deploy/reserved/) for more details.")
     hostname: Optional[StrictStr] = Field(None, description="The hostname to use within the operating system. The same hostname may be used on multiple devices within a project.")
+    href: Optional[StrictStr] = None
     ip_addresses: Optional[conlist(IPAddress)] = Field(None, description="The `ip_addresses attribute will allow you to specify the addresses you want created with your device.  The default value configures public IPv4, public IPv6, and private IPv4.  Private IPv4 address is required. When specifying `ip_addresses`, one of the array items must enable private IPv4.  Some operating systems require public IPv4 address. In those cases you will receive an error message if public IPv4 is not enabled.  For example, to only configure your server with a private IPv4 address, you can send `{ \"ip_addresses\": [{ \"address_family\": 4, \"public\": false }] }`.  It is possible to request a subnet size larger than a `/30` by assigning addresses using the UUID(s) of ip_reservations in your project.  For example, `{ \"ip_addresses\": [..., {\"address_family\": 4, \"public\": true, \"ip_reservations\": [\"uuid1\", \"uuid2\"]}] }`  To access a server without public IPs, you can use our Out-of-Band console access (SOS) or proxy through another server in the project with public IPs enabled.")
     ipxe_script_url: Optional[StrictStr] = Field(None, description="When set, the device will chainload an iPXE Script at boot fetched from the supplied URL.  See [Custom iPXE](https://metal.equinix.com/developers/docs/operating-systems/custom-ipxe/) for more details.")
     locked: Optional[StrictBool] = Field(False, description="Whether the device should be locked, preventing accidental deletion.")
     no_ssh_keys: Optional[StrictBool] = Field(False, description="Overrides default behaviour of attaching all of the organization members ssh keys and project ssh keys to device if no specific keys specified")
     operating_system: StrictStr = Field(..., description="The slug of the operating system to provision. Check the Equinix Metal operating system documentation for rules that may be imposed per operating system, including restrictions on IP address options and device plans.")
     plan: StrictStr = Field(..., description="The slug of the device plan to provision.")
     private_ipv4_subnet_size: Optional[StrictInt] = Field(28, description="Deprecated. Use ip_addresses. Subnet range for addresses allocated to this device.")
     project_ssh_keys: Optional[conlist(StrictStr)] = Field(None, description="A list of UUIDs identifying the device parent project that should be authorized to access this device (typically via /root/.ssh/authorized_keys). These keys will also appear in the device metadata.  If no SSH keys are specified (`user_ssh_keys`, `project_ssh_keys`, and `ssh_keys` are all empty lists or omitted), all parent project keys, parent project members keys and organization members keys will be included. This behaviour can be changed with 'no_ssh_keys' option to omit any SSH key being added. ")
     public_ipv4_subnet_size: Optional[StrictInt] = Field(31, description="Deprecated. Use ip_addresses. Subnet range for addresses allocated to this device. Your project must have addresses available for a non-default request.")
     spot_instance: Optional[StrictBool] = Field(None, description="Create a spot instance. Spot instances are created with a maximum bid price. If the bid price is not met, the spot instance will be terminated as indicated by the `termination_time` field.")
     spot_price_max: Optional[StrictFloat] = Field(None, description="The maximum amount to bid for a spot instance.")
     ssh_keys: Optional[conlist(SSHKeyInput)] = Field(None, description="A list of new or existing project ssh_keys that should be authorized to access this device (typically via /root/.ssh/authorized_keys). These keys will also appear in the device metadata.  These keys are added in addition to any keys defined by   `project_ssh_keys` and `user_ssh_keys`. ")
     tags: Optional[conlist(StrictStr)] = None
-    termination_time: Optional[datetime] = None
+    termination_time: Optional[datetime] = Field(None, description="When the device will be terminated. If you don't supply timezone info, the timestamp is assumed to be in UTC.  This is commonly set in advance for ephemeral spot market instances but this field may also be set with on-demand and reservation instances to automatically delete the resource at a given time. The termination time can also be used to release a hardware reservation instance at a given time, keeping the reservation open for other uses.  On a spot market device, the termination time will be set automatically when outbid. ")
     user_ssh_keys: Optional[conlist(StrictStr)] = Field(None, description="A list of UUIDs identifying the users that should be authorized to access this device (typically via /root/.ssh/authorized_keys).  These keys will also appear in the device metadata.  The users must be members of the project or organization.  If no SSH keys are specified (`user_ssh_keys`, `project_ssh_keys`, and `ssh_keys` are all empty lists or omitted), all parent project keys, parent project members keys and organization members keys will be included. This behaviour can be changed with 'no_ssh_keys' option to omit any SSH key being added. ")
     userdata: Optional[StrictStr] = Field(None, description="The userdata presented in the metadata service for this device.  Userdata is fetched and interpreted by the operating system installed on the device. Acceptable formats are determined by the operating system, with the exception of a special iPXE enabling syntax which is handled before the operating system starts.  See [Server User Data](https://metal.equinix.com/developers/docs/servers/user-data/) and [Provisioning with Custom iPXE](https://metal.equinix.com/developers/docs/operating-systems/custom-ipxe/#provisioning-with-custom-ipxe) for more details.")
-    __properties = ["facility", "href", "always_pxe", "billing_cycle", "customdata", "description", "features", "hardware_reservation_id", "hostname", "ip_addresses", "ipxe_script_url", "locked", "no_ssh_keys", "operating_system", "plan", "private_ipv4_subnet_size", "project_ssh_keys", "public_ipv4_subnet_size", "spot_instance", "spot_price_max", "ssh_keys", "tags", "termination_time", "user_ssh_keys", "userdata"]
+    __properties = ["always_pxe", "billing_cycle", "customdata", "description", "features", "hardware_reservation_id", "hostname", "href", "ip_addresses", "ipxe_script_url", "locked", "no_ssh_keys", "operating_system", "plan", "private_ipv4_subnet_size", "project_ssh_keys", "public_ipv4_subnet_size", "spot_instance", "spot_price_max", "ssh_keys", "tags", "termination_time", "user_ssh_keys", "userdata"]
 
     @validator('billing_cycle')
     def billing_cycle_validate_enum(cls, v):
         if v is None:
             return v
         if v not in ('hourly', 'daily', 'monthly', 'yearly'):
             raise ValueError("must be one of enum values ('hourly', 'daily', 'monthly', 'yearly')")
@@ -74,27 +72,24 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> DeviceCreateInFacilityInput:
-        """Create an instance of DeviceCreateInFacilityInput from a JSON string"""
+    def from_json(cls, json_str: str) -> DeviceCreateInput:
+        """Create an instance of DeviceCreateInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of facility
-        if self.facility:
-            _dict['facility'] = self.facility.to_dict()
         # override the default output from pydantic by calling `to_dict()` of each item in ip_addresses (list)
         _items = []
         if self.ip_addresses:
             for _item in self.ip_addresses:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['ip_addresses'] = _items
@@ -104,32 +99,31 @@
             for _item in self.ssh_keys:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['ssh_keys'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> DeviceCreateInFacilityInput:
-        """Create an instance of DeviceCreateInFacilityInput from a dict"""
+    def from_dict(cls, obj: dict) -> DeviceCreateInput:
+        """Create an instance of DeviceCreateInput from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return DeviceCreateInFacilityInput.parse_obj(obj)
+            return DeviceCreateInput.parse_obj(obj)
 
-        _obj = DeviceCreateInFacilityInput.parse_obj({
-            "facility": FacilityInputFacility.from_dict(obj.get("facility")) if obj.get("facility") is not None else None,
-            "href": obj.get("href"),
+        _obj = DeviceCreateInput.parse_obj({
             "always_pxe": obj.get("always_pxe"),
             "billing_cycle": obj.get("billing_cycle"),
             "customdata": obj.get("customdata"),
             "description": obj.get("description"),
             "features": obj.get("features"),
             "hardware_reservation_id": obj.get("hardware_reservation_id"),
             "hostname": obj.get("hostname"),
+            "href": obj.get("href"),
             "ip_addresses": [IPAddress.from_dict(_item) for _item in obj.get("ip_addresses")] if obj.get("ip_addresses") is not None else None,
             "ipxe_script_url": obj.get("ipxe_script_url"),
             "locked": obj.get("locked") if obj.get("locked") is not None else False,
             "no_ssh_keys": obj.get("no_ssh_keys") if obj.get("no_ssh_keys") is not None else False,
             "operating_system": obj.get("operating_system"),
             "plan": obj.get("plan"),
             "private_ipv4_subnet_size": obj.get("private_ipv4_subnet_size") if obj.get("private_ipv4_subnet_size") is not None else 28,
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/device_create_in_metro_input.py` & `equinix-metal-0.2.2/equinix_metal/models/device_create_in_metro_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     private_ipv4_subnet_size: Optional[StrictInt] = Field(28, description="Deprecated. Use ip_addresses. Subnet range for addresses allocated to this device.")
     project_ssh_keys: Optional[conlist(StrictStr)] = Field(None, description="A list of UUIDs identifying the device parent project that should be authorized to access this device (typically via /root/.ssh/authorized_keys). These keys will also appear in the device metadata.  If no SSH keys are specified (`user_ssh_keys`, `project_ssh_keys`, and `ssh_keys` are all empty lists or omitted), all parent project keys, parent project members keys and organization members keys will be included. This behaviour can be changed with 'no_ssh_keys' option to omit any SSH key being added. ")
     public_ipv4_subnet_size: Optional[StrictInt] = Field(31, description="Deprecated. Use ip_addresses. Subnet range for addresses allocated to this device. Your project must have addresses available for a non-default request.")
     spot_instance: Optional[StrictBool] = Field(None, description="Create a spot instance. Spot instances are created with a maximum bid price. If the bid price is not met, the spot instance will be terminated as indicated by the `termination_time` field.")
     spot_price_max: Optional[StrictFloat] = Field(None, description="The maximum amount to bid for a spot instance.")
     ssh_keys: Optional[conlist(SSHKeyInput)] = Field(None, description="A list of new or existing project ssh_keys that should be authorized to access this device (typically via /root/.ssh/authorized_keys). These keys will also appear in the device metadata.  These keys are added in addition to any keys defined by   `project_ssh_keys` and `user_ssh_keys`. ")
     tags: Optional[conlist(StrictStr)] = None
-    termination_time: Optional[datetime] = None
+    termination_time: Optional[datetime] = Field(None, description="When the device will be terminated. If you don't supply timezone info, the timestamp is assumed to be in UTC.  This is commonly set in advance for ephemeral spot market instances but this field may also be set with on-demand and reservation instances to automatically delete the resource at a given time. The termination time can also be used to release a hardware reservation instance at a given time, keeping the reservation open for other uses.  On a spot market device, the termination time will be set automatically when outbid. ")
     user_ssh_keys: Optional[conlist(StrictStr)] = Field(None, description="A list of UUIDs identifying the users that should be authorized to access this device (typically via /root/.ssh/authorized_keys).  These keys will also appear in the device metadata.  The users must be members of the project or organization.  If no SSH keys are specified (`user_ssh_keys`, `project_ssh_keys`, and `ssh_keys` are all empty lists or omitted), all parent project keys, parent project members keys and organization members keys will be included. This behaviour can be changed with 'no_ssh_keys' option to omit any SSH key being added. ")
     userdata: Optional[StrictStr] = Field(None, description="The userdata presented in the metadata service for this device.  Userdata is fetched and interpreted by the operating system installed on the device. Acceptable formats are determined by the operating system, with the exception of a special iPXE enabling syntax which is handled before the operating system starts.  See [Server User Data](https://metal.equinix.com/developers/docs/servers/user-data/) and [Provisioning with Custom iPXE](https://metal.equinix.com/developers/docs/operating-systems/custom-ipxe/#provisioning-with-custom-ipxe) for more details.")
     __properties = ["href", "metro", "always_pxe", "billing_cycle", "customdata", "description", "features", "hardware_reservation_id", "hostname", "ip_addresses", "ipxe_script_url", "locked", "no_ssh_keys", "operating_system", "plan", "private_ipv4_subnet_size", "project_ssh_keys", "public_ipv4_subnet_size", "spot_instance", "spot_price_max", "ssh_keys", "tags", "termination_time", "user_ssh_keys", "userdata"]
 
     @validator('billing_cycle')
     def billing_cycle_validate_enum(cls, v):
         if v is None:
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/device_create_input.py` & `equinix-metal-0.2.2/equinix_metal/models/device_create_in_facility_input.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,46 +18,48 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, StrictStr, conlist, validator
+from equinix_metal.models.facility_input_facility import FacilityInputFacility
 from equinix_metal.models.ip_address import IPAddress
 from equinix_metal.models.ssh_key_input import SSHKeyInput
 
-class DeviceCreateInput(BaseModel):
+class DeviceCreateInFacilityInput(BaseModel):
     """
-    DeviceCreateInput
+    DeviceCreateInFacilityInput
     """
+    facility: FacilityInputFacility = ...
+    href: Optional[StrictStr] = None
     always_pxe: Optional[StrictBool] = Field(None, description="When true, devices with a `custom_ipxe` OS will always boot to iPXE. The default setting of false ensures that iPXE will be used on only the first boot.")
     billing_cycle: Optional[StrictStr] = Field(None, description="The billing cycle of the device.")
     customdata: Optional[Dict[str, Any]] = Field(None, description="Customdata is an arbitrary JSON value that can be accessed via the metadata service.")
     description: Optional[StrictStr] = Field(None, description="Any description of the device or how it will be used. This may be used to inform other API consumers with project access.")
     features: Optional[conlist(StrictStr)] = Field(None, description="The features attribute allows you to optionally specify what features your server should have.  In the API shorthand syntax, all features listed are `required`:  ``` { \"features\": [\"tpm\"] } ```  Alternatively, if you do not require a certain feature, but would prefer to be assigned a server with that feature if there are any available, you may specify that feature with a `preferred` value. The request will not fail if we have no servers with that feature in our inventory. The API offers an alternative syntax for mixing preferred and required features:  ``` { \"features\": { \"tpm\": \"required\", \"raid\": \"preferred\" } } ```  The request will only fail if there are no available servers matching the required `tpm` criteria.")
     hardware_reservation_id: Optional[StrictStr] = Field(None, description="The Hardware Reservation UUID to provision. Alternatively, `next-available` can be specified to select from any of the available hardware reservations. An error will be returned if the requested reservation option is not available.  See [Reserved Hardware](https://metal.equinix.com/developers/docs/deploy/reserved/) for more details.")
     hostname: Optional[StrictStr] = Field(None, description="The hostname to use within the operating system. The same hostname may be used on multiple devices within a project.")
-    href: Optional[StrictStr] = None
     ip_addresses: Optional[conlist(IPAddress)] = Field(None, description="The `ip_addresses attribute will allow you to specify the addresses you want created with your device.  The default value configures public IPv4, public IPv6, and private IPv4.  Private IPv4 address is required. When specifying `ip_addresses`, one of the array items must enable private IPv4.  Some operating systems require public IPv4 address. In those cases you will receive an error message if public IPv4 is not enabled.  For example, to only configure your server with a private IPv4 address, you can send `{ \"ip_addresses\": [{ \"address_family\": 4, \"public\": false }] }`.  It is possible to request a subnet size larger than a `/30` by assigning addresses using the UUID(s) of ip_reservations in your project.  For example, `{ \"ip_addresses\": [..., {\"address_family\": 4, \"public\": true, \"ip_reservations\": [\"uuid1\", \"uuid2\"]}] }`  To access a server without public IPs, you can use our Out-of-Band console access (SOS) or proxy through another server in the project with public IPs enabled.")
     ipxe_script_url: Optional[StrictStr] = Field(None, description="When set, the device will chainload an iPXE Script at boot fetched from the supplied URL.  See [Custom iPXE](https://metal.equinix.com/developers/docs/operating-systems/custom-ipxe/) for more details.")
     locked: Optional[StrictBool] = Field(False, description="Whether the device should be locked, preventing accidental deletion.")
     no_ssh_keys: Optional[StrictBool] = Field(False, description="Overrides default behaviour of attaching all of the organization members ssh keys and project ssh keys to device if no specific keys specified")
     operating_system: StrictStr = Field(..., description="The slug of the operating system to provision. Check the Equinix Metal operating system documentation for rules that may be imposed per operating system, including restrictions on IP address options and device plans.")
     plan: StrictStr = Field(..., description="The slug of the device plan to provision.")
     private_ipv4_subnet_size: Optional[StrictInt] = Field(28, description="Deprecated. Use ip_addresses. Subnet range for addresses allocated to this device.")
     project_ssh_keys: Optional[conlist(StrictStr)] = Field(None, description="A list of UUIDs identifying the device parent project that should be authorized to access this device (typically via /root/.ssh/authorized_keys). These keys will also appear in the device metadata.  If no SSH keys are specified (`user_ssh_keys`, `project_ssh_keys`, and `ssh_keys` are all empty lists or omitted), all parent project keys, parent project members keys and organization members keys will be included. This behaviour can be changed with 'no_ssh_keys' option to omit any SSH key being added. ")
     public_ipv4_subnet_size: Optional[StrictInt] = Field(31, description="Deprecated. Use ip_addresses. Subnet range for addresses allocated to this device. Your project must have addresses available for a non-default request.")
     spot_instance: Optional[StrictBool] = Field(None, description="Create a spot instance. Spot instances are created with a maximum bid price. If the bid price is not met, the spot instance will be terminated as indicated by the `termination_time` field.")
     spot_price_max: Optional[StrictFloat] = Field(None, description="The maximum amount to bid for a spot instance.")
     ssh_keys: Optional[conlist(SSHKeyInput)] = Field(None, description="A list of new or existing project ssh_keys that should be authorized to access this device (typically via /root/.ssh/authorized_keys). These keys will also appear in the device metadata.  These keys are added in addition to any keys defined by   `project_ssh_keys` and `user_ssh_keys`. ")
     tags: Optional[conlist(StrictStr)] = None
-    termination_time: Optional[datetime] = None
+    termination_time: Optional[datetime] = Field(None, description="When the device will be terminated. If you don't supply timezone info, the timestamp is assumed to be in UTC.  This is commonly set in advance for ephemeral spot market instances but this field may also be set with on-demand and reservation instances to automatically delete the resource at a given time. The termination time can also be used to release a hardware reservation instance at a given time, keeping the reservation open for other uses.  On a spot market device, the termination time will be set automatically when outbid. ")
     user_ssh_keys: Optional[conlist(StrictStr)] = Field(None, description="A list of UUIDs identifying the users that should be authorized to access this device (typically via /root/.ssh/authorized_keys).  These keys will also appear in the device metadata.  The users must be members of the project or organization.  If no SSH keys are specified (`user_ssh_keys`, `project_ssh_keys`, and `ssh_keys` are all empty lists or omitted), all parent project keys, parent project members keys and organization members keys will be included. This behaviour can be changed with 'no_ssh_keys' option to omit any SSH key being added. ")
     userdata: Optional[StrictStr] = Field(None, description="The userdata presented in the metadata service for this device.  Userdata is fetched and interpreted by the operating system installed on the device. Acceptable formats are determined by the operating system, with the exception of a special iPXE enabling syntax which is handled before the operating system starts.  See [Server User Data](https://metal.equinix.com/developers/docs/servers/user-data/) and [Provisioning with Custom iPXE](https://metal.equinix.com/developers/docs/operating-systems/custom-ipxe/#provisioning-with-custom-ipxe) for more details.")
-    __properties = ["always_pxe", "billing_cycle", "customdata", "description", "features", "hardware_reservation_id", "hostname", "href", "ip_addresses", "ipxe_script_url", "locked", "no_ssh_keys", "operating_system", "plan", "private_ipv4_subnet_size", "project_ssh_keys", "public_ipv4_subnet_size", "spot_instance", "spot_price_max", "ssh_keys", "tags", "termination_time", "user_ssh_keys", "userdata"]
+    __properties = ["facility", "href", "always_pxe", "billing_cycle", "customdata", "description", "features", "hardware_reservation_id", "hostname", "ip_addresses", "ipxe_script_url", "locked", "no_ssh_keys", "operating_system", "plan", "private_ipv4_subnet_size", "project_ssh_keys", "public_ipv4_subnet_size", "spot_instance", "spot_price_max", "ssh_keys", "tags", "termination_time", "user_ssh_keys", "userdata"]
 
     @validator('billing_cycle')
     def billing_cycle_validate_enum(cls, v):
         if v is None:
             return v
         if v not in ('hourly', 'daily', 'monthly', 'yearly'):
             raise ValueError("must be one of enum values ('hourly', 'daily', 'monthly', 'yearly')")
@@ -72,24 +74,27 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> DeviceCreateInput:
-        """Create an instance of DeviceCreateInput from a JSON string"""
+    def from_json(cls, json_str: str) -> DeviceCreateInFacilityInput:
+        """Create an instance of DeviceCreateInFacilityInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of facility
+        if self.facility:
+            _dict['facility'] = self.facility.to_dict()
         # override the default output from pydantic by calling `to_dict()` of each item in ip_addresses (list)
         _items = []
         if self.ip_addresses:
             for _item in self.ip_addresses:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['ip_addresses'] = _items
@@ -99,31 +104,32 @@
             for _item in self.ssh_keys:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['ssh_keys'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> DeviceCreateInput:
-        """Create an instance of DeviceCreateInput from a dict"""
+    def from_dict(cls, obj: dict) -> DeviceCreateInFacilityInput:
+        """Create an instance of DeviceCreateInFacilityInput from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return DeviceCreateInput.parse_obj(obj)
+            return DeviceCreateInFacilityInput.parse_obj(obj)
 
-        _obj = DeviceCreateInput.parse_obj({
+        _obj = DeviceCreateInFacilityInput.parse_obj({
+            "facility": FacilityInputFacility.from_dict(obj.get("facility")) if obj.get("facility") is not None else None,
+            "href": obj.get("href"),
             "always_pxe": obj.get("always_pxe"),
             "billing_cycle": obj.get("billing_cycle"),
             "customdata": obj.get("customdata"),
             "description": obj.get("description"),
             "features": obj.get("features"),
             "hardware_reservation_id": obj.get("hardware_reservation_id"),
             "hostname": obj.get("hostname"),
-            "href": obj.get("href"),
             "ip_addresses": [IPAddress.from_dict(_item) for _item in obj.get("ip_addresses")] if obj.get("ip_addresses") is not None else None,
             "ipxe_script_url": obj.get("ipxe_script_url"),
             "locked": obj.get("locked") if obj.get("locked") is not None else False,
             "no_ssh_keys": obj.get("no_ssh_keys") if obj.get("no_ssh_keys") is not None else False,
             "operating_system": obj.get("operating_system"),
             "plan": obj.get("plan"),
             "private_ipv4_subnet_size": obj.get("private_ipv4_subnet_size") if obj.get("private_ipv4_subnet_size") is not None else 28,
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/device_created_by.py` & `equinix-metal-0.2.2/equinix_metal/models/device_created_by.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/device_list.py` & `equinix-metal-0.2.2/equinix_metal/models/device_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/device_metro.py` & `equinix-metal-0.2.2/equinix_metal/models/device_metro.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/device_project.py` & `equinix-metal-0.2.2/equinix_metal/models/device_project.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/device_project_lite.py` & `equinix-metal-0.2.2/equinix_metal/models/device_project_lite.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/device_update_input.py` & `equinix-metal-0.2.2/equinix_metal/models/device_update_input.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     always_pxe: Optional[StrictBool] = None
     billing_cycle: Optional[StrictStr] = None
     customdata: Optional[Dict[str, Any]] = None
     description: Optional[StrictStr] = None
     hostname: Optional[StrictStr] = None
     href: Optional[StrictStr] = None
     ipxe_script_url: Optional[StrictStr] = None
-    locked: Optional[StrictBool] = None
+    locked: Optional[StrictBool] = Field(None, description="Whether the device should be locked, preventing accidental deletion.")
     network_frozen: Optional[StrictBool] = Field(None, description="If true, this instance can not be converted to a different network type.")
     spot_instance: Optional[StrictBool] = Field(None, description="Can be set to false to convert a spot-market instance to on-demand.")
     tags: Optional[conlist(StrictStr)] = None
     userdata: Optional[StrictStr] = None
     __properties = ["always_pxe", "billing_cycle", "customdata", "description", "hostname", "href", "ipxe_script_url", "locked", "network_frozen", "spot_instance", "tags", "userdata"]
 
     class Config:
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/device_usage.py` & `equinix-metal-0.2.2/equinix_metal/models/device_usage.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/device_usage_list.py` & `equinix-metal-0.2.2/equinix_metal/models/device_usage_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/email.py` & `equinix-metal-0.2.2/equinix_metal/models/email.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/email_input.py` & `equinix-metal-0.2.2/equinix_metal/models/email_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/entitlement.py` & `equinix-metal-0.2.2/equinix_metal/models/entitlement.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/error.py` & `equinix-metal-0.2.2/equinix_metal/models/error.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/event.py` & `equinix-metal-0.2.2/equinix_metal/models/event.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/event_list.py` & `equinix-metal-0.2.2/equinix_metal/models/event_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/fabric_service_token.py` & `equinix-metal-0.2.2/equinix_metal/models/fabric_service_token.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/facility.py` & `equinix-metal-0.2.2/equinix_metal/models/facility.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/facility_input.py` & `equinix-metal-0.2.2/equinix_metal/models/facility_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/facility_input_facility.py` & `equinix-metal-0.2.2/equinix_metal/models/facility_input_facility.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/facility_list.py` & `equinix-metal-0.2.2/equinix_metal/models/facility_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/find_ip_address_by_id200_response.py` & `equinix-metal-0.2.2/equinix_metal/models/find_ip_address_by_id200_response.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/find_metal_gateway_by_id200_response.py` & `equinix-metal-0.2.2/equinix_metal/models/find_metal_gateway_by_id200_response.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/find_traffic_timeframe_parameter.py` & `equinix-metal-0.2.2/equinix_metal/models/find_traffic_timeframe_parameter.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/global_bgp_range.py` & `equinix-metal-0.2.2/equinix_metal/models/global_bgp_range.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/global_bgp_range_list.py` & `equinix-metal-0.2.2/equinix_metal/models/global_bgp_range_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/hardware_reservation.py` & `equinix-metal-0.2.2/equinix_metal/models/hardware_reservation.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/hardware_reservation_list.py` & `equinix-metal-0.2.2/equinix_metal/models/hardware_reservation_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/href.py` & `equinix-metal-0.2.2/equinix_metal/models/href.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/instances_batch_create_input.py` & `equinix-metal-0.2.2/equinix_metal/models/instances_batch_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/instances_batch_create_input_batches_inner.py` & `equinix-metal-0.2.2/equinix_metal/models/instances_batch_create_input_batches_inner.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     private_ipv4_subnet_size: Optional[StrictInt] = Field(28, description="Deprecated. Use ip_addresses. Subnet range for addresses allocated to this device.")
     project_ssh_keys: Optional[conlist(StrictStr)] = Field(None, description="A list of UUIDs identifying the device parent project that should be authorized to access this device (typically via /root/.ssh/authorized_keys). These keys will also appear in the device metadata.  If no SSH keys are specified (`user_ssh_keys`, `project_ssh_keys`, and `ssh_keys` are all empty lists or omitted), all parent project keys, parent project members keys and organization members keys will be included. This behaviour can be changed with 'no_ssh_keys' option to omit any SSH key being added. ")
     public_ipv4_subnet_size: Optional[StrictInt] = Field(31, description="Deprecated. Use ip_addresses. Subnet range for addresses allocated to this device. Your project must have addresses available for a non-default request.")
     spot_instance: Optional[StrictBool] = Field(None, description="Create a spot instance. Spot instances are created with a maximum bid price. If the bid price is not met, the spot instance will be terminated as indicated by the `termination_time` field.")
     spot_price_max: Optional[StrictFloat] = Field(None, description="The maximum amount to bid for a spot instance.")
     ssh_keys: Optional[conlist(SSHKeyInput)] = Field(None, description="A list of new or existing project ssh_keys that should be authorized to access this device (typically via /root/.ssh/authorized_keys). These keys will also appear in the device metadata.  These keys are added in addition to any keys defined by   `project_ssh_keys` and `user_ssh_keys`. ")
     tags: Optional[conlist(StrictStr)] = None
-    termination_time: Optional[datetime] = None
+    termination_time: Optional[datetime] = Field(None, description="When the device will be terminated. If you don't supply timezone info, the timestamp is assumed to be in UTC.  This is commonly set in advance for ephemeral spot market instances but this field may also be set with on-demand and reservation instances to automatically delete the resource at a given time. The termination time can also be used to release a hardware reservation instance at a given time, keeping the reservation open for other uses.  On a spot market device, the termination time will be set automatically when outbid. ")
     user_ssh_keys: Optional[conlist(StrictStr)] = Field(None, description="A list of UUIDs identifying the users that should be authorized to access this device (typically via /root/.ssh/authorized_keys).  These keys will also appear in the device metadata.  The users must be members of the project or organization.  If no SSH keys are specified (`user_ssh_keys`, `project_ssh_keys`, and `ssh_keys` are all empty lists or omitted), all parent project keys, parent project members keys and organization members keys will be included. This behaviour can be changed with 'no_ssh_keys' option to omit any SSH key being added. ")
     userdata: Optional[StrictStr] = Field(None, description="The userdata presented in the metadata service for this device.  Userdata is fetched and interpreted by the operating system installed on the device. Acceptable formats are determined by the operating system, with the exception of a special iPXE enabling syntax which is handled before the operating system starts.  See [Server User Data](https://metal.equinix.com/developers/docs/servers/user-data/) and [Provisioning with Custom iPXE](https://metal.equinix.com/developers/docs/operating-systems/custom-ipxe/#provisioning-with-custom-ipxe) for more details.")
     facility: FacilityInputFacility = ...
     __properties = ["hostnames", "href", "quantity", "metro", "always_pxe", "billing_cycle", "customdata", "description", "features", "hardware_reservation_id", "hostname", "ip_addresses", "ipxe_script_url", "locked", "no_ssh_keys", "operating_system", "plan", "private_ipv4_subnet_size", "project_ssh_keys", "public_ipv4_subnet_size", "spot_instance", "spot_price_max", "ssh_keys", "tags", "termination_time", "user_ssh_keys", "userdata", "facility"]
 
     @validator('billing_cycle')
     def billing_cycle_validate_enum(cls, v):
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/instances_batch_create_input_batches_inner_all_of.py` & `equinix-metal-0.2.2/equinix_metal/models/instances_batch_create_input_batches_inner_all_of.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/interconnection.py` & `equinix-metal-0.2.2/equinix_metal/models/interconnection.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/interconnection_create_input.py` & `equinix-metal-0.2.2/equinix_metal/models/interconnection_create_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr, conlist, validator
 
 class InterconnectionCreateInput(BaseModel):
     """
     InterconnectionCreateInput
     """
-    contact_email: Optional[StrictStr] = None
+    contact_email: Optional[StrictStr] = Field(None, description="The preferred email used for communication and notifications about the Equinix Fabric interconnection. Required when using a Project API key. Optional and defaults to the primary user email address when using a User API key.")
     description: Optional[StrictStr] = None
     href: Optional[StrictStr] = None
     metro: StrictStr = Field(..., description="A Metro ID or code. For interconnections with Dedicated Ports, this will be the location of the issued Dedicated Ports. When creating Fabric VCs (Metal Billed), this is where interconnection will be originating from, as we pre-authorize the use of one of our shared ports as the origin of the interconnection using A-Side service tokens. We only allow local connections for Fabric VCs (Metal Billed), so the destination location must be the same as the origin. For Fabric VCs (Fabric Billed), or shared connections, this will be the destination of the interconnection. We allow remote connections for Fabric VCs (Fabric Billed), so the origin of the interconnection can be a different metro set here.")
     mode: Optional[StrictStr] = Field(None, description="The mode of the interconnection (only relevant to Dedicated Ports). Fabric VCs won't have this field. Can be either 'standard' or 'tunnel'.   The default mode of an interconnection on a Dedicated Port is 'standard'. The mode can only be changed when there are no associated virtual circuits on the interconnection.   In tunnel mode, an 802.1q tunnel is added to a port to send/receive double tagged packets from server instances.")
     name: StrictStr = ...
     project: Optional[StrictStr] = None
     redundancy: StrictStr = Field(..., description="Either 'primary' or 'redundant'.")
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/interconnection_list.py` & `equinix-metal-0.2.2/equinix_metal/models/interconnection_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/interconnection_metro.py` & `equinix-metal-0.2.2/equinix_metal/models/interconnection_metro.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/interconnection_port.py` & `equinix-metal-0.2.2/equinix_metal/models/interconnection_port.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/interconnection_port_list.py` & `equinix-metal-0.2.2/equinix_metal/models/interconnection_port_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/interconnection_update_input.py` & `equinix-metal-0.2.2/equinix_metal/models/interconnection_update_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/invitation.py` & `equinix-metal-0.2.2/equinix_metal/models/invitation.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/invitation_input.py` & `equinix-metal-0.2.2/equinix_metal/models/invitation_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/invitation_list.py` & `equinix-metal-0.2.2/equinix_metal/models/invitation_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/ip_address.py` & `equinix-metal-0.2.2/equinix_metal/models/ip_address.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/ip_assignment.py` & `equinix-metal-0.2.2/equinix_metal/models/ip_assignment.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
-from pydantic import BaseModel, StrictBool, StrictInt, StrictStr
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr, validator
 from equinix_metal.models.href import Href
 from equinix_metal.models.ip_assignment_metro import IPAssignmentMetro
 from equinix_metal.models.parent_block import ParentBlock
 
 class IPAssignment(BaseModel):
     """
     IPAssignment
@@ -41,17 +41,27 @@
     href: Optional[StrictStr] = None
     id: Optional[StrictStr] = None
     manageable: Optional[StrictBool] = None
     management: Optional[StrictBool] = None
     metro: Optional[IPAssignmentMetro] = None
     netmask: Optional[StrictStr] = None
     network: Optional[StrictStr] = None
+    next_hop: Optional[StrictStr] = Field(None, description="Only set when this is a Metal Gateway Elastic IP Assignment.  The IP address within the Metal Gateway to which requests to the Elastic IP are forwarded. ")
     parent_block: Optional[ParentBlock] = None
     public: Optional[StrictBool] = None
-    __properties = ["address", "address_family", "assigned_to", "cidr", "created_at", "enabled", "gateway", "global_ip", "href", "id", "manageable", "management", "metro", "netmask", "network", "parent_block", "public"]
+    state: Optional[StrictStr] = Field(None, description="Only set when this is a Metal Gateway Elastic IP Assignment.  Describes the current configuration state of this IP on the network. ")
+    __properties = ["address", "address_family", "assigned_to", "cidr", "created_at", "enabled", "gateway", "global_ip", "href", "id", "manageable", "management", "metro", "netmask", "network", "next_hop", "parent_block", "public", "state"]
+
+    @validator('state')
+    def state_validate_enum(cls, v):
+        if v is None:
+            return v
+        if v not in ('pending', 'active', 'deleting'):
+            raise ValueError("must be one of enum values ('pending', 'active', 'deleting')")
+        return v
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -104,12 +114,14 @@
             "href": obj.get("href"),
             "id": obj.get("id"),
             "manageable": obj.get("manageable"),
             "management": obj.get("management"),
             "metro": IPAssignmentMetro.from_dict(obj.get("metro")) if obj.get("metro") is not None else None,
             "netmask": obj.get("netmask"),
             "network": obj.get("network"),
+            "next_hop": obj.get("next_hop"),
             "parent_block": ParentBlock.from_dict(obj.get("parent_block")) if obj.get("parent_block") is not None else None,
-            "public": obj.get("public")
+            "public": obj.get("public"),
+            "state": obj.get("state")
         })
         return _obj
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/ip_assignment_input.py` & `equinix-metal-0.2.2/equinix_metal/models/ip_assignment_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/ip_assignment_list.py` & `equinix-metal-0.2.2/equinix_metal/models/ip_assignment_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/ip_assignment_metro.py` & `equinix-metal-0.2.2/equinix_metal/models/ip_assignment_metro.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/ip_assignment_update_input.py` & `equinix-metal-0.2.2/equinix_metal/models/ip_assignment_update_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/ip_availabilities_list.py` & `equinix-metal-0.2.2/equinix_metal/models/ip_availabilities_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/ip_reservation.py` & `equinix-metal-0.2.2/equinix_metal/models/ip_reservation.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/ip_reservation_facility.py` & `equinix-metal-0.2.2/equinix_metal/models/ip_reservation_facility.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/ip_reservation_list.py` & `equinix-metal-0.2.2/equinix_metal/models/ip_reservation_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/ip_reservation_list_ip_addresses_inner.py` & `equinix-metal-0.2.2/equinix_metal/models/ip_reservation_list_ip_addresses_inner.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/ip_reservation_metro.py` & `equinix-metal-0.2.2/equinix_metal/models/ip_reservation_metro.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/ip_reservation_request_input.py` & `equinix-metal-0.2.2/equinix_metal/models/ip_reservation_request_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/license.py` & `equinix-metal-0.2.2/equinix_metal/models/license.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/license_create_input.py` & `equinix-metal-0.2.2/equinix_metal/models/license_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/license_list.py` & `equinix-metal-0.2.2/equinix_metal/models/license_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/license_update_input.py` & `equinix-metal-0.2.2/equinix_metal/models/license_update_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/membership.py` & `equinix-metal-0.2.2/equinix_metal/models/membership.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/membership_input.py` & `equinix-metal-0.2.2/equinix_metal/models/membership_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/membership_list.py` & `equinix-metal-0.2.2/equinix_metal/models/membership_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/meta.py` & `equinix-metal-0.2.2/equinix_metal/models/meta.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/metadata.py` & `equinix-metal-0.2.2/equinix_metal/models/metadata.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/metadata_network.py` & `equinix-metal-0.2.2/equinix_metal/models/metadata_network.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/metadata_network_network.py` & `equinix-metal-0.2.2/equinix_metal/models/metadata_network_network.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/metadata_network_network_bonding.py` & `equinix-metal-0.2.2/equinix_metal/models/metadata_network_network_bonding.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/metal_gateway.py` & `equinix-metal-0.2.2/equinix_metal/models/metal_gateway.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/metal_gateway_create_input.py` & `equinix-metal-0.2.2/equinix_metal/models/metal_gateway_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/metal_gateway_list.py` & `equinix-metal-0.2.2/equinix_metal/models/metal_gateway_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/metal_gateway_list_metal_gateways_inner.py` & `equinix-metal-0.2.2/equinix_metal/models/metal_gateway_list_metal_gateways_inner.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/metal_gateway_lite.py` & `equinix-metal-0.2.2/equinix_metal/models/metal_gateway_lite.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/metro.py` & `equinix-metal-0.2.2/equinix_metal/models/metro.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/metro_capacity_list.py` & `equinix-metal-0.2.2/equinix_metal/models/metro_capacity_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/metro_capacity_report.py` & `equinix-metal-0.2.2/equinix_metal/models/metro_capacity_report.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/metro_input.py` & `equinix-metal-0.2.2/equinix_metal/models/metro_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/metro_list.py` & `equinix-metal-0.2.2/equinix_metal/models/metro_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/metro_server_info.py` & `equinix-metal-0.2.2/equinix_metal/models/metro_server_info.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/move_hardware_reservation_request.py` & `equinix-metal-0.2.2/equinix_metal/models/move_hardware_reservation_request.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/new_password.py` & `equinix-metal-0.2.2/equinix_metal/models/new_password.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/operating_system.py` & `equinix-metal-0.2.2/equinix_metal/models/operating_system.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/operating_system_list.py` & `equinix-metal-0.2.2/equinix_metal/models/operating_system_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/organization.py` & `equinix-metal-0.2.2/equinix_metal/models/organization.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictBytes, StrictFloat, StrictInt, StrictStr, conlist
+from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, conlist
 from equinix_metal.models.address import Address
 from equinix_metal.models.href import Href
 
 class Organization(BaseModel):
     """
     Organization
     """
@@ -34,15 +34,15 @@
     created_at: Optional[datetime] = None
     credit_amount: Optional[StrictFloat] = None
     customdata: Optional[Dict[str, Any]] = None
     description: Optional[StrictStr] = None
     enforce_2fa_at: Optional[datetime] = Field(None, description="Force to all members to have enabled the two factor authentication after that date, unless the value is null")
     href: Optional[StrictStr] = None
     id: Optional[StrictStr] = None
-    logo: Optional[StrictBytes] = None
+    logo: Optional[StrictStr] = None
     members: Optional[conlist(Href)] = None
     memberships: Optional[conlist(Href)] = None
     name: Optional[StrictStr] = None
     projects: Optional[conlist(Href)] = None
     terms: Optional[StrictInt] = None
     twitter: Optional[StrictStr] = None
     updated_at: Optional[datetime] = None
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/organization_input.py` & `equinix-metal-0.2.2/equinix_metal/models/organization_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/organization_list.py` & `equinix-metal-0.2.2/equinix_metal/models/organization_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/parent_block.py` & `equinix-metal-0.2.2/equinix_metal/models/parent_block.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/payment_method.py` & `equinix-metal-0.2.2/equinix_metal/models/payment_method.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/payment_method_billing_address.py` & `equinix-metal-0.2.2/equinix_metal/models/payment_method_billing_address.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/payment_method_create_input.py` & `equinix-metal-0.2.2/equinix_metal/models/payment_method_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/payment_method_list.py` & `equinix-metal-0.2.2/equinix_metal/models/payment_method_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/payment_method_update_input.py` & `equinix-metal-0.2.2/equinix_metal/models/payment_method_update_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/plan.py` & `equinix-metal-0.2.2/equinix_metal/models/plan.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,27 +28,28 @@
 
 class Plan(BaseModel):
     """
     Plan
     """
     available_in: Optional[conlist(PlanAvailableInInner)] = Field(None, description="Shows which facilities the plan is available in, and the facility-based price if it is different from the default price.")
     available_in_metros: Optional[conlist(PlanAvailableInMetrosInner)] = Field(None, description="Shows which metros the plan is available in, and the metro-based price if it is different from the default price.")
+    categories: Optional[conlist(StrictStr)] = Field(None, description="Categories of the plan, like compute or storage. A Plan can belong to multiple categories.")
     var_class: Optional[StrictStr] = Field(None, alias="class")
     deployment_types: Optional[conlist(StrictStr, min_items=0, unique_items=True)] = None
     description: Optional[StrictStr] = None
     href: Optional[StrictStr] = None
     id: Optional[StrictStr] = None
     legacy: Optional[StrictBool] = Field(None, description="Deprecated. Always return false")
     line: Optional[StrictStr] = None
     name: Optional[StrictStr] = None
     pricing: Optional[Dict[str, Any]] = None
     slug: Optional[StrictStr] = None
     specs: Optional[PlanSpecs] = None
     type: Optional[StrictStr] = Field(None, description="The plan type")
-    __properties = ["available_in", "available_in_metros", "class", "deployment_types", "description", "href", "id", "legacy", "line", "name", "pricing", "slug", "specs", "type"]
+    __properties = ["available_in", "available_in_metros", "categories", "class", "deployment_types", "description", "href", "id", "legacy", "line", "name", "pricing", "slug", "specs", "type"]
 
     @validator('deployment_types')
     def deployment_types_validate_enum(cls, v):
         if v is None:
             return v
         for i in v:
             if i not in ('on_demand', 'spot_market'):
@@ -113,14 +114,15 @@
 
         if type(obj) is not dict:
             return Plan.parse_obj(obj)
 
         _obj = Plan.parse_obj({
             "available_in": [PlanAvailableInInner.from_dict(_item) for _item in obj.get("available_in")] if obj.get("available_in") is not None else None,
             "available_in_metros": [PlanAvailableInMetrosInner.from_dict(_item) for _item in obj.get("available_in_metros")] if obj.get("available_in_metros") is not None else None,
+            "categories": obj.get("categories"),
             "var_class": obj.get("class"),
             "deployment_types": obj.get("deployment_types"),
             "description": obj.get("description"),
             "href": obj.get("href"),
             "id": obj.get("id"),
             "legacy": obj.get("legacy"),
             "line": obj.get("line"),
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/plan_available_in_inner.py` & `equinix-metal-0.2.2/equinix_metal/models/plan_available_in_inner.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/plan_available_in_inner_price.py` & `equinix-metal-0.2.2/equinix_metal/models/plan_available_in_inner_price.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/plan_available_in_metros_inner.py` & `equinix-metal-0.2.2/equinix_metal/models/plan_available_in_metros_inner.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/plan_list.py` & `equinix-metal-0.2.2/equinix_metal/models/plan_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/plan_specs.py` & `equinix-metal-0.2.2/equinix_metal/models/plan_specs.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/plan_specs_cpus_inner.py` & `equinix-metal-0.2.2/equinix_metal/models/plan_specs_cpus_inner.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/plan_specs_drives_inner.py` & `equinix-metal-0.2.2/equinix_metal/models/plan_specs_drives_inner.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/plan_specs_features.py` & `equinix-metal-0.2.2/equinix_metal/models/plan_specs_features.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/plan_specs_nics_inner.py` & `equinix-metal-0.2.2/equinix_metal/models/plan_specs_nics_inner.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/port.py` & `equinix-metal-0.2.2/equinix_metal/models/port.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/port_assign_input.py` & `equinix-metal-0.2.2/equinix_metal/models/port_assign_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/port_convert_layer3_input.py` & `equinix-metal-0.2.2/equinix_metal/models/port_convert_layer3_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/port_convert_layer3_input_request_ips_inner.py` & `equinix-metal-0.2.2/equinix_metal/models/port_convert_layer3_input_request_ips_inner.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/port_data.py` & `equinix-metal-0.2.2/equinix_metal/models/port_data.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/port_vlan_assignment.py` & `equinix-metal-0.2.2/equinix_metal/models/port_vlan_assignment.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/port_vlan_assignment_batch.py` & `equinix-metal-0.2.2/equinix_metal/models/port_vlan_assignment_batch.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/port_vlan_assignment_batch_create_input.py` & `equinix-metal-0.2.2/equinix_metal/models/port_vlan_assignment_batch_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/port_vlan_assignment_batch_create_input_vlan_assignments_inner.py` & `equinix-metal-0.2.2/equinix_metal/models/port_vlan_assignment_batch_create_input_vlan_assignments_inner.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/port_vlan_assignment_batch_list.py` & `equinix-metal-0.2.2/equinix_metal/models/port_vlan_assignment_batch_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/port_vlan_assignment_batch_vlan_assignments_inner.py` & `equinix-metal-0.2.2/equinix_metal/models/port_vlan_assignment_batch_vlan_assignments_inner.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/port_vlan_assignment_list.py` & `equinix-metal-0.2.2/equinix_metal/models/port_vlan_assignment_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/project.py` & `equinix-metal-0.2.2/equinix_metal/models/project.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/project_create_from_root_input.py` & `equinix-metal-0.2.2/equinix_metal/models/project_create_from_root_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/project_create_input.py` & `equinix-metal-0.2.2/equinix_metal/models/project_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/project_list.py` & `equinix-metal-0.2.2/equinix_metal/models/project_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/project_update_input.py` & `equinix-metal-0.2.2/equinix_metal/models/project_update_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/project_usage.py` & `equinix-metal-0.2.2/equinix_metal/models/project_usage.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/project_usage_list.py` & `equinix-metal-0.2.2/equinix_metal/models/project_usage_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/recovery_code_list.py` & `equinix-metal-0.2.2/equinix_metal/models/recovery_code_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/request_ip_reservation201_response.py` & `equinix-metal-0.2.2/equinix_metal/models/request_ip_reservation201_response.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/request_ip_reservation_request.py` & `equinix-metal-0.2.2/equinix_metal/models/request_ip_reservation_request.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/self_service_reservation_item_request.py` & `equinix-metal-0.2.2/equinix_metal/models/self_service_reservation_item_request.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/self_service_reservation_item_response.py` & `equinix-metal-0.2.2/equinix_metal/models/self_service_reservation_item_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,33 +16,34 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr
+from typing import List, Optional
+from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr, conlist
 
 class SelfServiceReservationItemResponse(BaseModel):
     """
     SelfServiceReservationItemResponse
     """
     amount: Optional[StrictFloat] = None
     href: Optional[StrictStr] = None
     id: Optional[StrictStr] = None
     metro_code: Optional[StrictStr] = None
     metro_id: Optional[StrictStr] = None
     metro_name: Optional[StrictStr] = None
+    plan_categories: Optional[conlist(StrictStr)] = None
     plan_id: Optional[StrictStr] = None
     plan_name: Optional[StrictStr] = None
     plan_slug: Optional[StrictStr] = None
     quantity: Optional[StrictInt] = None
     term: Optional[StrictStr] = None
-    __properties = ["amount", "href", "id", "metro_code", "metro_id", "metro_name", "plan_id", "plan_name", "plan_slug", "quantity", "term"]
+    __properties = ["amount", "href", "id", "metro_code", "metro_id", "metro_name", "plan_categories", "plan_id", "plan_name", "plan_slug", "quantity", "term"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -77,14 +78,15 @@
         _obj = SelfServiceReservationItemResponse.parse_obj({
             "amount": obj.get("amount"),
             "href": obj.get("href"),
             "id": obj.get("id"),
             "metro_code": obj.get("metro_code"),
             "metro_id": obj.get("metro_id"),
             "metro_name": obj.get("metro_name"),
+            "plan_categories": obj.get("plan_categories"),
             "plan_id": obj.get("plan_id"),
             "plan_name": obj.get("plan_name"),
             "plan_slug": obj.get("plan_slug"),
             "quantity": obj.get("quantity"),
             "term": obj.get("term")
         })
         return _obj
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/self_service_reservation_list.py` & `equinix-metal-0.2.2/equinix_metal/models/self_service_reservation_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/self_service_reservation_response.py` & `equinix-metal-0.2.2/equinix_metal/models/self_service_reservation_response.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/server_info.py` & `equinix-metal-0.2.2/equinix_metal/models/server_info.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/spot_market_prices_list.py` & `equinix-metal-0.2.2/equinix_metal/models/spot_market_prices_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/spot_market_prices_per_metro_list.py` & `equinix-metal-0.2.2/equinix_metal/models/spot_market_prices_per_metro_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/spot_market_prices_per_metro_report.py` & `equinix-metal-0.2.2/equinix_metal/models/spot_market_prices_per_metro_report.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/spot_market_request.py` & `equinix-metal-0.2.2/equinix_metal/models/spot_market_request.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/spot_market_request_create_input.py` & `equinix-metal-0.2.2/equinix_metal/models/spot_market_request_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/spot_market_request_create_input_instance_parameters.py` & `equinix-metal-0.2.2/equinix_metal/models/spot_market_request_create_input_instance_parameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     billing_cycle: Optional[StrictStr] = None
     customdata: Optional[Dict[str, Any]] = None
     description: Optional[StrictStr] = None
     features: Optional[conlist(StrictStr)] = None
     hostname: Optional[StrictStr] = None
     hostnames: Optional[conlist(StrictStr)] = None
     href: Optional[StrictStr] = None
-    locked: Optional[StrictBool] = None
+    locked: Optional[StrictBool] = Field(None, description="Whether the device should be locked, preventing accidental deletion.")
     no_ssh_keys: Optional[StrictBool] = None
     operating_system: Optional[StrictStr] = None
     plan: Optional[StrictStr] = None
     private_ipv4_subnet_size: Optional[StrictInt] = None
     project_ssh_keys: Optional[conlist(StrictStr)] = None
     public_ipv4_subnet_size: Optional[StrictInt] = None
     tags: Optional[conlist(StrictStr)] = None
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/spot_market_request_list.py` & `equinix-metal-0.2.2/equinix_metal/models/spot_market_request_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/spot_market_request_metro.py` & `equinix-metal-0.2.2/equinix_metal/models/spot_market_request_metro.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/spot_prices_datapoints.py` & `equinix-metal-0.2.2/equinix_metal/models/spot_prices_datapoints.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/spot_prices_history_report.py` & `equinix-metal-0.2.2/equinix_metal/models/spot_prices_history_report.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/spot_prices_per_baremetal.py` & `equinix-metal-0.2.2/equinix_metal/models/spot_prices_per_baremetal.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/spot_prices_per_facility.py` & `equinix-metal-0.2.2/equinix_metal/models/spot_prices_per_facility.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/spot_prices_per_new_facility.py` & `equinix-metal-0.2.2/equinix_metal/models/spot_prices_per_new_facility.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/spot_prices_report.py` & `equinix-metal-0.2.2/equinix_metal/models/spot_prices_report.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/ssh_key.py` & `equinix-metal-0.2.2/equinix_metal/models/ssh_key.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/ssh_key_create_input.py` & `equinix-metal-0.2.2/equinix_metal/models/ssh_key_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/ssh_key_input.py` & `equinix-metal-0.2.2/equinix_metal/models/ssh_key_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/ssh_key_list.py` & `equinix-metal-0.2.2/equinix_metal/models/ssh_key_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/support_request_input.py` & `equinix-metal-0.2.2/equinix_metal/models/support_request_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/transfer_request.py` & `equinix-metal-0.2.2/equinix_metal/models/transfer_request.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/transfer_request_input.py` & `equinix-metal-0.2.2/equinix_metal/models/transfer_request_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/transfer_request_list.py` & `equinix-metal-0.2.2/equinix_metal/models/transfer_request_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/update_email_input.py` & `equinix-metal-0.2.2/equinix_metal/models/update_email_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/user.py` & `equinix-metal-0.2.2/equinix_metal/models/user.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     """
     User
     """
     avatar_thumb_url: Optional[StrictStr] = None
     avatar_url: Optional[StrictStr] = None
     created_at: Optional[datetime] = None
     customdata: Optional[Dict[str, Any]] = None
+    default_organization_id: Optional[StrictStr] = None
+    default_project_id: Optional[StrictStr] = None
     email: Optional[StrictStr] = None
     emails: Optional[conlist(Href)] = None
     first_name: Optional[StrictStr] = None
     fraud_score: Optional[StrictStr] = None
     full_name: Optional[StrictStr] = None
     href: Optional[StrictStr] = None
     id: Optional[StrictStr] = None
@@ -44,15 +46,15 @@
     max_organizations: Optional[StrictInt] = None
     max_projects: Optional[StrictInt] = None
     phone_number: Optional[StrictStr] = None
     short_id: Optional[StrictStr] = None
     timezone: Optional[StrictStr] = None
     two_factor_auth: Optional[StrictStr] = None
     updated_at: Optional[datetime] = None
-    __properties = ["avatar_thumb_url", "avatar_url", "created_at", "customdata", "email", "emails", "first_name", "fraud_score", "full_name", "href", "id", "last_login_at", "last_name", "max_organizations", "max_projects", "phone_number", "short_id", "timezone", "two_factor_auth", "updated_at"]
+    __properties = ["avatar_thumb_url", "avatar_url", "created_at", "customdata", "default_organization_id", "default_project_id", "email", "emails", "first_name", "fraud_score", "full_name", "href", "id", "last_login_at", "last_name", "max_organizations", "max_projects", "phone_number", "short_id", "timezone", "two_factor_auth", "updated_at"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -92,14 +94,16 @@
             return User.parse_obj(obj)
 
         _obj = User.parse_obj({
             "avatar_thumb_url": obj.get("avatar_thumb_url"),
             "avatar_url": obj.get("avatar_url"),
             "created_at": obj.get("created_at"),
             "customdata": obj.get("customdata"),
+            "default_organization_id": obj.get("default_organization_id"),
+            "default_project_id": obj.get("default_project_id"),
             "email": obj.get("email"),
             "emails": [Href.from_dict(_item) for _item in obj.get("emails")] if obj.get("emails") is not None else None,
             "first_name": obj.get("first_name"),
             "fraud_score": obj.get("fraud_score"),
             "full_name": obj.get("full_name"),
             "href": obj.get("href"),
             "id": obj.get("id"),
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/user_create_input.py` & `equinix-metal-0.2.2/equinix_metal/models/user_create_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, StrictBool, StrictBytes, StrictStr, conlist
+from pydantic import BaseModel, StrictBytes, StrictStr, conlist
 from equinix_metal.models.email_input import EmailInput
 
 class UserCreateInput(BaseModel):
     """
     UserCreateInput
     """
     avatar: Optional[StrictBytes] = None
@@ -34,24 +34,23 @@
     customdata: Optional[Dict[str, Any]] = None
     emails: conlist(EmailInput) = ...
     first_name: StrictStr = ...
     href: Optional[StrictStr] = None
     invitation_id: Optional[StrictStr] = None
     last_name: StrictStr = ...
     level: Optional[StrictStr] = None
-    locked: Optional[StrictBool] = None
     nonce: Optional[StrictStr] = None
     password: Optional[StrictStr] = None
     phone_number: Optional[StrictStr] = None
     social_accounts: Optional[Dict[str, Any]] = None
     timezone: Optional[StrictStr] = None
     title: Optional[StrictStr] = None
     two_factor_auth: Optional[StrictStr] = None
     verified_at: Optional[datetime] = None
-    __properties = ["avatar", "company_name", "company_url", "customdata", "emails", "first_name", "href", "invitation_id", "last_name", "level", "locked", "nonce", "password", "phone_number", "social_accounts", "timezone", "title", "two_factor_auth", "verified_at"]
+    __properties = ["avatar", "company_name", "company_url", "customdata", "emails", "first_name", "href", "invitation_id", "last_name", "level", "nonce", "password", "phone_number", "social_accounts", "timezone", "title", "two_factor_auth", "verified_at"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -97,15 +96,14 @@
             "customdata": obj.get("customdata"),
             "emails": [EmailInput.from_dict(_item) for _item in obj.get("emails")] if obj.get("emails") is not None else None,
             "first_name": obj.get("first_name"),
             "href": obj.get("href"),
             "invitation_id": obj.get("invitation_id"),
             "last_name": obj.get("last_name"),
             "level": obj.get("level"),
-            "locked": obj.get("locked"),
             "nonce": obj.get("nonce"),
             "password": obj.get("password"),
             "phone_number": obj.get("phone_number"),
             "social_accounts": obj.get("social_accounts"),
             "timezone": obj.get("timezone"),
             "title": obj.get("title"),
             "two_factor_auth": obj.get("two_factor_auth"),
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/user_limited.py` & `equinix-metal-0.2.2/equinix_metal/models/user_limited.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/user_list.py` & `equinix-metal-0.2.2/equinix_metal/models/user_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/user_lite.py` & `equinix-metal-0.2.2/equinix_metal/models/user_lite.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/user_update_input.py` & `equinix-metal-0.2.2/equinix_metal/models/user_update_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/userdata.py` & `equinix-metal-0.2.2/equinix_metal/models/userdata.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/verify_email.py` & `equinix-metal-0.2.2/equinix_metal/models/verify_email.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/virtual_circuit.py` & `equinix-metal-0.2.2/equinix_metal/models/virtual_circuit.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/virtual_circuit_create_input.py` & `equinix-metal-0.2.2/equinix_metal/models/virtual_circuit_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/virtual_circuit_list.py` & `equinix-metal-0.2.2/equinix_metal/models/virtual_circuit_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/virtual_circuit_update_input.py` & `equinix-metal-0.2.2/equinix_metal/models/virtual_circuit_update_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/virtual_network.py` & `equinix-metal-0.2.2/equinix_metal/models/virtual_network.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/virtual_network_create_input.py` & `equinix-metal-0.2.2/equinix_metal/models/virtual_network_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/virtual_network_list.py` & `equinix-metal-0.2.2/equinix_metal/models/virtual_network_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/vlan_virtual_circuit.py` & `equinix-metal-0.2.2/equinix_metal/models/vlan_virtual_circuit.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/vlan_virtual_circuit_create_input.py` & `equinix-metal-0.2.2/equinix_metal/models/vlan_virtual_circuit_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/vlan_virtual_circuit_update_input.py` & `equinix-metal-0.2.2/equinix_metal/models/vlan_virtual_circuit_update_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/vrf.py` & `equinix-metal-0.2.2/equinix_metal/models/vrf.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/vrf_create_input.py` & `equinix-metal-0.2.2/equinix_metal/models/vrf_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/vrf_ip_reservation.py` & `equinix-metal-0.2.2/equinix_metal/models/vrf_ip_reservation.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/vrf_ip_reservation_create_input.py` & `equinix-metal-0.2.2/equinix_metal/models/vrf_ip_reservation_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/vrf_ip_reservation_list.py` & `equinix-metal-0.2.2/equinix_metal/models/vrf_ip_reservation_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/vrf_list.py` & `equinix-metal-0.2.2/equinix_metal/models/vrf_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/vrf_metal_gateway.py` & `equinix-metal-0.2.2/equinix_metal/models/vrf_metal_gateway.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/vrf_metal_gateway_create_input.py` & `equinix-metal-0.2.2/equinix_metal/models/vrf_metal_gateway_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/vrf_route.py` & `equinix-metal-0.2.2/equinix_metal/models/vrf_route.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,33 +18,33 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr, validator
-from equinix_metal.models.vrf_route_metal_gateway import VrfRouteMetalGateway
-from equinix_metal.models.vrf_route_virtual_network import VrfRouteVirtualNetwork
-from equinix_metal.models.vrf_route_vrf import VrfRouteVrf
+from equinix_metal.models.virtual_network import VirtualNetwork
+from equinix_metal.models.vrf import Vrf
+from equinix_metal.models.vrf_metal_gateway import VrfMetalGateway
 
 class VrfRoute(BaseModel):
     """
     VrfRoute
     """
     created_at: Optional[datetime] = None
     href: Optional[StrictStr] = None
     id: Optional[StrictStr] = Field(None, description="The unique identifier for the newly-created resource")
-    metal_gateway: Optional[VrfRouteMetalGateway] = None
+    metal_gateway: Optional[VrfMetalGateway] = None
     next_hop: Optional[StrictStr] = Field(None, description="The next-hop IPv4 address for the route")
     prefix: Optional[StrictStr] = Field(None, description="The IPv4 prefix for the route, in CIDR-style notation")
     status: Optional[StrictStr] = Field(None, description="The status of the route. Potential values are \"pending\", \"active\", \"deleting\", and \"error\", representing various lifecycle states of the route and whether or not it has been successfully configured on the network")
     type: Optional[StrictStr] = Field(None, description="VRF route type, like 'bgp', 'connected', and 'static'. Currently, only static routes are supported")
     updated_at: Optional[datetime] = None
-    virtual_network: Optional[VrfRouteVirtualNetwork] = None
-    vrf: Optional[VrfRouteVrf] = None
+    virtual_network: Optional[VirtualNetwork] = None
+    vrf: Optional[Vrf] = None
     __properties = ["created_at", "href", "id", "metal_gateway", "next_hop", "prefix", "status", "type", "updated_at", "virtual_network", "vrf"]
 
     @validator('status')
     def status_validate_enum(cls, v):
         if v is None:
             return v
         if v not in ('pending', 'active', 'deleting', 'error'):
@@ -108,18 +108,18 @@
         if type(obj) is not dict:
             return VrfRoute.parse_obj(obj)
 
         _obj = VrfRoute.parse_obj({
             "created_at": obj.get("created_at"),
             "href": obj.get("href"),
             "id": obj.get("id"),
-            "metal_gateway": VrfRouteMetalGateway.from_dict(obj.get("metal_gateway")) if obj.get("metal_gateway") is not None else None,
+            "metal_gateway": VrfMetalGateway.from_dict(obj.get("metal_gateway")) if obj.get("metal_gateway") is not None else None,
             "next_hop": obj.get("next_hop"),
             "prefix": obj.get("prefix"),
             "status": obj.get("status"),
             "type": obj.get("type"),
             "updated_at": obj.get("updated_at"),
-            "virtual_network": VrfRouteVirtualNetwork.from_dict(obj.get("virtual_network")) if obj.get("virtual_network") is not None else None,
-            "vrf": VrfRouteVrf.from_dict(obj.get("vrf")) if obj.get("vrf") is not None else None
+            "virtual_network": VirtualNetwork.from_dict(obj.get("virtual_network")) if obj.get("virtual_network") is not None else None,
+            "vrf": Vrf.from_dict(obj.get("vrf")) if obj.get("vrf") is not None else None
         })
         return _obj
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/vrf_route_create_input.py` & `equinix-metal-0.2.2/equinix_metal/models/vrf_route_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/vrf_route_list.py` & `equinix-metal-0.2.2/equinix_metal/models/vrf_route_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/vrf_route_metal_gateway.py` & `equinix-metal-0.2.2/equinix_metal/models/vrf_update_input.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,111 +11,75 @@
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
-import json
 import pprint
 import re  # noqa: F401
+import json
 
-from typing import Any, List, Optional
-from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
-from equinix_metal.models.href import Href
-from equinix_metal.models.metal_gateway import MetalGateway
-from typing import Any, List
-from pydantic import StrictStr, Field
 
-VRFROUTEMETALGATEWAY_ONE_OF_SCHEMAS = ["Href", "MetalGateway"]
+from typing import List, Optional
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr, conlist
 
-class VrfRouteMetalGateway(BaseModel):
+class VrfUpdateInput(BaseModel):
     """
-    A link to the Metal Gateway to which this VRF Route is associated
+    VrfUpdateInput
     """
-    # data type: Href
-    oneof_schema_1_validator: Optional[Href] = None
-    # data type: MetalGateway
-    oneof_schema_2_validator: Optional[MetalGateway] = None
-    actual_instance: Any
-    one_of_schemas: List[str] = Field(VRFROUTEMETALGATEWAY_ONE_OF_SCHEMAS, const=True)
+    bgp_dynamic_neighbors_bfd_enabled: Optional[StrictBool] = Field(None, description="Toggle BFD on dynamic bgp neighbors sessions")
+    bgp_dynamic_neighbors_enabled: Optional[StrictBool] = Field(None, description="Toggle to enable the dynamic bgp neighbors feature on the VRF")
+    bgp_dynamic_neighbors_export_route_map: Optional[StrictBool] = Field(None, description="Toggle to export the VRF route-map to the dynamic bgp neighbors")
+    description: Optional[StrictStr] = None
+    href: Optional[StrictStr] = None
+    ip_ranges: Optional[conlist(StrictStr)] = Field(None, description="A list of CIDR network addresses. Like [\"10.0.0.0/16\", \"2001:d78::/56\"]. IPv4 blocks must be between /8 and /29 in size. IPv6 blocks must be between /56 and /64. A VRF\\'s IP ranges must be defined in order to create VRF IP Reservations, which can then be used for Metal Gateways or Virtual Circuits. Adding a new CIDR address to the list will result in the creation of a new IP Range for this VRF. Removal of an existing CIDR address from the list will result in the deletion of an existing IP Range for this VRF. Deleting an IP Range will result in the deletion of any VRF IP Reservations contained within the IP Range, as well as the VRF IP Reservation\\'s associated Metal Gateways or Virtual Circuits. If you do not wish to add or remove IP Ranges, either include the full existing list of IP Ranges in the update request, or do not specify the `ip_ranges` field in the update request. Specifying a value of `[]` will remove all existing IP Ranges from the VRF.")
+    local_asn: Optional[StrictInt] = Field(None, description="The new `local_asn` value for the VRF. This field cannot be updated when there are active Interconnection Virtual Circuits associated to the VRF.")
+    name: Optional[StrictStr] = None
+    __properties = ["bgp_dynamic_neighbors_bfd_enabled", "bgp_dynamic_neighbors_enabled", "bgp_dynamic_neighbors_export_route_map", "description", "href", "ip_ranges", "local_asn", "name"]
 
     class Config:
+        allow_population_by_field_name = True
         validate_assignment = True
 
-    @validator('actual_instance')
-    def actual_instance_must_validate_oneof(cls, v):
-        instance = cls()
-        error_messages = []
-        match = 0
-        # validate data type: Href
-        if type(v) is not Href:
-            error_messages.append(f"Error! Input type `{type(v)}` is not `Href`")
-        else:
-            match += 1
-
-        # validate data type: MetalGateway
-        if type(v) is not MetalGateway:
-            error_messages.append(f"Error! Input type `{type(v)}` is not `MetalGateway`")
-        else:
-            match += 1
-
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into VrfRouteMetalGateway with oneOf schemas: Href, MetalGateway. Details: " + ", ".join(error_messages))
-        elif match == 0:
-            # no match
-            raise ValueError("No match found when deserializing the JSON string into VrfRouteMetalGateway with oneOf schemas: Href, MetalGateway. Details: " + ", ".join(error_messages))
-        else:
-            return v
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
 
-    @classmethod
-    def from_dict(cls, obj: dict) -> VrfRouteMetalGateway:
-        return cls.from_json(json.dumps(obj))
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VrfRouteMetalGateway:
-        """Returns the object represented by the json string"""
-        instance = cls()
-        error_messages = []
-        match = 0
-
-        # deserialize data into Href
-        try:
-            instance.actual_instance = Href.from_json(json_str)
-            match += 1
-        except ValidationError as e:
-            error_messages.append(str(e))
-        # deserialize data into MetalGateway
-        try:
-            instance.actual_instance = MetalGateway.from_json(json_str)
-            match += 1
-        except ValidationError as e:
-            error_messages.append(str(e))
-
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into VrfRouteMetalGateway with oneOf schemas: Href, MetalGateway. Details: " + ", ".join(error_messages))
-        elif match == 0:
-            # no match
-            raise ValueError("No match found when deserializing the JSON string into VrfRouteMetalGateway with oneOf schemas: Href, MetalGateway. Details: " + ", ".join(error_messages))
-        else:
-            return instance
+    def from_json(cls, json_str: str) -> VrfUpdateInput:
+        """Create an instance of VrfUpdateInput from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        return _dict
 
-    def to_json(self) -> str:
-        """Returns the JSON representation of the actual instance"""
-        if self.actual_instance is not None:
-            return self.actual_instance.to_json()
-        else:
-            return "null"
-
-    def to_dict(self) -> dict:
-        """Returns the dict representation of the actual instance"""
-        if self.actual_instance is not None:
-            return self.actual_instance.to_dict()
-        else:
-            return dict()
-
-    def to_str(self) -> str:
-        """Returns the string representation of the actual instance"""
-        return pprint.pformat(self.dict())
+    @classmethod
+    def from_dict(cls, obj: dict) -> VrfUpdateInput:
+        """Create an instance of VrfUpdateInput from a dict"""
+        if obj is None:
+            return None
+
+        if type(obj) is not dict:
+            return VrfUpdateInput.parse_obj(obj)
+
+        _obj = VrfUpdateInput.parse_obj({
+            "bgp_dynamic_neighbors_bfd_enabled": obj.get("bgp_dynamic_neighbors_bfd_enabled"),
+            "bgp_dynamic_neighbors_enabled": obj.get("bgp_dynamic_neighbors_enabled"),
+            "bgp_dynamic_neighbors_export_route_map": obj.get("bgp_dynamic_neighbors_export_route_map"),
+            "description": obj.get("description"),
+            "href": obj.get("href"),
+            "ip_ranges": obj.get("ip_ranges"),
+            "local_asn": obj.get("local_asn"),
+            "name": obj.get("name")
+        })
+        return _obj
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/vrf_route_virtual_network.py` & `equinix-metal-0.2.2/equinix_metal/models/line_item.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,111 +11,79 @@
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
-import json
 import pprint
 import re  # noqa: F401
+import json
 
-from typing import Any, List, Optional
-from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
-from equinix_metal.models.href import Href
-from equinix_metal.models.virtual_network import VirtualNetwork
-from typing import Any, List
-from pydantic import StrictStr, Field
 
-VRFROUTEVIRTUALNETWORK_ONE_OF_SCHEMAS = ["Href", "VirtualNetwork"]
+from typing import Optional
+from pydantic import BaseModel, StrictFloat, StrictStr
+from equinix_metal.models.plan import Plan
 
-class VrfRouteVirtualNetwork(BaseModel):
+class LineItem(BaseModel):
     """
-    A link to the Virtual Network to which this VRF Route is associated, through the Metal Gateway
+    LineItem
     """
-    # data type: Href
-    oneof_schema_1_validator: Optional[Href] = None
-    # data type: VirtualNetwork
-    oneof_schema_2_validator: Optional[VirtualNetwork] = None
-    actual_instance: Any
-    one_of_schemas: List[str] = Field(VRFROUTEVIRTUALNETWORK_ONE_OF_SCHEMAS, const=True)
+    amount: Optional[StrictFloat] = None
+    currency: Optional[StrictStr] = None
+    description: Optional[StrictStr] = None
+    details: Optional[StrictStr] = None
+    href: Optional[StrictStr] = None
+    plan: Optional[Plan] = None
+    unit: Optional[StrictStr] = None
+    unit_price: Optional[StrictFloat] = None
+    __properties = ["amount", "currency", "description", "details", "href", "plan", "unit", "unit_price"]
 
     class Config:
+        allow_population_by_field_name = True
         validate_assignment = True
 
-    @validator('actual_instance')
-    def actual_instance_must_validate_oneof(cls, v):
-        instance = cls()
-        error_messages = []
-        match = 0
-        # validate data type: Href
-        if type(v) is not Href:
-            error_messages.append(f"Error! Input type `{type(v)}` is not `Href`")
-        else:
-            match += 1
-
-        # validate data type: VirtualNetwork
-        if type(v) is not VirtualNetwork:
-            error_messages.append(f"Error! Input type `{type(v)}` is not `VirtualNetwork`")
-        else:
-            match += 1
-
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into VrfRouteVirtualNetwork with oneOf schemas: Href, VirtualNetwork. Details: " + ", ".join(error_messages))
-        elif match == 0:
-            # no match
-            raise ValueError("No match found when deserializing the JSON string into VrfRouteVirtualNetwork with oneOf schemas: Href, VirtualNetwork. Details: " + ", ".join(error_messages))
-        else:
-            return v
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
 
-    @classmethod
-    def from_dict(cls, obj: dict) -> VrfRouteVirtualNetwork:
-        return cls.from_json(json.dumps(obj))
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VrfRouteVirtualNetwork:
-        """Returns the object represented by the json string"""
-        instance = cls()
-        error_messages = []
-        match = 0
-
-        # deserialize data into Href
-        try:
-            instance.actual_instance = Href.from_json(json_str)
-            match += 1
-        except ValidationError as e:
-            error_messages.append(str(e))
-        # deserialize data into VirtualNetwork
-        try:
-            instance.actual_instance = VirtualNetwork.from_json(json_str)
-            match += 1
-        except ValidationError as e:
-            error_messages.append(str(e))
-
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into VrfRouteVirtualNetwork with oneOf schemas: Href, VirtualNetwork. Details: " + ", ".join(error_messages))
-        elif match == 0:
-            # no match
-            raise ValueError("No match found when deserializing the JSON string into VrfRouteVirtualNetwork with oneOf schemas: Href, VirtualNetwork. Details: " + ", ".join(error_messages))
-        else:
-            return instance
+    def from_json(cls, json_str: str) -> LineItem:
+        """Create an instance of LineItem from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of plan
+        if self.plan:
+            _dict['plan'] = self.plan.to_dict()
+        return _dict
 
-    def to_json(self) -> str:
-        """Returns the JSON representation of the actual instance"""
-        if self.actual_instance is not None:
-            return self.actual_instance.to_json()
-        else:
-            return "null"
-
-    def to_dict(self) -> dict:
-        """Returns the dict representation of the actual instance"""
-        if self.actual_instance is not None:
-            return self.actual_instance.to_dict()
-        else:
-            return dict()
-
-    def to_str(self) -> str:
-        """Returns the string representation of the actual instance"""
-        return pprint.pformat(self.dict())
+    @classmethod
+    def from_dict(cls, obj: dict) -> LineItem:
+        """Create an instance of LineItem from a dict"""
+        if obj is None:
+            return None
+
+        if type(obj) is not dict:
+            return LineItem.parse_obj(obj)
+
+        _obj = LineItem.parse_obj({
+            "amount": obj.get("amount"),
+            "currency": obj.get("currency"),
+            "description": obj.get("description"),
+            "details": obj.get("details"),
+            "href": obj.get("href"),
+            "plan": Plan.from_dict(obj.get("plan")) if obj.get("plan") is not None else None,
+            "unit": obj.get("unit"),
+            "unit_price": obj.get("unit_price")
+        })
+        return _obj
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/vrf_route_vrf.py` & `equinix-metal-0.2.2/equinix_metal/models/invoice_list.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,111 +11,71 @@
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
-import json
 import pprint
 import re  # noqa: F401
+import json
 
-from typing import Any, List, Optional
-from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
-from equinix_metal.models.href import Href
-from equinix_metal.models.vrf import Vrf
-from typing import Any, List
-from pydantic import StrictStr, Field
 
-VRFROUTEVRF_ONE_OF_SCHEMAS = ["Href", "Vrf"]
+from typing import List, Optional
+from pydantic import BaseModel, StrictStr, conlist
+from equinix_metal.models.invoice import Invoice
 
-class VrfRouteVrf(BaseModel):
+class InvoiceList(BaseModel):
     """
-    A link to the VRF within which this route exists
+    InvoiceList
     """
-    # data type: Href
-    oneof_schema_1_validator: Optional[Href] = None
-    # data type: Vrf
-    oneof_schema_2_validator: Optional[Vrf] = None
-    actual_instance: Any
-    one_of_schemas: List[str] = Field(VRFROUTEVRF_ONE_OF_SCHEMAS, const=True)
+    href: Optional[StrictStr] = None
+    invoices: Optional[conlist(Invoice)] = None
+    __properties = ["href", "invoices"]
 
     class Config:
+        allow_population_by_field_name = True
         validate_assignment = True
 
-    @validator('actual_instance')
-    def actual_instance_must_validate_oneof(cls, v):
-        instance = cls()
-        error_messages = []
-        match = 0
-        # validate data type: Href
-        if type(v) is not Href:
-            error_messages.append(f"Error! Input type `{type(v)}` is not `Href`")
-        else:
-            match += 1
-
-        # validate data type: Vrf
-        if type(v) is not Vrf:
-            error_messages.append(f"Error! Input type `{type(v)}` is not `Vrf`")
-        else:
-            match += 1
-
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into VrfRouteVrf with oneOf schemas: Href, Vrf. Details: " + ", ".join(error_messages))
-        elif match == 0:
-            # no match
-            raise ValueError("No match found when deserializing the JSON string into VrfRouteVrf with oneOf schemas: Href, Vrf. Details: " + ", ".join(error_messages))
-        else:
-            return v
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
 
-    @classmethod
-    def from_dict(cls, obj: dict) -> VrfRouteVrf:
-        return cls.from_json(json.dumps(obj))
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VrfRouteVrf:
-        """Returns the object represented by the json string"""
-        instance = cls()
-        error_messages = []
-        match = 0
-
-        # deserialize data into Href
-        try:
-            instance.actual_instance = Href.from_json(json_str)
-            match += 1
-        except ValidationError as e:
-            error_messages.append(str(e))
-        # deserialize data into Vrf
-        try:
-            instance.actual_instance = Vrf.from_json(json_str)
-            match += 1
-        except ValidationError as e:
-            error_messages.append(str(e))
-
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into VrfRouteVrf with oneOf schemas: Href, Vrf. Details: " + ", ".join(error_messages))
-        elif match == 0:
-            # no match
-            raise ValueError("No match found when deserializing the JSON string into VrfRouteVrf with oneOf schemas: Href, Vrf. Details: " + ", ".join(error_messages))
-        else:
-            return instance
+    def from_json(cls, json_str: str) -> InvoiceList:
+        """Create an instance of InvoiceList from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in invoices (list)
+        _items = []
+        if self.invoices:
+            for _item in self.invoices:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['invoices'] = _items
+        return _dict
 
-    def to_json(self) -> str:
-        """Returns the JSON representation of the actual instance"""
-        if self.actual_instance is not None:
-            return self.actual_instance.to_json()
-        else:
-            return "null"
-
-    def to_dict(self) -> dict:
-        """Returns the dict representation of the actual instance"""
-        if self.actual_instance is not None:
-            return self.actual_instance.to_dict()
-        else:
-            return dict()
-
-    def to_str(self) -> str:
-        """Returns the string representation of the actual instance"""
-        return pprint.pformat(self.dict())
+    @classmethod
+    def from_dict(cls, obj: dict) -> InvoiceList:
+        """Create an instance of InvoiceList from a dict"""
+        if obj is None:
+            return None
+
+        if type(obj) is not dict:
+            return InvoiceList.parse_obj(obj)
+
+        _obj = InvoiceList.parse_obj({
+            "href": obj.get("href"),
+            "invoices": [Invoice.from_dict(_item) for _item in obj.get("invoices")] if obj.get("invoices") is not None else None
+        })
+        return _obj
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/vrf_update_input.py` & `equinix-metal-0.2.2/equinix_metal/models/vrf_virtual_circuit_update_input.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,69 +17,73 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr, conlist
+from pydantic import BaseModel, Field, StrictInt, StrictStr, conlist
 
-class VrfUpdateInput(BaseModel):
+class VrfVirtualCircuitUpdateInput(BaseModel):
     """
-    VrfUpdateInput
+    VrfVirtualCircuitUpdateInput
     """
-    bgp_dynamic_neighbors_bfd_enabled: Optional[StrictBool] = Field(None, description="Toggle BFD on dynamic bgp neighbors sessions")
-    bgp_dynamic_neighbors_enabled: Optional[StrictBool] = Field(None, description="Toggle to enable the dynamic bgp neighbors feature on the VRF")
-    bgp_dynamic_neighbors_export_route_map: Optional[StrictBool] = Field(None, description="Toggle to export the VRF route-map to the dynamic bgp neighbors")
+    customer_ip: Optional[StrictStr] = Field(None, description="An IP address from the subnet that will be used on the Customer side. This parameter is optional, but if supplied, we will use the other usable IP address in the subnet as the Metal IP. By default, the last usable IP address in the subnet will be used.")
     description: Optional[StrictStr] = None
     href: Optional[StrictStr] = None
-    ip_ranges: Optional[conlist(StrictStr)] = Field(None, description="A list of CIDR network addresses. Like [\"10.0.0.0/16\", \"2001:d78::/56\"]. IPv4 blocks must be between /8 and /29 in size. IPv6 blocks must be between /56 and /64. A VRF\\'s IP ranges must be defined in order to create VRF IP Reservations, which can then be used for Metal Gateways or Virtual Circuits. Adding a new CIDR address to the list will result in the creation of a new IP Range for this VRF. Removal of an existing CIDR address from the list will result in the deletion of an existing IP Range for this VRF. Deleting an IP Range will result in the deletion of any VRF IP Reservations contained within the IP Range, as well as the VRF IP Reservation\\'s associated Metal Gateways or Virtual Circuits. If you do not wish to add or remove IP Ranges, either include the full existing list of IP Ranges in the update request, or do not specify the `ip_ranges` field in the update request. Specifying a value of `[]` will remove all existing IP Ranges from the VRF.")
-    local_asn: Optional[StrictInt] = Field(None, description="The new `local_asn` value for the VRF. This field cannot be updated when there are active Interconnection Virtual Circuits associated to the VRF.")
+    md5: Optional[StrictStr] = Field(None, description="The MD5 password for the BGP peering in plaintext (not a checksum).")
+    metal_ip: Optional[StrictStr] = Field(None, description="An IP address from the subnet that will be used on the Metal side. This parameter is optional, but if supplied, we will use the other usable IP address in the subnet as the Customer IP. By default, the first usable IP address in the subnet will be used.")
     name: Optional[StrictStr] = None
-    __properties = ["bgp_dynamic_neighbors_bfd_enabled", "bgp_dynamic_neighbors_enabled", "bgp_dynamic_neighbors_export_route_map", "description", "href", "ip_ranges", "local_asn", "name"]
+    peer_asn: Optional[StrictInt] = Field(None, description="The peer ASN that will be used with the VRF on the Virtual Circuit.")
+    speed: Optional[StrictStr] = Field(None, description="Speed can be changed only if it is an interconnection on a Dedicated Port")
+    subnet: Optional[StrictStr] = Field(None, description="The /30 or /31 subnet of one of the VRF IP Blocks that will be used with the VRF for the Virtual Circuit. This subnet does not have to be an existing VRF IP reservation, as we will create the VRF IP reservation on creation if it does not exist. The Metal IP and Customer IP must be IPs from this subnet. For /30 subnets, the network and broadcast IPs cannot be used as the Metal or Customer IP.")
+    tags: Optional[conlist(StrictStr)] = None
+    __properties = ["customer_ip", "description", "href", "md5", "metal_ip", "name", "peer_asn", "speed", "subnet", "tags"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VrfUpdateInput:
-        """Create an instance of VrfUpdateInput from a JSON string"""
+    def from_json(cls, json_str: str) -> VrfVirtualCircuitUpdateInput:
+        """Create an instance of VrfVirtualCircuitUpdateInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> VrfUpdateInput:
-        """Create an instance of VrfUpdateInput from a dict"""
+    def from_dict(cls, obj: dict) -> VrfVirtualCircuitUpdateInput:
+        """Create an instance of VrfVirtualCircuitUpdateInput from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return VrfUpdateInput.parse_obj(obj)
+            return VrfVirtualCircuitUpdateInput.parse_obj(obj)
 
-        _obj = VrfUpdateInput.parse_obj({
-            "bgp_dynamic_neighbors_bfd_enabled": obj.get("bgp_dynamic_neighbors_bfd_enabled"),
-            "bgp_dynamic_neighbors_enabled": obj.get("bgp_dynamic_neighbors_enabled"),
-            "bgp_dynamic_neighbors_export_route_map": obj.get("bgp_dynamic_neighbors_export_route_map"),
+        _obj = VrfVirtualCircuitUpdateInput.parse_obj({
+            "customer_ip": obj.get("customer_ip"),
             "description": obj.get("description"),
             "href": obj.get("href"),
-            "ip_ranges": obj.get("ip_ranges"),
-            "local_asn": obj.get("local_asn"),
-            "name": obj.get("name")
+            "md5": obj.get("md5"),
+            "metal_ip": obj.get("metal_ip"),
+            "name": obj.get("name"),
+            "peer_asn": obj.get("peer_asn"),
+            "speed": obj.get("speed"),
+            "subnet": obj.get("subnet"),
+            "tags": obj.get("tags")
         })
         return _obj
```

### Comparing `equinix-metal-0.2.1/equinix_metal/models/vrf_virtual_circuit.py` & `equinix-metal-0.2.2/equinix_metal/models/vrf_virtual_circuit.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/vrf_virtual_circuit_create_input.py` & `equinix-metal-0.2.2/equinix_metal/models/vrf_virtual_circuit_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal/models/vrf_virtual_circuit_update_input.py` & `equinix-metal-0.2.2/equinix_metal/models/metal_gateway_elastic_ip_create_input.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,74 +16,64 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr, conlist
+from typing import Any, Dict, List, Optional
+from pydantic import BaseModel, Field, StrictStr, conlist
 
-class VrfVirtualCircuitUpdateInput(BaseModel):
+class MetalGatewayElasticIpCreateInput(BaseModel):
     """
-    VrfVirtualCircuitUpdateInput
+    MetalGatewayElasticIpCreateInput
     """
-    customer_ip: Optional[StrictStr] = Field(None, description="An IP address from the subnet that will be used on the Customer side. This parameter is optional, but if supplied, we will use the other usable IP address in the subnet as the Metal IP. By default, the last usable IP address in the subnet will be used.")
-    description: Optional[StrictStr] = None
+    address: StrictStr = Field(..., description="An IP address (or IP Address range) contained within one of the project's IP Reservations")
+    customdata: Optional[Dict[str, Any]] = Field(None, description="Optional User-defined JSON object value.")
     href: Optional[StrictStr] = None
-    md5: Optional[StrictStr] = Field(None, description="The MD5 password for the BGP peering in plaintext (not a checksum).")
-    metal_ip: Optional[StrictStr] = Field(None, description="An IP address from the subnet that will be used on the Metal side. This parameter is optional, but if supplied, we will use the other usable IP address in the subnet as the Customer IP. By default, the first usable IP address in the subnet will be used.")
-    name: Optional[StrictStr] = None
-    peer_asn: Optional[StrictInt] = Field(None, description="The peer ASN that will be used with the VRF on the Virtual Circuit.")
-    speed: Optional[StrictStr] = Field(None, description="Speed can be changed only if it is an interconnection on a Dedicated Port")
-    subnet: Optional[StrictStr] = Field(None, description="The /30 or /31 subnet of one of the VRF IP Blocks that will be used with the VRF for the Virtual Circuit. This subnet does not have to be an existing VRF IP reservation, as we will create the VRF IP reservation on creation if it does not exist. The Metal IP and Customer IP must be IPs from this subnet. For /30 subnets, the network and broadcast IPs cannot be used as the Metal or Customer IP.")
-    tags: Optional[conlist(StrictStr)] = None
-    __properties = ["customer_ip", "description", "href", "md5", "metal_ip", "name", "peer_asn", "speed", "subnet", "tags"]
+    next_hop: StrictStr = Field(..., description="An IP address contained within the Metal Gateways' IP Reservation range.")
+    tags: Optional[conlist(StrictStr)] = Field(None, description="Optional list of User-defined tags. Can be used by users to provide additional details or context regarding the purpose or usage of this resource.")
+    __properties = ["address", "customdata", "href", "next_hop", "tags"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VrfVirtualCircuitUpdateInput:
-        """Create an instance of VrfVirtualCircuitUpdateInput from a JSON string"""
+    def from_json(cls, json_str: str) -> MetalGatewayElasticIpCreateInput:
+        """Create an instance of MetalGatewayElasticIpCreateInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> VrfVirtualCircuitUpdateInput:
-        """Create an instance of VrfVirtualCircuitUpdateInput from a dict"""
+    def from_dict(cls, obj: dict) -> MetalGatewayElasticIpCreateInput:
+        """Create an instance of MetalGatewayElasticIpCreateInput from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return VrfVirtualCircuitUpdateInput.parse_obj(obj)
+            return MetalGatewayElasticIpCreateInput.parse_obj(obj)
 
-        _obj = VrfVirtualCircuitUpdateInput.parse_obj({
-            "customer_ip": obj.get("customer_ip"),
-            "description": obj.get("description"),
+        _obj = MetalGatewayElasticIpCreateInput.parse_obj({
+            "address": obj.get("address"),
+            "customdata": obj.get("customdata"),
             "href": obj.get("href"),
-            "md5": obj.get("md5"),
-            "metal_ip": obj.get("metal_ip"),
-            "name": obj.get("name"),
-            "peer_asn": obj.get("peer_asn"),
-            "speed": obj.get("speed"),
-            "subnet": obj.get("subnet"),
+            "next_hop": obj.get("next_hop"),
             "tags": obj.get("tags")
         })
         return _obj
```

### Comparing `equinix-metal-0.2.1/equinix_metal/rest.py` & `equinix-metal-0.2.2/equinix_metal/rest.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/equinix_metal.egg-info/PKG-INFO` & `equinix-metal-0.2.2/equinix_metal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equinix-metal
-Version: 0.2.1
+Version: 0.2.2
 Summary: Metal API
 Home-page: 
 Author: Equinix Metal API Team
 Author-email: support@equinixmetal.com
 License: Equinix Metal
 Keywords: OpenAPI,OpenAPI-Generator,Metal API
 Description-Content-Type: text/markdown
```

### Comparing `equinix-metal-0.2.1/equinix_metal.egg-info/SOURCES.txt` & `equinix-metal-0.2.2/equinix_metal.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 equinix_metal/api/emails_api.py
 equinix_metal/api/events_api.py
 equinix_metal/api/facilities_api.py
 equinix_metal/api/hardware_reservations_api.py
 equinix_metal/api/incidents_api.py
 equinix_metal/api/interconnections_api.py
 equinix_metal/api/invitations_api.py
+equinix_metal/api/invoices_api.py
 equinix_metal/api/ip_addresses_api.py
 equinix_metal/api/licenses_api.py
 equinix_metal/api/memberships_api.py
 equinix_metal/api/metal_gateways_api.py
 equinix_metal/api/metros_api.py
 equinix_metal/api/operating_systems_api.py
 equinix_metal/api/organizations_api.py
@@ -131,14 +132,16 @@
 equinix_metal/models/interconnection_metro.py
 equinix_metal/models/interconnection_port.py
 equinix_metal/models/interconnection_port_list.py
 equinix_metal/models/interconnection_update_input.py
 equinix_metal/models/invitation.py
 equinix_metal/models/invitation_input.py
 equinix_metal/models/invitation_list.py
+equinix_metal/models/invoice.py
+equinix_metal/models/invoice_list.py
 equinix_metal/models/ip_address.py
 equinix_metal/models/ip_assignment.py
 equinix_metal/models/ip_assignment_input.py
 equinix_metal/models/ip_assignment_list.py
 equinix_metal/models/ip_assignment_metro.py
 equinix_metal/models/ip_assignment_update_input.py
 equinix_metal/models/ip_availabilities_list.py
@@ -148,24 +151,26 @@
 equinix_metal/models/ip_reservation_list_ip_addresses_inner.py
 equinix_metal/models/ip_reservation_metro.py
 equinix_metal/models/ip_reservation_request_input.py
 equinix_metal/models/license.py
 equinix_metal/models/license_create_input.py
 equinix_metal/models/license_list.py
 equinix_metal/models/license_update_input.py
+equinix_metal/models/line_item.py
 equinix_metal/models/membership.py
 equinix_metal/models/membership_input.py
 equinix_metal/models/membership_list.py
 equinix_metal/models/meta.py
 equinix_metal/models/metadata.py
 equinix_metal/models/metadata_network.py
 equinix_metal/models/metadata_network_network.py
 equinix_metal/models/metadata_network_network_bonding.py
 equinix_metal/models/metal_gateway.py
 equinix_metal/models/metal_gateway_create_input.py
+equinix_metal/models/metal_gateway_elastic_ip_create_input.py
 equinix_metal/models/metal_gateway_list.py
 equinix_metal/models/metal_gateway_list_metal_gateways_inner.py
 equinix_metal/models/metal_gateway_lite.py
 equinix_metal/models/metro.py
 equinix_metal/models/metro_capacity_list.py
 equinix_metal/models/metro_capacity_report.py
 equinix_metal/models/metro_input.py
@@ -205,14 +210,15 @@
 equinix_metal/models/port_vlan_assignment_batch_create_input_vlan_assignments_inner.py
 equinix_metal/models/port_vlan_assignment_batch_list.py
 equinix_metal/models/port_vlan_assignment_batch_vlan_assignments_inner.py
 equinix_metal/models/port_vlan_assignment_list.py
 equinix_metal/models/project.py
 equinix_metal/models/project_create_from_root_input.py
 equinix_metal/models/project_create_input.py
+equinix_metal/models/project_id_name.py
 equinix_metal/models/project_list.py
 equinix_metal/models/project_update_input.py
 equinix_metal/models/project_usage.py
 equinix_metal/models/project_usage_list.py
 equinix_metal/models/recovery_code_list.py
 equinix_metal/models/request_ip_reservation201_response.py
 equinix_metal/models/request_ip_reservation_request.py
@@ -269,17 +275,15 @@
 equinix_metal/models/vrf_ip_reservation_list.py
 equinix_metal/models/vrf_list.py
 equinix_metal/models/vrf_metal_gateway.py
 equinix_metal/models/vrf_metal_gateway_create_input.py
 equinix_metal/models/vrf_route.py
 equinix_metal/models/vrf_route_create_input.py
 equinix_metal/models/vrf_route_list.py
-equinix_metal/models/vrf_route_metal_gateway.py
-equinix_metal/models/vrf_route_virtual_network.py
-equinix_metal/models/vrf_route_vrf.py
+equinix_metal/models/vrf_route_update_input.py
 equinix_metal/models/vrf_update_input.py
 equinix_metal/models/vrf_virtual_circuit.py
 equinix_metal/models/vrf_virtual_circuit_create_input.py
 equinix_metal/models/vrf_virtual_circuit_update_input.py
 test/test_activate_hardware_reservation_request.py
 test/test_address.py
 test/test_auth_token.py
@@ -372,14 +376,17 @@
 test/test_interconnection_port_list.py
 test/test_interconnection_update_input.py
 test/test_interconnections_api.py
 test/test_invitation.py
 test/test_invitation_input.py
 test/test_invitation_list.py
 test/test_invitations_api.py
+test/test_invoice.py
+test/test_invoice_list.py
+test/test_invoices_api.py
 test/test_ip_address.py
 test/test_ip_addresses_api.py
 test/test_ip_assignment.py
 test/test_ip_assignment_input.py
 test/test_ip_assignment_list.py
 test/test_ip_assignment_metro.py
 test/test_ip_assignment_update_input.py
@@ -391,25 +398,27 @@
 test/test_ip_reservation_metro.py
 test/test_ip_reservation_request_input.py
 test/test_license.py
 test/test_license_create_input.py
 test/test_license_list.py
 test/test_license_update_input.py
 test/test_licenses_api.py
+test/test_line_item.py
 test/test_membership.py
 test/test_membership_input.py
 test/test_membership_list.py
 test/test_memberships_api.py
 test/test_meta.py
 test/test_metadata.py
 test/test_metadata_network.py
 test/test_metadata_network_network.py
 test/test_metadata_network_network_bonding.py
 test/test_metal_gateway.py
 test/test_metal_gateway_create_input.py
+test/test_metal_gateway_elastic_ip_create_input.py
 test/test_metal_gateway_list.py
 test/test_metal_gateway_list_metal_gateways_inner.py
 test/test_metal_gateway_lite.py
 test/test_metal_gateways_api.py
 test/test_metro.py
 test/test_metro_capacity_list.py
 test/test_metro_capacity_report.py
@@ -458,14 +467,15 @@
 test/test_port_vlan_assignment_batch_list.py
 test/test_port_vlan_assignment_batch_vlan_assignments_inner.py
 test/test_port_vlan_assignment_list.py
 test/test_ports_api.py
 test/test_project.py
 test/test_project_create_from_root_input.py
 test/test_project_create_input.py
+test/test_project_id_name.py
 test/test_project_list.py
 test/test_project_update_input.py
 test/test_project_usage.py
 test/test_project_usage_list.py
 test/test_projects_api.py
 test/test_recovery_code_list.py
 test/test_request_ip_reservation201_response.py
@@ -534,15 +544,13 @@
 test/test_vrf_ip_reservation_list.py
 test/test_vrf_list.py
 test/test_vrf_metal_gateway.py
 test/test_vrf_metal_gateway_create_input.py
 test/test_vrf_route.py
 test/test_vrf_route_create_input.py
 test/test_vrf_route_list.py
-test/test_vrf_route_metal_gateway.py
-test/test_vrf_route_virtual_network.py
-test/test_vrf_route_vrf.py
+test/test_vrf_route_update_input.py
 test/test_vrf_update_input.py
 test/test_vrf_virtual_circuit.py
 test/test_vrf_virtual_circuit_create_input.py
 test/test_vrf_virtual_circuit_update_input.py
 test/test_vrfs_api.py
```

### Comparing `equinix-metal-0.2.1/pyproject.toml` & `equinix-metal-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "equinix_metal"
-version = "0.2.1"
+version = "0.2.2"
 description = "Metal API"
 authors = ["support@equinixmetal.com"]
 license = "Equinix Metal"
 readme = "README.md"
 repository = "https://github.com/metal-python/equinix-labs"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Metal API"]
```

### Comparing `equinix-metal-0.2.1/setup.py` & `equinix-metal-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "equinix-metal"
-VERSION = "0.2.1"
+VERSION = "0.2.2"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3",
     "python-dateutil",
     "pydantic",
     "aenum"
 ]
```

### Comparing `equinix-metal-0.2.1/test/test_activate_hardware_reservation_request.py` & `equinix-metal-0.2.2/test/test_activate_hardware_reservation_request.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_address.py` & `equinix-metal-0.2.2/test/test_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,17 +51,14 @@
                 country = '', 
                 href = '', 
                 state = '', 
                 zip_code = ''
             )
         else :
             return Address(
-                address = '',
-                country = '',
-                zip_code = '',
         )
         """
 
     def testAddress(self):
         """Test Address"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `equinix-metal-0.2.1/test/test_auth_token.py` & `equinix-metal-0.2.2/test/test_auth_token.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_auth_token_input.py` & `equinix-metal-0.2.2/test/test_auth_token_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_auth_token_list.py` & `equinix-metal-0.2.2/test/test_auth_token_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_auth_token_project.py` & `equinix-metal-0.2.2/test/test_auth_token_project.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_auth_token_user.py` & `equinix-metal-0.2.2/test/test_auth_token_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,16 @@
         model = equinix_metal.models.auth_token_user.AuthTokenUser()  # noqa: E501
         if include_optional :
             return AuthTokenUser(
                 avatar_thumb_url = '', 
                 avatar_url = '', 
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 customdata = equinix_metal.models.customdata.customdata(), 
+                default_organization_id = '', 
+                default_project_id = '', 
                 email = '', 
                 emails = [
                     equinix_metal.models.href.Href(
                         href = '', )
                     ], 
                 first_name = '', 
                 fraud_score = '',
```

### Comparing `equinix-metal-0.2.1/test/test_authentication_api.py` & `equinix-metal-0.2.2/test/test_authentication_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_batch.py` & `equinix-metal-0.2.2/test/test_batch.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_batches_api.py` & `equinix-metal-0.2.2/test/test_batches_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_batches_list.py` & `equinix-metal-0.2.2/test/test_batches_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_bgp_api.py` & `equinix-metal-0.2.2/test/test_bgp_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_bgp_config.py` & `equinix-metal-0.2.2/test/test_bgp_config.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_bgp_config_request_input.py` & `equinix-metal-0.2.2/test/test_bgp_config_request_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_bgp_dynamic_neighbor.py` & `equinix-metal-0.2.2/test/test_bgp_dynamic_neighbor.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_bgp_dynamic_neighbor_create_input.py` & `equinix-metal-0.2.2/test/test_bgp_dynamic_neighbor_create_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
             return BgpDynamicNeighborCreateInput(
                 bgp_neighbor_asn = 12345, 
                 bgp_neighbor_range = '192.168.1.0/25', 
                 href = ''
             )
         else :
             return BgpDynamicNeighborCreateInput(
+                bgp_neighbor_asn = 12345,
+                bgp_neighbor_range = '192.168.1.0/25',
         )
         """
 
     def testBgpDynamicNeighborCreateInput(self):
         """Test BgpDynamicNeighborCreateInput"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `equinix-metal-0.2.1/test/test_bgp_dynamic_neighbor_list.py` & `equinix-metal-0.2.2/test/test_bgp_dynamic_neighbor_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_bgp_neighbor_data.py` & `equinix-metal-0.2.2/test/test_bgp_neighbor_data.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_bgp_route.py` & `equinix-metal-0.2.2/test/test_bgp_route.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_bgp_session.py` & `equinix-metal-0.2.2/test/test_bgp_session.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_bgp_session_input.py` & `equinix-metal-0.2.2/test/test_bgp_session_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_bgp_session_list.py` & `equinix-metal-0.2.2/test/test_bgp_session_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_bgp_session_neighbors.py` & `equinix-metal-0.2.2/test/test_bgp_session_neighbors.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_bond_port_data.py` & `equinix-metal-0.2.2/test/test_bond_port_data.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_capacity_api.py` & `equinix-metal-0.2.2/test/test_capacity_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_capacity_check_per_facility_info.py` & `equinix-metal-0.2.2/test/test_capacity_check_per_facility_info.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_capacity_check_per_facility_list.py` & `equinix-metal-0.2.2/test/test_capacity_check_per_facility_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_capacity_check_per_metro_info.py` & `equinix-metal-0.2.2/test/test_capacity_check_per_metro_info.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_capacity_check_per_metro_list.py` & `equinix-metal-0.2.2/test/test_capacity_check_per_metro_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_capacity_input.py` & `equinix-metal-0.2.2/test/test_capacity_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_capacity_level_per_baremetal.py` & `equinix-metal-0.2.2/test/test_capacity_level_per_baremetal.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_capacity_list.py` & `equinix-metal-0.2.2/test/test_capacity_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_capacity_per_facility.py` & `equinix-metal-0.2.2/test/test_capacity_per_facility.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_capacity_per_metro_input.py` & `equinix-metal-0.2.2/test/test_capacity_per_metro_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_capacity_per_new_facility.py` & `equinix-metal-0.2.2/test/test_capacity_per_new_facility.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_capacity_report.py` & `equinix-metal-0.2.2/test/test_capacity_report.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_coordinates.py` & `equinix-metal-0.2.2/test/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_create_device_request.py` & `equinix-metal-0.2.2/test/test_create_device_request.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_create_email_input.py` & `equinix-metal-0.2.2/test/test_create_email_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_create_metal_gateway_request.py` & `equinix-metal-0.2.2/test/test_create_metal_gateway_request.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_create_self_service_reservation_request.py` & `equinix-metal-0.2.2/test/test_create_self_service_reservation_request.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_create_self_service_reservation_request_period.py` & `equinix-metal-0.2.2/test/test_create_self_service_reservation_request_period.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_device.py` & `equinix-metal-0.2.2/test/test_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
                 bonding_mode = 56, 
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 created_by = None, 
                 customdata = { }, 
                 description = '', 
                 facility = equinix_metal.models.facility.Facility(
                     address = equinix_metal.models.address.Address(
-                        address = '', 
                         address2 = '', 
                         city = '', 
                         coordinates = equinix_metal.models.coordinates.Coordinates(
                             href = '', 
                             latitude = '', 
                             longitude = '', ), 
                         country = '', 
@@ -94,20 +93,22 @@
                         href = '', 
                         id = '', 
                         manageable = True, 
                         management = True, 
                         metro = null, 
                         netmask = '', 
                         network = '', 
+                        next_hop = '', 
                         parent_block = equinix_metal.models.parent_block.ParentBlock(
                             cidr = 56, 
                             href = '', 
                             netmask = '', 
                             network = '', ), 
-                        public = True, )
+                        public = True, 
+                        state = 'pending', )
                     ], 
                 ipxe_script_url = '', 
                 iqn = '', 
                 locked = True, 
                 metro = None, 
                 network_ports = [
                     equinix_metal.models.port.Port(
@@ -176,14 +177,17 @@
                                 hour = 1.23, 
                                 href = '', ), )
                         ], 
                     available_in_metros = [
                         equinix_metal.models.plan_available_in_metros_inner.Plan_available_in_metros_inner(
                             href = '', )
                         ], 
+                    categories = [
+                        ''
+                        ], 
                     class = 'm3.large.x86', 
                     deployment_types = [
                         'on_demand'
                         ], 
                     description = '', 
                     href = '', 
                     id = '',
```

### Comparing `equinix-metal-0.2.1/test/test_device_action_input.py` & `equinix-metal-0.2.2/test/test_device_action_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_device_actions_inner.py` & `equinix-metal-0.2.2/test/test_device_actions_inner.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_device_create_in_facility_input.py` & `equinix-metal-0.2.2/test/test_device_create_in_facility_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_device_create_in_metro_input.py` & `equinix-metal-0.2.2/test/test_device_create_in_metro_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_device_create_input.py` & `equinix-metal-0.2.2/test/test_device_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_device_created_by.py` & `equinix-metal-0.2.2/test/test_device_created_by.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_device_list.py` & `equinix-metal-0.2.2/test/test_device_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
                         bonding_mode = 56, 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         created_by = null, 
                         customdata = { }, 
                         description = '', 
                         facility = equinix_metal.models.facility.Facility(
                             address = equinix_metal.models.address.Address(
-                                address = '', 
                                 address2 = '', 
                                 city = '', 
                                 coordinates = equinix_metal.models.coordinates.Coordinates(
                                     href = '', 
                                     latitude = '', 
                                     longitude = '', ), 
                                 country = '', 
@@ -94,20 +93,22 @@
                                 global_ip = True, 
                                 href = '', 
                                 id = '', 
                                 manageable = True, 
                                 management = True, 
                                 netmask = '', 
                                 network = '', 
+                                next_hop = '', 
                                 parent_block = equinix_metal.models.parent_block.ParentBlock(
                                     cidr = 56, 
                                     href = '', 
                                     netmask = '', 
                                     network = '', ), 
-                                public = True, )
+                                public = True, 
+                                state = 'pending', )
                             ], 
                         ipxe_script_url = '', 
                         iqn = '', 
                         locked = True, 
                         metro = null, 
                         network_ports = [
                             equinix_metal.models.port.Port(
@@ -171,14 +172,17 @@
                                         hour = 1.23, 
                                         href = '', ), )
                                 ], 
                             available_in_metros = [
                                 equinix_metal.models.plan_available_in_metros_inner.Plan_available_in_metros_inner(
                                     href = '', )
                                 ], 
+                            categories = [
+                                ''
+                                ], 
                             class = 'm3.large.x86', 
                             deployment_types = [
                                 'on_demand'
                                 ], 
                             description = '', 
                             href = '', 
                             id = '',
```

### Comparing `equinix-metal-0.2.1/test/test_device_metro.py` & `equinix-metal-0.2.2/test/test_device_metro.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_device_project.py` & `equinix-metal-0.2.2/test/test_device_project.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_device_project_lite.py` & `equinix-metal-0.2.2/test/test_device_project_lite.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_device_update_input.py` & `equinix-metal-0.2.2/test/test_device_update_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_device_usage.py` & `equinix-metal-0.2.2/test/test_device_usage.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_device_usage_list.py` & `equinix-metal-0.2.2/test/test_device_usage_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_devices_api.py` & `equinix-metal-0.2.2/test/test_devices_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_email.py` & `equinix-metal-0.2.2/test/test_email.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_email_input.py` & `equinix-metal-0.2.2/test/test_email_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_emails_api.py` & `equinix-metal-0.2.2/test/test_emails_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_entitlement.py` & `equinix-metal-0.2.2/test/test_entitlement.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_error.py` & `equinix-metal-0.2.2/test/test_error.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_event.py` & `equinix-metal-0.2.2/test/test_event.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_event_list.py` & `equinix-metal-0.2.2/test/test_event_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_events_api.py` & `equinix-metal-0.2.2/test/test_events_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,14 +79,21 @@
         Retrieve project's events  # noqa: E501
         """
         pass
 
     def test_find_virtual_circuit_events(self):
         """Test case for find_virtual_circuit_events
 
-        Retrieve interconnection events  # noqa: E501
+        Retrieve virtual circuit events  # noqa: E501
+        """
+        pass
+
+    def test_find_vrf_route_events(self):
+        """Test case for find_vrf_route_events
+
+        Retrieve VRF route events  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `equinix-metal-0.2.1/test/test_fabric_service_token.py` & `equinix-metal-0.2.2/test/test_fabric_service_token.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_facilities_api.py` & `equinix-metal-0.2.2/test/test_facilities_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_facility.py` & `equinix-metal-0.2.2/test/test_facility.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
             optional params are included """
         # uncomment below to create an instance of `Facility`
         """
         model = equinix_metal.models.facility.Facility()  # noqa: E501
         if include_optional :
             return Facility(
                 address = equinix_metal.models.address.Address(
-                    address = '', 
                     address2 = '', 
                     city = '', 
                     coordinates = equinix_metal.models.coordinates.Coordinates(
                         href = '', 
                         latitude = '', 
                         longitude = '', ), 
                     country = '',
```

### Comparing `equinix-metal-0.2.1/test/test_facility_input.py` & `equinix-metal-0.2.2/test/test_facility_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_facility_input_facility.py` & `equinix-metal-0.2.2/test/test_facility_input_facility.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_facility_list.py` & `equinix-metal-0.2.2/test/test_facility_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         """
         model = equinix_metal.models.facility_list.FacilityList()  # noqa: E501
         if include_optional :
             return FacilityList(
                 facilities = [
                     equinix_metal.models.facility.Facility(
                         address = equinix_metal.models.address.Address(
-                            address = '', 
                             address2 = '', 
                             city = '', 
                             coordinates = equinix_metal.models.coordinates.Coordinates(
                                 href = '', 
                                 latitude = '', 
                                 longitude = '', ), 
                             country = '',
```

### Comparing `equinix-metal-0.2.1/test/test_find_ip_address_by_id200_response.py` & `equinix-metal-0.2.2/test/test_find_ip_address_by_id200_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,20 +58,22 @@
                     code = '', 
                     country = '', 
                     href = '', 
                     id = '', 
                     name = '', ), 
                 netmask = '', 
                 network = '', 
+                next_hop = '', 
                 parent_block = equinix_metal.models.parent_block.ParentBlock(
                     cidr = 56, 
                     href = '', 
                     netmask = '', 
                     network = '', ), 
                 public = True, 
+                state = '', 
                 addon = True, 
                 assignments = [
                     equinix_metal.models.href.Href(
                         href = '', )
                     ], 
                 available = '', 
                 bill = True, 
@@ -150,15 +152,14 @@
                         ], 
                     updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     volumes = [
                         
                         ], ), 
                 requested_by = equinix_metal.models.href.Href(
                     href = '', ), 
-                state = '', 
                 tags = [
                     ''
                     ], 
                 type = 'vrf', 
                 created_by = equinix_metal.models.href.Href(
                     href = '', ), 
                 vrf = equinix_metal.models.vrf.Vrf(
@@ -168,14 +169,16 @@
                     bill = True, 
                     created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     created_by = equinix_metal.models.user.User(
                         avatar_thumb_url = '', 
                         avatar_url = '', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         customdata = equinix_metal.models.customdata.customdata(), 
+                        default_organization_id = '', 
+                        default_project_id = '', 
                         email = '', 
                         emails = [
                             equinix_metal.models.href.Href(
                                 href = '', )
                             ], 
                         first_name = '', 
                         fraud_score = '', 
@@ -272,14 +275,16 @@
                     bill = True, 
                     created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     created_by = equinix_metal.models.user.User(
                         avatar_thumb_url = '', 
                         avatar_url = '', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         customdata = equinix_metal.models.customdata.customdata(), 
+                        default_organization_id = '', 
+                        default_project_id = '', 
                         email = '', 
                         emails = [
                             equinix_metal.models.href.Href(
                                 href = '', )
                             ], 
                         first_name = '', 
                         fraud_score = '',
```

### Comparing `equinix-metal-0.2.1/test/test_find_metal_gateway_by_id200_response.py` & `equinix-metal-0.2.2/test/test_find_metal_gateway_by_id200_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,14 +225,16 @@
                     bill = True, 
                     created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     created_by = equinix_metal.models.user.User(
                         avatar_thumb_url = '', 
                         avatar_url = '', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         customdata = equinix_metal.models.customdata.customdata(), 
+                        default_organization_id = '', 
+                        default_project_id = '', 
                         email = '', 
                         emails = [
                             equinix_metal.models.href.Href(
                                 href = '', )
                             ], 
                         first_name = '', 
                         fraud_score = '',
```

### Comparing `equinix-metal-0.2.1/test/test_find_traffic_timeframe_parameter.py` & `equinix-metal-0.2.2/test/test_find_traffic_timeframe_parameter.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_global_bgp_range.py` & `equinix-metal-0.2.2/test/test_global_bgp_range.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_global_bgp_range_list.py` & `equinix-metal-0.2.2/test/test_global_bgp_range_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_hardware_reservation.py` & `equinix-metal-0.2.2/test/test_hardware_reservation.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,14 @@
                     bonding_mode = 56, 
                     created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     created_by = null, 
                     customdata = { }, 
                     description = '', 
                     facility = equinix_metal.models.facility.Facility(
                         address = equinix_metal.models.address.Address(
-                            address = '', 
                             address2 = '', 
                             city = '', 
                             coordinates = equinix_metal.models.coordinates.Coordinates(
                                 href = '', 
                                 latitude = '', 
                                 longitude = '', ), 
                             country = '', 
@@ -95,20 +94,22 @@
                             global_ip = True, 
                             href = '', 
                             id = '', 
                             manageable = True, 
                             management = True, 
                             netmask = '', 
                             network = '', 
+                            next_hop = '', 
                             parent_block = equinix_metal.models.parent_block.ParentBlock(
                                 cidr = 56, 
                                 href = '', 
                                 netmask = '', 
                                 network = '', ), 
-                            public = True, )
+                            public = True, 
+                            state = 'pending', )
                         ], 
                     ipxe_script_url = '', 
                     iqn = '', 
                     locked = True, 
                     metro = null, 
                     network_ports = [
                         equinix_metal.models.port.Port(
@@ -172,14 +173,17 @@
                                     hour = 1.23, 
                                     href = '', ), )
                             ], 
                         available_in_metros = [
                             equinix_metal.models.plan_available_in_metros_inner.Plan_available_in_metros_inner(
                                 href = '', )
                             ], 
+                        categories = [
+                            ''
+                            ], 
                         class = 'm3.large.x86', 
                         deployment_types = [
                             'on_demand'
                             ], 
                         description = '', 
                         href = '', 
                         id = '', 
@@ -252,15 +256,14 @@
                     user = '', 
                     userdata = '', 
                     volumes = [
                         
                         ], ), 
                 facility = equinix_metal.models.facility.Facility(
                     address = equinix_metal.models.address.Address(
-                        address = '', 
                         address2 = '', 
                         city = '', 
                         coordinates = equinix_metal.models.coordinates.Coordinates(
                             href = '', 
                             latitude = '', 
                             longitude = '', ), 
                         country = '', 
@@ -285,14 +288,17 @@
                                 hour = 1.23, 
                                 href = '', ), )
                         ], 
                     available_in_metros = [
                         equinix_metal.models.plan_available_in_metros_inner.Plan_available_in_metros_inner(
                             href = '', )
                         ], 
+                    categories = [
+                        ''
+                        ], 
                     class = 'm3.large.x86', 
                     deployment_types = [
                         'on_demand'
                         ], 
                     description = '', 
                     href = '', 
                     id = '',
```

### Comparing `equinix-metal-0.2.1/test/test_hardware_reservation_list.py` & `equinix-metal-0.2.2/test/test_hardware_reservation_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
                             bonding_mode = 56, 
                             created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                             created_by = null, 
                             customdata = { }, 
                             description = '', 
                             facility = equinix_metal.models.facility.Facility(
                                 address = equinix_metal.models.address.Address(
-                                    address = '', 
                                     address2 = '', 
                                     city = '', 
                                     coordinates = equinix_metal.models.coordinates.Coordinates(
                                         href = '', 
                                         latitude = '', 
                                         longitude = '', ), 
                                     country = '', 
@@ -97,20 +96,22 @@
                                     global_ip = True, 
                                     href = '', 
                                     id = '', 
                                     manageable = True, 
                                     management = True, 
                                     netmask = '', 
                                     network = '', 
+                                    next_hop = '', 
                                     parent_block = equinix_metal.models.parent_block.ParentBlock(
                                         cidr = 56, 
                                         href = '', 
                                         netmask = '', 
                                         network = '', ), 
-                                    public = True, )
+                                    public = True, 
+                                    state = 'pending', )
                                 ], 
                             ipxe_script_url = '', 
                             iqn = '', 
                             locked = True, 
                             metro = null, 
                             network_ports = [
                                 equinix_metal.models.port.Port(
@@ -174,14 +175,17 @@
                                             hour = 1.23, 
                                             href = '', ), )
                                     ], 
                                 available_in_metros = [
                                     equinix_metal.models.plan_available_in_metros_inner.Plan_available_in_metros_inner(
                                         href = '', )
                                     ], 
+                                categories = [
+                                    ''
+                                    ], 
                                 class = 'm3.large.x86', 
                                 deployment_types = [
                                     'on_demand'
                                     ], 
                                 description = '', 
                                 href = '', 
                                 id = '',
```

### Comparing `equinix-metal-0.2.1/test/test_hardware_reservations_api.py` & `equinix-metal-0.2.2/test/test_hardware_reservations_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_href.py` & `equinix-metal-0.2.2/test/test_href.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_incidents_api.py` & `equinix-metal-0.2.2/test/test_incidents_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_instances_batch_create_input.py` & `equinix-metal-0.2.2/test/test_instances_batch_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_instances_batch_create_input_batches_inner.py` & `equinix-metal-0.2.2/test/test_instances_batch_create_input_batches_inner.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_instances_batch_create_input_batches_inner_all_of.py` & `equinix-metal-0.2.2/test/test_instances_batch_create_input_batches_inner_all_of.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_interconnection.py` & `equinix-metal-0.2.2/test/test_interconnection.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_interconnection_create_input.py` & `equinix-metal-0.2.2/test/test_interconnection_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_interconnection_list.py` & `equinix-metal-0.2.2/test/test_interconnection_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_interconnection_metro.py` & `equinix-metal-0.2.2/test/test_interconnection_metro.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_interconnection_port.py` & `equinix-metal-0.2.2/test/test_interconnection_port.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_interconnection_port_list.py` & `equinix-metal-0.2.2/test/test_interconnection_port_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_interconnection_update_input.py` & `equinix-metal-0.2.2/test/test_interconnection_update_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_interconnections_api.py` & `equinix-metal-0.2.2/test/test_interconnections_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_invitation.py` & `equinix-metal-0.2.2/test/test_invitation.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_invitation_input.py` & `equinix-metal-0.2.2/test/test_invitation_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_invitation_list.py` & `equinix-metal-0.2.2/test/test_invitation_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_invitations_api.py` & `equinix-metal-0.2.2/test/test_invitations_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_ip_address.py` & `equinix-metal-0.2.2/test/test_ip_address.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_ip_addresses_api.py` & `equinix-metal-0.2.2/test/test_ip_addresses_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_ip_assignment.py` & `equinix-metal-0.2.2/test/test_ip_assignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,20 +53,22 @@
                 href = '', 
                 id = '', 
                 manageable = True, 
                 management = True, 
                 metro = None, 
                 netmask = '', 
                 network = '', 
+                next_hop = '', 
                 parent_block = equinix_metal.models.parent_block.ParentBlock(
                     cidr = 56, 
                     href = '', 
                     netmask = '', 
                     network = '', ), 
-                public = True
+                public = True, 
+                state = 'pending'
             )
         else :
             return IPAssignment(
                 assigned_to = equinix_metal.models.href.Href(
                     href = '', ),
         )
         """
```

### Comparing `equinix-metal-0.2.1/test/test_ip_assignment_input.py` & `equinix-metal-0.2.2/test/test_ip_assignment_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_ip_assignment_list.py` & `equinix-metal-0.2.2/test/test_ip_assignment_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,20 +56,22 @@
                         href = '', 
                         id = '', 
                         manageable = True, 
                         management = True, 
                         metro = null, 
                         netmask = '', 
                         network = '', 
+                        next_hop = '', 
                         parent_block = equinix_metal.models.parent_block.ParentBlock(
                             cidr = 56, 
                             href = '', 
                             netmask = '', 
                             network = '', ), 
-                        public = True, )
+                        public = True, 
+                        state = 'pending', )
                     ]
             )
         else :
             return IPAssignmentList(
         )
         """
```

### Comparing `equinix-metal-0.2.1/test/test_ip_assignment_metro.py` & `equinix-metal-0.2.2/test/test_ip_assignment_metro.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_ip_assignment_update_input.py` & `equinix-metal-0.2.2/test/test_ip_assignment_update_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_ip_availabilities_list.py` & `equinix-metal-0.2.2/test/test_ip_availabilities_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_ip_reservation.py` & `equinix-metal-0.2.2/test/test_ip_reservation.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_ip_reservation_facility.py` & `equinix-metal-0.2.2/test/test_ip_reservation_facility.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
             optional params are included """
         # uncomment below to create an instance of `IPReservationFacility`
         """
         model = equinix_metal.models.ip_reservation_facility.IPReservationFacility()  # noqa: E501
         if include_optional :
             return IPReservationFacility(
                 address = equinix_metal.models.address.Address(
-                    address = '', 
                     address2 = '', 
                     city = '', 
                     coordinates = equinix_metal.models.coordinates.Coordinates(
                         href = '', 
                         latitude = '', 
                         longitude = '', ), 
                     country = '',
```

### Comparing `equinix-metal-0.2.1/test/test_ip_reservation_list.py` & `equinix-metal-0.2.2/test/test_ip_reservation_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_ip_reservation_list_ip_addresses_inner.py` & `equinix-metal-0.2.2/test/test_ip_reservation_list_ip_addresses_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,16 @@
                     bill = True, 
                     created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     created_by = equinix_metal.models.user.User(
                         avatar_thumb_url = '', 
                         avatar_url = '', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         customdata = equinix_metal.models.customdata.customdata(), 
+                        default_organization_id = '', 
+                        default_project_id = '', 
                         email = '', 
                         emails = [
                             equinix_metal.models.href.Href(
                                 href = '', )
                             ], 
                         first_name = '', 
                         fraud_score = '', 
@@ -263,14 +265,16 @@
                     bill = True, 
                     created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     created_by = equinix_metal.models.user.User(
                         avatar_thumb_url = '', 
                         avatar_url = '', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         customdata = equinix_metal.models.customdata.customdata(), 
+                        default_organization_id = '', 
+                        default_project_id = '', 
                         email = '', 
                         emails = [
                             equinix_metal.models.href.Href(
                                 href = '', )
                             ], 
                         first_name = '', 
                         fraud_score = '',
```

### Comparing `equinix-metal-0.2.1/test/test_ip_reservation_metro.py` & `equinix-metal-0.2.2/test/test_ip_reservation_metro.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_ip_reservation_request_input.py` & `equinix-metal-0.2.2/test/test_ip_reservation_request_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_license.py` & `equinix-metal-0.2.2/test/test_license.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_license_create_input.py` & `equinix-metal-0.2.2/test/test_license_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_license_list.py` & `equinix-metal-0.2.2/test/test_license_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_license_update_input.py` & `equinix-metal-0.2.2/test/test_license_update_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_licenses_api.py` & `equinix-metal-0.2.2/test/test_licenses_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_membership.py` & `equinix-metal-0.2.2/test/test_membership.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_membership_input.py` & `equinix-metal-0.2.2/test/test_membership_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_membership_list.py` & `equinix-metal-0.2.2/test/test_membership_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_memberships_api.py` & `equinix-metal-0.2.2/test/test_memberships_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_meta.py` & `equinix-metal-0.2.2/test/test_meta.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_metadata.py` & `equinix-metal-0.2.2/test/test_metadata.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_metadata_network.py` & `equinix-metal-0.2.2/test/test_metadata_network.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_metadata_network_network.py` & `equinix-metal-0.2.2/test/test_metadata_network_network.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_metadata_network_network_bonding.py` & `equinix-metal-0.2.2/test/test_metadata_network_network_bonding.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_metal_gateway.py` & `equinix-metal-0.2.2/test/test_metal_gateway.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_metal_gateway_create_input.py` & `equinix-metal-0.2.2/test/test_metal_gateway_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_metal_gateway_list.py` & `equinix-metal-0.2.2/test/test_metal_gateway_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_metal_gateway_list_metal_gateways_inner.py` & `equinix-metal-0.2.2/test/test_metal_gateway_list_metal_gateways_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,14 +225,16 @@
                     bill = True, 
                     created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     created_by = equinix_metal.models.user.User(
                         avatar_thumb_url = '', 
                         avatar_url = '', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         customdata = equinix_metal.models.customdata.customdata(), 
+                        default_organization_id = '', 
+                        default_project_id = '', 
                         email = '', 
                         emails = [
                             equinix_metal.models.href.Href(
                                 href = '', )
                             ], 
                         first_name = '', 
                         fraud_score = '',
```

### Comparing `equinix-metal-0.2.1/test/test_metal_gateway_lite.py` & `equinix-metal-0.2.2/test/test_metal_gateway_lite.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_metal_gateways_api.py` & `equinix-metal-0.2.2/test/test_metal_gateways_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,21 @@
     def test_create_metal_gateway(self):
         """Test case for create_metal_gateway
 
         Create a metal gateway  # noqa: E501
         """
         pass
 
+    def test_create_metal_gateway_elastic_ip(self):
+        """Test case for create_metal_gateway_elastic_ip
+
+        Create a Metal Gateway Elastic IP  # noqa: E501
+        """
+        pass
+
     def test_delete_metal_gateway(self):
         """Test case for delete_metal_gateway
 
         Deletes the metal gateway  # noqa: E501
         """
         pass
 
@@ -55,10 +62,17 @@
     def test_find_metal_gateways_by_project(self):
         """Test case for find_metal_gateways_by_project
 
         Returns all metal gateways for a project  # noqa: E501
         """
         pass
 
+    def test_get_metal_gateway_elastic_ips(self):
+        """Test case for get_metal_gateway_elastic_ips
+
+        List Metal Gateway Elastic IPs  # noqa: E501
+        """
+        pass
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `equinix-metal-0.2.1/test/test_metro.py` & `equinix-metal-0.2.2/test/test_metro.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_metro_capacity_list.py` & `equinix-metal-0.2.2/test/test_metro_capacity_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_metro_capacity_report.py` & `equinix-metal-0.2.2/test/test_metro_capacity_report.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_metro_input.py` & `equinix-metal-0.2.2/test/test_metro_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_metro_list.py` & `equinix-metal-0.2.2/test/test_metro_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_metro_server_info.py` & `equinix-metal-0.2.2/test/test_metro_server_info.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_metros_api.py` & `equinix-metal-0.2.2/test/test_metros_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_move_hardware_reservation_request.py` & `equinix-metal-0.2.2/test/test_move_hardware_reservation_request.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_new_password.py` & `equinix-metal-0.2.2/test/test_new_password.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_operating_system.py` & `equinix-metal-0.2.2/test/test_operating_system.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_operating_system_list.py` & `equinix-metal-0.2.2/test/test_operating_system_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_operating_systems_api.py` & `equinix-metal-0.2.2/test/test_operating_systems_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_organization.py` & `equinix-metal-0.2.2/test/test_organization.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 credit_amount = 1.337, 
                 customdata = None, 
                 description = '', 
                 enforce_2fa_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 href = '', 
                 id = '', 
-                logo = bytes(b'blah'), 
+                logo = '', 
                 members = [
                     equinix_metal.models.href.Href(
                         href = '', )
                     ], 
                 memberships = [
                     equinix_metal.models.href.Href(
                         href = '', )
```

### Comparing `equinix-metal-0.2.1/test/test_organization_input.py` & `equinix-metal-0.2.2/test/test_organization_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_organization_list.py` & `equinix-metal-0.2.2/test/test_organization_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,41 +53,39 @@
                     next = , 
                     previous = , 
                     self = , 
                     total = 56, ), 
                 organizations = [
                     equinix_metal.models.organization.Organization(
                         address = equinix_metal.models.address.Address(
-                            address = '', 
                             address2 = '', 
                             city = '', 
                             coordinates = equinix_metal.models.coordinates.Coordinates(
                                 href = '', 
                                 latitude = '', 
                                 longitude = '', ), 
                             country = '', 
                             href = '', 
                             state = '', 
                             zip_code = '', ), 
                         billing_address = equinix_metal.models.address.Address(
-                            address = '', 
                             address2 = '', 
                             city = '', 
                             country = '', 
                             href = '', 
                             state = '', 
                             zip_code = '', ), 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         credit_amount = 1.337, 
                         customdata = equinix_metal.models.customdata.customdata(), 
                         description = '', 
                         enforce_2fa_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         href = '', 
                         id = '', 
-                        logo = bytes(b'blah'), 
+                        logo = '', 
                         members = [
                             equinix_metal.models.href.Href(
                                 href = '', )
                             ], 
                         memberships = [
                             equinix_metal.models.href.Href(
                                 href = '', )
```

### Comparing `equinix-metal-0.2.1/test/test_organizations_api.py` & `equinix-metal-0.2.2/test/test_organizations_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_otps_api.py` & `equinix-metal-0.2.2/test/test_otps_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_parent_block.py` & `equinix-metal-0.2.2/test/test_parent_block.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_password_reset_tokens_api.py` & `equinix-metal-0.2.2/test/test_password_reset_tokens_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_payment_method.py` & `equinix-metal-0.2.2/test/test_payment_method.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_payment_method_billing_address.py` & `equinix-metal-0.2.2/test/test_payment_method_billing_address.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_payment_method_create_input.py` & `equinix-metal-0.2.2/test/test_payment_method_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_payment_method_list.py` & `equinix-metal-0.2.2/test/test_payment_method_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_payment_method_update_input.py` & `equinix-metal-0.2.2/test/test_payment_method_update_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_payment_methods_api.py` & `equinix-metal-0.2.2/test/test_payment_methods_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_plan.py` & `equinix-metal-0.2.2/test/test_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,17 @@
                 available_in_metros = [
                     equinix_metal.models.plan_available_in_metros_inner.Plan_available_in_metros_inner(
                         href = '', 
                         price = equinix_metal.models.plan_available_in_inner_price.Plan_available_in_inner_price(
                             hour = 1.23, 
                             href = '', ), )
                     ], 
+                categories = [
+                    ''
+                    ], 
                 var_class = 'm3.large.x86', 
                 deployment_types = [
                     'on_demand'
                     ], 
                 description = '', 
                 href = '', 
                 id = '',
```

### Comparing `equinix-metal-0.2.1/test/test_plan_available_in_inner.py` & `equinix-metal-0.2.2/test/test_plan_available_in_inner.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_plan_available_in_inner_price.py` & `equinix-metal-0.2.2/test/test_plan_available_in_inner_price.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_plan_available_in_metros_inner.py` & `equinix-metal-0.2.2/test/test_plan_available_in_metros_inner.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_plan_list.py` & `equinix-metal-0.2.2/test/test_plan_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,17 @@
                                     hour = 1.23, 
                                     href = '', ), )
                             ], 
                         available_in_metros = [
                             equinix_metal.models.plan_available_in_metros_inner.Plan_available_in_metros_inner(
                                 href = '', )
                             ], 
+                        categories = [
+                            ''
+                            ], 
                         class = 'm3.large.x86', 
                         deployment_types = [
                             'on_demand'
                             ], 
                         description = '', 
                         href = '', 
                         id = '',
```

### Comparing `equinix-metal-0.2.1/test/test_plan_specs.py` & `equinix-metal-0.2.2/test/test_plan_specs.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_plan_specs_cpus_inner.py` & `equinix-metal-0.2.2/test/test_plan_specs_cpus_inner.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_plan_specs_drives_inner.py` & `equinix-metal-0.2.2/test/test_plan_specs_drives_inner.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_plan_specs_features.py` & `equinix-metal-0.2.2/test/test_plan_specs_features.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_plan_specs_nics_inner.py` & `equinix-metal-0.2.2/test/test_plan_specs_nics_inner.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_plans_api.py` & `equinix-metal-0.2.2/test/test_plans_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_port.py` & `equinix-metal-0.2.2/test/test_port.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_port_assign_input.py` & `equinix-metal-0.2.2/test/test_port_assign_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_port_convert_layer3_input.py` & `equinix-metal-0.2.2/test/test_port_convert_layer3_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_port_convert_layer3_input_request_ips_inner.py` & `equinix-metal-0.2.2/test/test_port_convert_layer3_input_request_ips_inner.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_port_data.py` & `equinix-metal-0.2.2/test/test_port_data.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_port_vlan_assignment.py` & `equinix-metal-0.2.2/test/test_port_vlan_assignment.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_port_vlan_assignment_batch.py` & `equinix-metal-0.2.2/test/test_port_vlan_assignment_batch.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_port_vlan_assignment_batch_create_input.py` & `equinix-metal-0.2.2/test/test_port_vlan_assignment_batch_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_port_vlan_assignment_batch_create_input_vlan_assignments_inner.py` & `equinix-metal-0.2.2/test/test_port_vlan_assignment_batch_create_input_vlan_assignments_inner.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_port_vlan_assignment_batch_list.py` & `equinix-metal-0.2.2/test/test_port_vlan_assignment_batch_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_port_vlan_assignment_batch_vlan_assignments_inner.py` & `equinix-metal-0.2.2/test/test_port_vlan_assignment_batch_vlan_assignments_inner.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_port_vlan_assignment_list.py` & `equinix-metal-0.2.2/test/test_port_vlan_assignment_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_ports_api.py` & `equinix-metal-0.2.2/test/test_ports_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_project.py` & `equinix-metal-0.2.2/test/test_project.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_project_create_from_root_input.py` & `equinix-metal-0.2.2/test/test_project_create_from_root_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_project_create_input.py` & `equinix-metal-0.2.2/test/test_project_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_project_list.py` & `equinix-metal-0.2.2/test/test_project_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_project_update_input.py` & `equinix-metal-0.2.2/test/test_project_update_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_project_usage.py` & `equinix-metal-0.2.2/test/test_project_usage.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_project_usage_list.py` & `equinix-metal-0.2.2/test/test_project_usage_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_projects_api.py` & `equinix-metal-0.2.2/test/test_projects_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_recovery_code_list.py` & `equinix-metal-0.2.2/test/test_recovery_code_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_request_ip_reservation201_response.py` & `equinix-metal-0.2.2/test/test_request_ip_reservation201_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,16 @@
                     bill = True, 
                     created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     created_by = equinix_metal.models.user.User(
                         avatar_thumb_url = '', 
                         avatar_url = '', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         customdata = equinix_metal.models.customdata.customdata(), 
+                        default_organization_id = '', 
+                        default_project_id = '', 
                         email = '', 
                         emails = [
                             equinix_metal.models.href.Href(
                                 href = '', )
                             ], 
                         first_name = '', 
                         fraud_score = '', 
@@ -263,14 +265,16 @@
                     bill = True, 
                     created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     created_by = equinix_metal.models.user.User(
                         avatar_thumb_url = '', 
                         avatar_url = '', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         customdata = equinix_metal.models.customdata.customdata(), 
+                        default_organization_id = '', 
+                        default_project_id = '', 
                         email = '', 
                         emails = [
                             equinix_metal.models.href.Href(
                                 href = '', )
                             ], 
                         first_name = '', 
                         fraud_score = '',
```

### Comparing `equinix-metal-0.2.1/test/test_request_ip_reservation_request.py` & `equinix-metal-0.2.2/test/test_request_ip_reservation_request.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_self_service_reservation_item_request.py` & `equinix-metal-0.2.2/test/test_self_service_reservation_item_request.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_self_service_reservation_item_response.py` & `equinix-metal-0.2.2/test/test_self_service_reservation_item_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,17 @@
             return SelfServiceReservationItemResponse(
                 amount = 1.337, 
                 href = '', 
                 id = '', 
                 metro_code = '', 
                 metro_id = '', 
                 metro_name = '', 
+                plan_categories = [
+                    ''
+                    ], 
                 plan_id = '', 
                 plan_name = '', 
                 plan_slug = '', 
                 quantity = 56, 
                 term = ''
             )
         else :
```

### Comparing `equinix-metal-0.2.1/test/test_self_service_reservation_list.py` & `equinix-metal-0.2.2/test/test_self_service_reservation_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,17 @@
                             equinix_metal.models.self_service_reservation_item_response.SelfServiceReservationItemResponse(
                                 amount = 1.337, 
                                 href = '', 
                                 id = '', 
                                 metro_code = '', 
                                 metro_id = '', 
                                 metro_name = '', 
+                                plan_categories = [
+                                    ''
+                                    ], 
                                 plan_id = '', 
                                 plan_name = '', 
                                 plan_slug = '', 
                                 quantity = 56, 
                                 term = '', )
                             ], 
                         notes = '',
```

### Comparing `equinix-metal-0.2.1/test/test_self_service_reservation_response.py` & `equinix-metal-0.2.2/test/test_self_service_reservation_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,17 @@
                     equinix_metal.models.self_service_reservation_item_response.SelfServiceReservationItemResponse(
                         amount = 1.337, 
                         href = '', 
                         id = '', 
                         metro_code = '', 
                         metro_id = '', 
                         metro_name = '', 
+                        plan_categories = [
+                            ''
+                            ], 
                         plan_id = '', 
                         plan_name = '', 
                         plan_slug = '', 
                         quantity = 56, 
                         term = '', )
                     ], 
                 notes = '',
```

### Comparing `equinix-metal-0.2.1/test/test_self_service_reservations_api.py` & `equinix-metal-0.2.2/test/test_self_service_reservations_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_server_info.py` & `equinix-metal-0.2.2/test/test_server_info.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_spot_market_api.py` & `equinix-metal-0.2.2/test/test_spot_market_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_spot_market_prices_list.py` & `equinix-metal-0.2.2/test/test_spot_market_prices_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_spot_market_prices_per_metro_list.py` & `equinix-metal-0.2.2/test/test_spot_market_prices_per_metro_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_spot_market_prices_per_metro_report.py` & `equinix-metal-0.2.2/test/test_spot_market_prices_per_metro_report.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_spot_market_request.py` & `equinix-metal-0.2.2/test/test_spot_market_request.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_spot_market_request_create_input.py` & `equinix-metal-0.2.2/test/test_spot_market_request_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_spot_market_request_create_input_instance_parameters.py` & `equinix-metal-0.2.2/test/test_spot_market_request_create_input_instance_parameters.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_spot_market_request_list.py` & `equinix-metal-0.2.2/test/test_spot_market_request_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_spot_market_request_metro.py` & `equinix-metal-0.2.2/test/test_spot_market_request_metro.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_spot_prices_datapoints.py` & `equinix-metal-0.2.2/test/test_spot_prices_datapoints.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_spot_prices_history_report.py` & `equinix-metal-0.2.2/test/test_spot_prices_history_report.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_spot_prices_per_baremetal.py` & `equinix-metal-0.2.2/test/test_spot_prices_per_baremetal.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_spot_prices_per_facility.py` & `equinix-metal-0.2.2/test/test_spot_prices_per_facility.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_spot_prices_per_new_facility.py` & `equinix-metal-0.2.2/test/test_spot_prices_per_new_facility.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_spot_prices_report.py` & `equinix-metal-0.2.2/test/test_spot_prices_report.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_ssh_key.py` & `equinix-metal-0.2.2/test/test_ssh_key.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_ssh_key_create_input.py` & `equinix-metal-0.2.2/test/test_ssh_key_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_ssh_key_input.py` & `equinix-metal-0.2.2/test/test_ssh_key_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_ssh_key_list.py` & `equinix-metal-0.2.2/test/test_ssh_key_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_ssh_keys_api.py` & `equinix-metal-0.2.2/test/test_ssh_keys_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_support_request_api.py` & `equinix-metal-0.2.2/test/test_support_request_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_support_request_input.py` & `equinix-metal-0.2.2/test/test_support_request_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_transfer_request.py` & `equinix-metal-0.2.2/test/test_transfer_request.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_transfer_request_input.py` & `equinix-metal-0.2.2/test/test_transfer_request_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_transfer_request_list.py` & `equinix-metal-0.2.2/test/test_transfer_request_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_transfer_requests_api.py` & `equinix-metal-0.2.2/test/test_transfer_requests_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_two_factor_auth_api.py` & `equinix-metal-0.2.2/test/test_two_factor_auth_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_update_email_input.py` & `equinix-metal-0.2.2/test/test_update_email_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_usages_api.py` & `equinix-metal-0.2.2/test/test_usages_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_user.py` & `equinix-metal-0.2.2/test/test_user_lite.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,65 +15,54 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import equinix_metal
-from equinix_metal.models.user import User  # noqa: E501
+from equinix_metal.models.user_lite import UserLite  # noqa: E501
 from equinix_metal.rest import ApiException
 
-class TestUser(unittest.TestCase):
-    """User unit test stubs"""
+class TestUserLite(unittest.TestCase):
+    """UserLite unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test User
+        """Test UserLite
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `User`
+        # uncomment below to create an instance of `UserLite`
         """
-        model = equinix_metal.models.user.User()  # noqa: E501
+        model = equinix_metal.models.user_lite.UserLite()  # noqa: E501
         if include_optional :
-            return User(
+            return UserLite(
                 avatar_thumb_url = '', 
-                avatar_url = '', 
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                customdata = equinix_metal.models.customdata.customdata(), 
                 email = '', 
-                emails = [
-                    equinix_metal.models.href.Href(
-                        href = '', )
-                    ], 
                 first_name = '', 
-                fraud_score = '', 
                 full_name = '', 
                 href = '', 
                 id = '', 
-                last_login_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 last_name = '', 
-                max_organizations = 56, 
-                max_projects = 56, 
-                phone_number = '', 
                 short_id = '', 
-                timezone = '', 
-                two_factor_auth = '', 
                 updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
             )
         else :
-            return User(
+            return UserLite(
+                id = '',
+                short_id = '',
         )
         """
 
-    def testUser(self):
-        """Test User"""
+    def testUserLite(self):
+        """Test UserLite"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `equinix-metal-0.2.1/test/test_user_create_input.py` & `equinix-metal-0.2.2/test/test_user_create_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
                         href = '', )
                     ], 
                 first_name = '', 
                 href = '', 
                 invitation_id = '', 
                 last_name = '', 
                 level = '', 
-                locked = True, 
                 nonce = '', 
                 password = '', 
                 phone_number = '', 
                 social_accounts = None, 
                 timezone = '', 
                 title = '', 
                 two_factor_auth = '',
```

### Comparing `equinix-metal-0.2.1/test/test_user_limited.py` & `equinix-metal-0.2.2/test/test_user_limited.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_user_list.py` & `equinix-metal-0.2.2/test/test_user_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,16 @@
                     total = 56, ), 
                 users = [
                     equinix_metal.models.user.User(
                         avatar_thumb_url = '', 
                         avatar_url = '', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         customdata = equinix_metal.models.customdata.customdata(), 
+                        default_organization_id = '', 
+                        default_project_id = '', 
                         email = '', 
                         emails = [
                             equinix_metal.models.href.Href(
                                 href = '', )
                             ], 
                         first_name = '', 
                         fraud_score = '',
```

### Comparing `equinix-metal-0.2.1/test/test_user_lite.py` & `equinix-metal-0.2.2/test/test_user_update_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,54 +15,49 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import equinix_metal
-from equinix_metal.models.user_lite import UserLite  # noqa: E501
+from equinix_metal.models.user_update_input import UserUpdateInput  # noqa: E501
 from equinix_metal.rest import ApiException
 
-class TestUserLite(unittest.TestCase):
-    """UserLite unit test stubs"""
+class TestUserUpdateInput(unittest.TestCase):
+    """UserUpdateInput unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test UserLite
+        """Test UserUpdateInput
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `UserLite`
+        # uncomment below to create an instance of `UserUpdateInput`
         """
-        model = equinix_metal.models.user_lite.UserLite()  # noqa: E501
+        model = equinix_metal.models.user_update_input.UserUpdateInput()  # noqa: E501
         if include_optional :
-            return UserLite(
-                avatar_thumb_url = '', 
-                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                email = '', 
+            return UserUpdateInput(
+                customdata = None, 
                 first_name = '', 
-                full_name = '', 
                 href = '', 
-                id = '', 
                 last_name = '', 
-                short_id = '', 
-                updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
+                password = '', 
+                phone_number = '', 
+                timezone = ''
             )
         else :
-            return UserLite(
-                id = '',
-                short_id = '',
+            return UserUpdateInput(
         )
         """
 
-    def testUserLite(self):
-        """Test UserLite"""
+    def testUserUpdateInput(self):
+        """Test UserUpdateInput"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `equinix-metal-0.2.1/test/test_user_update_input.py` & `equinix-metal-0.2.2/test/test_vrf_virtual_circuit_update_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,49 +15,54 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import equinix_metal
-from equinix_metal.models.user_update_input import UserUpdateInput  # noqa: E501
+from equinix_metal.models.vrf_virtual_circuit_update_input import VrfVirtualCircuitUpdateInput  # noqa: E501
 from equinix_metal.rest import ApiException
 
-class TestUserUpdateInput(unittest.TestCase):
-    """UserUpdateInput unit test stubs"""
+class TestVrfVirtualCircuitUpdateInput(unittest.TestCase):
+    """VrfVirtualCircuitUpdateInput unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test UserUpdateInput
+        """Test VrfVirtualCircuitUpdateInput
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `UserUpdateInput`
+        # uncomment below to create an instance of `VrfVirtualCircuitUpdateInput`
         """
-        model = equinix_metal.models.user_update_input.UserUpdateInput()  # noqa: E501
+        model = equinix_metal.models.vrf_virtual_circuit_update_input.VrfVirtualCircuitUpdateInput()  # noqa: E501
         if include_optional :
-            return UserUpdateInput(
-                customdata = None, 
-                first_name = '', 
+            return VrfVirtualCircuitUpdateInput(
+                customer_ip = '12.0.0.2', 
+                description = '', 
                 href = '', 
-                last_name = '', 
-                password = '', 
-                phone_number = '', 
-                timezone = ''
+                md5 = '', 
+                metal_ip = '12.0.0.1', 
+                name = '', 
+                peer_asn = 56, 
+                speed = '', 
+                subnet = '12.0.0.0/30', 
+                tags = [
+                    ''
+                    ]
             )
         else :
-            return UserUpdateInput(
+            return VrfVirtualCircuitUpdateInput(
         )
         """
 
-    def testUserUpdateInput(self):
-        """Test UserUpdateInput"""
+    def testVrfVirtualCircuitUpdateInput(self):
+        """Test VrfVirtualCircuitUpdateInput"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `equinix-metal-0.2.1/test/test_user_verification_tokens_api.py` & `equinix-metal-0.2.2/test/test_user_verification_tokens_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_userdata.py` & `equinix-metal-0.2.2/test/test_userdata.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_userdata_api.py` & `equinix-metal-0.2.2/test/test_userdata_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_users_api.py` & `equinix-metal-0.2.2/test/test_users_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_verify_email.py` & `equinix-metal-0.2.2/test/test_verify_email.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_virtual_circuit.py` & `equinix-metal-0.2.2/test/test_virtual_circuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,16 @@
                     bill = True, 
                     created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     created_by = equinix_metal.models.user.User(
                         avatar_thumb_url = '', 
                         avatar_url = '', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         customdata = equinix_metal.models.customdata.customdata(), 
+                        default_organization_id = '', 
+                        default_project_id = '', 
                         email = '', 
                         emails = [
                             equinix_metal.models.href.Href(
                                 href = '', )
                             ], 
                         first_name = '', 
                         fraud_score = '',
```

### Comparing `equinix-metal-0.2.1/test/test_virtual_circuit_create_input.py` & `equinix-metal-0.2.2/test/test_virtual_circuit_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_virtual_circuit_list.py` & `equinix-metal-0.2.2/test/test_virtual_circuit_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_virtual_circuit_update_input.py` & `equinix-metal-0.2.2/test/test_virtual_circuit_update_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_virtual_network.py` & `equinix-metal-0.2.2/test/test_virtual_network.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_virtual_network_create_input.py` & `equinix-metal-0.2.2/test/test_virtual_network_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_virtual_network_list.py` & `equinix-metal-0.2.2/test/test_virtual_network_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_vlan_virtual_circuit.py` & `equinix-metal-0.2.2/test/test_vlan_virtual_circuit.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_vlan_virtual_circuit_create_input.py` & `equinix-metal-0.2.2/test/test_vlan_virtual_circuit_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_vlan_virtual_circuit_update_input.py` & `equinix-metal-0.2.2/test/test_vlan_virtual_circuit_update_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_vlans_api.py` & `equinix-metal-0.2.2/test/test_vlans_api.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_vrf.py` & `equinix-metal-0.2.2/test/test_vrf.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,16 @@
                 bill = True, 
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 created_by = equinix_metal.models.user.User(
                     avatar_thumb_url = '', 
                     avatar_url = '', 
                     created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     customdata = equinix_metal.models.customdata.customdata(), 
+                    default_organization_id = '', 
+                    default_project_id = '', 
                     email = '', 
                     emails = [
                         equinix_metal.models.href.Href(
                             href = '', )
                         ], 
                     first_name = '', 
                     fraud_score = '', 
@@ -148,14 +150,16 @@
                             bill = True, 
                             created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                             created_by = equinix_metal.models.user.User(
                                 avatar_thumb_url = '', 
                                 avatar_url = '', 
                                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                                 customdata = equinix_metal.models.customdata.customdata(), 
+                                default_organization_id = '', 
+                                default_project_id = '', 
                                 email = '', 
                                 emails = [
                                     
                                     ], 
                                 first_name = '', 
                                 fraud_score = '', 
                                 full_name = '',
```

### Comparing `equinix-metal-0.2.1/test/test_vrf_create_input.py` & `equinix-metal-0.2.2/test/test_vrf_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_vrf_ip_reservation.py` & `equinix-metal-0.2.2/test/test_vrf_ip_reservation.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,16 @@
                     bill = True, 
                     created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     created_by = equinix_metal.models.user.User(
                         avatar_thumb_url = '', 
                         avatar_url = '', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         customdata = equinix_metal.models.customdata.customdata(), 
+                        default_organization_id = '', 
+                        default_project_id = '', 
                         email = '', 
                         emails = [
                             equinix_metal.models.href.Href(
                                 href = '', )
                             ], 
                         first_name = '', 
                         fraud_score = '', 
@@ -252,14 +254,16 @@
                     bill = True, 
                     created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     created_by = equinix_metal.models.user.User(
                         avatar_thumb_url = '', 
                         avatar_url = '', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         customdata = equinix_metal.models.customdata.customdata(), 
+                        default_organization_id = '', 
+                        default_project_id = '', 
                         email = '', 
                         emails = [
                             equinix_metal.models.href.Href(
                                 href = '', )
                             ], 
                         first_name = '', 
                         fraud_score = '',
```

### Comparing `equinix-metal-0.2.1/test/test_vrf_ip_reservation_create_input.py` & `equinix-metal-0.2.2/test/test_vrf_ip_reservation_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_vrf_ip_reservation_list.py` & `equinix-metal-0.2.2/test/test_vrf_ip_reservation_list.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_vrf_list.py` & `equinix-metal-0.2.2/test/test_vrf_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,16 @@
                         bill = True, 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         created_by = equinix_metal.models.user.User(
                             avatar_thumb_url = '', 
                             avatar_url = '', 
                             created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                             customdata = equinix_metal.models.customdata.customdata(), 
+                            default_organization_id = '', 
+                            default_project_id = '', 
                             email = '', 
                             emails = [
                                 equinix_metal.models.href.Href(
                                     href = '', )
                                 ], 
                             first_name = '', 
                             fraud_score = '',
```

### Comparing `equinix-metal-0.2.1/test/test_vrf_metal_gateway.py` & `equinix-metal-0.2.2/test/test_vrf_metal_gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,14 +225,16 @@
                     bill = True, 
                     created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     created_by = equinix_metal.models.user.User(
                         avatar_thumb_url = '', 
                         avatar_url = '', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         customdata = equinix_metal.models.customdata.customdata(), 
+                        default_organization_id = '', 
+                        default_project_id = '', 
                         email = '', 
                         emails = [
                             equinix_metal.models.href.Href(
                                 href = '', )
                             ], 
                         first_name = '', 
                         fraud_score = '',
```

### Comparing `equinix-metal-0.2.1/test/test_vrf_metal_gateway_create_input.py` & `equinix-metal-0.2.2/test/test_vrf_metal_gateway_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_vrf_route.py` & `equinix-metal-0.2.2/test/test_vrf_route_create_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,53 +15,47 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import equinix_metal
-from equinix_metal.models.vrf_route import VrfRoute  # noqa: E501
+from equinix_metal.models.vrf_route_create_input import VrfRouteCreateInput  # noqa: E501
 from equinix_metal.rest import ApiException
 
-class TestVrfRoute(unittest.TestCase):
-    """VrfRoute unit test stubs"""
+class TestVrfRouteCreateInput(unittest.TestCase):
+    """VrfRouteCreateInput unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test VrfRoute
+        """Test VrfRouteCreateInput
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `VrfRoute`
+        # uncomment below to create an instance of `VrfRouteCreateInput`
         """
-        model = equinix_metal.models.vrf_route.VrfRoute()  # noqa: E501
+        model = equinix_metal.models.vrf_route_create_input.VrfRouteCreateInput()  # noqa: E501
         if include_optional :
-            return VrfRoute(
-                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                href = '/routes/e1ff9c2b-051a-4688-965f-153e274f77e0', 
-                id = 'e1ff9c2b-051a-4688-965f-153e274f77e0', 
-                metal_gateway = None, 
+            return VrfRouteCreateInput(
+                href = '', 
                 next_hop = '192.168.1.254', 
-                prefix = '0.0.0.0/0', 
-                status = 'active', 
-                type = 'static', 
-                updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                virtual_network = None, 
-                vrf = None
+                prefix = '0.0.0.0/0'
             )
         else :
-            return VrfRoute(
+            return VrfRouteCreateInput(
+                next_hop = '192.168.1.254',
+                prefix = '0.0.0.0/0',
         )
         """
 
-    def testVrfRoute(self):
-        """Test VrfRoute"""
+    def testVrfRouteCreateInput(self):
+        """Test VrfRouteCreateInput"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `equinix-metal-0.2.1/test/test_vrf_route_create_input.py` & `equinix-metal-0.2.2/test/test_vrf_update_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,47 +15,52 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import equinix_metal
-from equinix_metal.models.vrf_route_create_input import VrfRouteCreateInput  # noqa: E501
+from equinix_metal.models.vrf_update_input import VrfUpdateInput  # noqa: E501
 from equinix_metal.rest import ApiException
 
-class TestVrfRouteCreateInput(unittest.TestCase):
-    """VrfRouteCreateInput unit test stubs"""
+class TestVrfUpdateInput(unittest.TestCase):
+    """VrfUpdateInput unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test VrfRouteCreateInput
+        """Test VrfUpdateInput
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `VrfRouteCreateInput`
+        # uncomment below to create an instance of `VrfUpdateInput`
         """
-        model = equinix_metal.models.vrf_route_create_input.VrfRouteCreateInput()  # noqa: E501
+        model = equinix_metal.models.vrf_update_input.VrfUpdateInput()  # noqa: E501
         if include_optional :
-            return VrfRouteCreateInput(
+            return VrfUpdateInput(
+                bgp_dynamic_neighbors_bfd_enabled = True, 
+                bgp_dynamic_neighbors_enabled = True, 
+                bgp_dynamic_neighbors_export_route_map = True, 
+                description = '', 
                 href = '', 
-                next_hop = '192.168.1.254', 
-                prefix = '0.0.0.0/0'
+                ip_ranges = [
+                    ''
+                    ], 
+                local_asn = 56, 
+                name = ''
             )
         else :
-            return VrfRouteCreateInput(
-                next_hop = '192.168.1.254',
-                prefix = '0.0.0.0/0',
+            return VrfUpdateInput(
         )
         """
 
-    def testVrfRouteCreateInput(self):
-        """Test VrfRouteCreateInput"""
+    def testVrfUpdateInput(self):
+        """Test VrfUpdateInput"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `equinix-metal-0.2.1/test/test_vrf_route_list.py` & `equinix-metal-0.2.2/test/test_user.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,69 +15,67 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import equinix_metal
-from equinix_metal.models.vrf_route_list import VrfRouteList  # noqa: E501
+from equinix_metal.models.user import User  # noqa: E501
 from equinix_metal.rest import ApiException
 
-class TestVrfRouteList(unittest.TestCase):
-    """VrfRouteList unit test stubs"""
+class TestUser(unittest.TestCase):
+    """User unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test VrfRouteList
+        """Test User
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `VrfRouteList`
+        # uncomment below to create an instance of `User`
         """
-        model = equinix_metal.models.vrf_route_list.VrfRouteList()  # noqa: E501
+        model = equinix_metal.models.user.User()  # noqa: E501
         if include_optional :
-            return VrfRouteList(
+            return User(
+                avatar_thumb_url = '', 
+                avatar_url = '', 
+                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                customdata = equinix_metal.models.customdata.customdata(), 
+                default_organization_id = '', 
+                default_project_id = '', 
+                email = '', 
+                emails = [
+                    equinix_metal.models.href.Href(
+                        href = '', )
+                    ], 
+                first_name = '', 
+                fraud_score = '', 
+                full_name = '', 
                 href = '', 
-                meta = equinix_metal.models.meta.Meta(
-                    current_page = 56, 
-                    first = equinix_metal.models.href.Href(
-                        href = '', ), 
-                    href = '', 
-                    last = equinix_metal.models.href.Href(
-                        href = '', ), 
-                    last_page = 56, 
-                    next = , 
-                    previous = , 
-                    self = , 
-                    total = 56, ), 
-                routes = [
-                    equinix_metal.models.vrf_route.VrfRoute(
-                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        href = '/routes/e1ff9c2b-051a-4688-965f-153e274f77e0', 
-                        id = 'e1ff9c2b-051a-4688-965f-153e274f77e0', 
-                        metal_gateway = null, 
-                        next_hop = '192.168.1.254', 
-                        prefix = '0.0.0.0/0', 
-                        status = 'active', 
-                        type = 'static', 
-                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        virtual_network = null, 
-                        vrf = null, )
-                    ]
+                id = '', 
+                last_login_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                last_name = '', 
+                max_organizations = 56, 
+                max_projects = 56, 
+                phone_number = '', 
+                short_id = '', 
+                timezone = '', 
+                two_factor_auth = '', 
+                updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
             )
         else :
-            return VrfRouteList(
+            return User(
         )
         """
 
-    def testVrfRouteList(self):
-        """Test VrfRouteList"""
+    def testUser(self):
+        """Test User"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `equinix-metal-0.2.1/test/test_vrf_route_metal_gateway.py` & `equinix-metal-0.2.2/test/test_vrf_virtual_circuit.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,74 +15,103 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import equinix_metal
-from equinix_metal.models.vrf_route_metal_gateway import VrfRouteMetalGateway  # noqa: E501
+from equinix_metal.models.vrf_virtual_circuit import VrfVirtualCircuit  # noqa: E501
 from equinix_metal.rest import ApiException
 
-class TestVrfRouteMetalGateway(unittest.TestCase):
-    """VrfRouteMetalGateway unit test stubs"""
+class TestVrfVirtualCircuit(unittest.TestCase):
+    """VrfVirtualCircuit unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test VrfRouteMetalGateway
+        """Test VrfVirtualCircuit
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `VrfRouteMetalGateway`
+        # uncomment below to create an instance of `VrfVirtualCircuit`
         """
-        model = equinix_metal.models.vrf_route_metal_gateway.VrfRouteMetalGateway()  # noqa: E501
+        model = equinix_metal.models.vrf_virtual_circuit.VrfVirtualCircuit()  # noqa: E501
         if include_optional :
-            return VrfRouteMetalGateway(
-                href = '', 
+            return VrfVirtualCircuit(
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                created_by = equinix_metal.models.href.Href(
-                    href = '', ), 
+                customer_ip = '12.0.0.2', 
+                description = '', 
+                href = '', 
                 id = '', 
-                ip_reservation = equinix_metal.models.ip_reservation.IPReservation(
-                    addon = True, 
-                    address = '', 
-                    address_family = 56, 
-                    assignments = [
-                        equinix_metal.models.href.Href(
-                            href = '', )
-                        ], 
-                    available = '', 
+                md5 = '', 
+                metal_ip = '12.0.0.1', 
+                name = '', 
+                nni_vlan = 56, 
+                peer_asn = 56, 
+                port = equinix_metal.models.href.Href(
+                    href = '', ), 
+                project = equinix_metal.models.href.Href(
+                    href = '', ), 
+                speed = 56, 
+                status = '', 
+                subnet = '12.0.0.0/30', 
+                tags = [
+                    ''
+                    ], 
+                updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                vrf = equinix_metal.models.vrf.Vrf(
+                    bgp_dynamic_neighbors_bfd_enabled = True, 
+                    bgp_dynamic_neighbors_enabled = True, 
+                    bgp_dynamic_neighbors_export_route_map = True, 
                     bill = True, 
-                    cidr = 56, 
                     created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    customdata = equinix_metal.models.customdata.customdata(), 
-                    details = '', 
-                    enabled = True, 
-                    facility = null, 
-                    gateway = '', 
-                    global_ip = True, 
+                    created_by = equinix_metal.models.user.User(
+                        avatar_thumb_url = '', 
+                        avatar_url = '', 
+                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        customdata = equinix_metal.models.customdata.customdata(), 
+                        default_organization_id = '', 
+                        default_project_id = '', 
+                        email = '', 
+                        emails = [
+                            equinix_metal.models.href.Href(
+                                href = '', )
+                            ], 
+                        first_name = '', 
+                        fraud_score = '', 
+                        full_name = '', 
+                        href = '', 
+                        id = '', 
+                        last_login_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        last_name = '', 
+                        max_organizations = 56, 
+                        max_projects = 56, 
+                        phone_number = '', 
+                        short_id = '', 
+                        timezone = '', 
+                        two_factor_auth = '', 
+                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ), 
+                    description = '', 
                     href = '', 
                     id = '', 
-                    manageable = True, 
-                    management = True, 
-                    metal_gateway = equinix_metal.models.metal_gateway_lite.MetalGatewayLite(
-                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        gateway_address = '10.1.2.1/27', 
+                    ip_ranges = [
+                        ''
+                        ], 
+                    local_asn = 56, 
+                    metro = equinix_metal.models.metro.Metro(
+                        code = '', 
+                        country = '', 
                         href = '', 
                         id = '', 
-                        state = 'ready', 
-                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        vlan = 1001, ), 
-                    metro = null, 
-                    netmask = '', 
-                    network = '', 
+                        name = '', ), 
+                    name = '', 
                     project = equinix_metal.models.project.Project(
                         backend_transfer_enabled = True, 
                         bgp_config = equinix_metal.models.href.Href(
                             href = '', ), 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         customdata = equinix_metal.models.customdata.customdata(), 
                         devices = [
@@ -107,89 +136,42 @@
                         ssh_keys = [
                             
                             ], 
                         updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         volumes = [
                             
                             ], ), 
-                    project_lite = , 
-                    public = True, 
-                    requested_by = , 
-                    state = '', 
-                    tags = [
-                        ''
-                        ], 
-                    type = 'global_ipv4', ), 
-                project = equinix_metal.models.project.Project(
-                    backend_transfer_enabled = True, 
-                    bgp_config = equinix_metal.models.href.Href(
-                        href = '', ), 
-                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    customdata = equinix_metal.models.customdata.customdata(), 
-                    devices = [
-                        equinix_metal.models.href.Href(
-                            href = '', )
-                        ], 
-                    href = '', 
-                    id = '', 
-                    invitations = [
-                        
-                        ], 
-                    max_devices = equinix_metal.models.max_devices.max_devices(), 
-                    members = [
-                        
-                        ], 
-                    memberships = [
-                        
-                        ], 
-                    name = '', 
-                    network_status = equinix_metal.models.network_status.network_status(), 
-                    organization = , 
-                    payment_method = , 
-                    ssh_keys = [
-                        
-                        ], 
                     updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    volumes = [
-                        
-                        ], ), 
-                state = 'ready', 
-                updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                virtual_network = equinix_metal.models.virtual_network.VirtualNetwork(
-                    assigned_to = equinix_metal.models.href.Href(
-                        href = '', ), 
-                    assigned_to_virtual_circuit = True, 
-                    description = '', 
-                    facility = equinix_metal.models.href.Href(
-                        href = '', ), 
-                    href = '', 
-                    id = '', 
-                    instances = [
-                        
-                        ], 
-                    metal_gateways = [
-                        equinix_metal.models.metal_gateway_lite.MetalGatewayLite(
+                    virtual_circuits = [
+                        equinix_metal.models.vrf_virtual_circuit.VrfVirtualCircuit(
                             created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                            gateway_address = '10.1.2.1/27', 
+                            customer_ip = '12.0.0.2', 
+                            description = '', 
                             href = '', 
                             id = '', 
-                            state = 'ready', 
-                            updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                            vlan = 1001, )
-                        ], 
-                    metro = , 
-                    metro_code = '', 
-                    vxlan = 56, )
+                            md5 = '', 
+                            metal_ip = '12.0.0.1', 
+                            name = '', 
+                            nni_vlan = 56, 
+                            peer_asn = 56, 
+                            port = , 
+                            speed = 56, 
+                            status = '', 
+                            subnet = '12.0.0.0/30', 
+                            tags = [
+                                ''
+                                ], 
+                            updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
+                        ], )
             )
         else :
-            return VrfRouteMetalGateway(
-                href = '',
+            return VrfVirtualCircuit(
         )
         """
 
-    def testVrfRouteMetalGateway(self):
-        """Test VrfRouteMetalGateway"""
+    def testVrfVirtualCircuit(self):
+        """Test VrfVirtualCircuit"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `equinix-metal-0.2.1/test/test_vrf_route_virtual_network.py` & `equinix-metal-0.2.2/test/test_project_id_name.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,69 +15,45 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import equinix_metal
-from equinix_metal.models.vrf_route_virtual_network import VrfRouteVirtualNetwork  # noqa: E501
+from equinix_metal.models.project_id_name import ProjectIdName  # noqa: E501
 from equinix_metal.rest import ApiException
 
-class TestVrfRouteVirtualNetwork(unittest.TestCase):
-    """VrfRouteVirtualNetwork unit test stubs"""
+class TestProjectIdName(unittest.TestCase):
+    """ProjectIdName unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test VrfRouteVirtualNetwork
+        """Test ProjectIdName
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `VrfRouteVirtualNetwork`
+        # uncomment below to create an instance of `ProjectIdName`
         """
-        model = equinix_metal.models.vrf_route_virtual_network.VrfRouteVirtualNetwork()  # noqa: E501
+        model = equinix_metal.models.project_id_name.ProjectIdName()  # noqa: E501
         if include_optional :
-            return VrfRouteVirtualNetwork(
+            return ProjectIdName(
                 href = '', 
-                assigned_to = equinix_metal.models.href.Href(
-                    href = '', ), 
-                assigned_to_virtual_circuit = True, 
-                description = '', 
-                facility = equinix_metal.models.href.Href(
-                    href = '', ), 
                 id = '', 
-                instances = [
-                    equinix_metal.models.href.Href(
-                        href = '', )
-                    ], 
-                metal_gateways = [
-                    equinix_metal.models.metal_gateway_lite.MetalGatewayLite(
-                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        gateway_address = '10.1.2.1/27', 
-                        href = '', 
-                        id = '', 
-                        state = 'ready', 
-                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        vlan = 1001, )
-                    ], 
-                metro = equinix_metal.models.href.Href(
-                    href = '', ), 
-                metro_code = '', 
-                vxlan = 56
+                name = ''
             )
         else :
-            return VrfRouteVirtualNetwork(
-                href = '',
+            return ProjectIdName(
         )
         """
 
-    def testVrfRouteVirtualNetwork(self):
-        """Test VrfRouteVirtualNetwork"""
+    def testProjectIdName(self):
+        """Test ProjectIdName"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `equinix-metal-0.2.1/test/test_vrf_route_vrf.py` & `equinix-metal-0.2.2/test/test_vrf_route_list.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,188 +15,219 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import equinix_metal
-from equinix_metal.models.vrf_route_vrf import VrfRouteVrf  # noqa: E501
+from equinix_metal.models.vrf_route_list import VrfRouteList  # noqa: E501
 from equinix_metal.rest import ApiException
 
-class TestVrfRouteVrf(unittest.TestCase):
-    """VrfRouteVrf unit test stubs"""
+class TestVrfRouteList(unittest.TestCase):
+    """VrfRouteList unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test VrfRouteVrf
+        """Test VrfRouteList
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `VrfRouteVrf`
+        # uncomment below to create an instance of `VrfRouteList`
         """
-        model = equinix_metal.models.vrf_route_vrf.VrfRouteVrf()  # noqa: E501
+        model = equinix_metal.models.vrf_route_list.VrfRouteList()  # noqa: E501
         if include_optional :
-            return VrfRouteVrf(
+            return VrfRouteList(
                 href = '', 
-                bgp_dynamic_neighbors_bfd_enabled = True, 
-                bgp_dynamic_neighbors_enabled = True, 
-                bgp_dynamic_neighbors_export_route_map = True, 
-                bill = True, 
-                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                created_by = equinix_metal.models.user.User(
-                    avatar_thumb_url = '', 
-                    avatar_url = '', 
-                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    customdata = equinix_metal.models.customdata.customdata(), 
-                    email = '', 
-                    emails = [
-                        equinix_metal.models.href.Href(
-                            href = '', )
-                        ], 
-                    first_name = '', 
-                    fraud_score = '', 
-                    full_name = '', 
-                    href = '', 
-                    id = '', 
-                    last_login_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    last_name = '', 
-                    max_organizations = 56, 
-                    max_projects = 56, 
-                    phone_number = '', 
-                    short_id = '', 
-                    timezone = '', 
-                    two_factor_auth = '', 
-                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ), 
-                description = '', 
-                id = '', 
-                ip_ranges = [
-                    ''
-                    ], 
-                local_asn = 56, 
-                metro = equinix_metal.models.metro.Metro(
-                    code = '', 
-                    country = '', 
-                    href = '', 
-                    id = '', 
-                    name = '', ), 
-                name = '', 
-                project = equinix_metal.models.project.Project(
-                    backend_transfer_enabled = True, 
-                    bgp_config = equinix_metal.models.href.Href(
+                meta = equinix_metal.models.meta.Meta(
+                    current_page = 56, 
+                    first = equinix_metal.models.href.Href(
                         href = '', ), 
-                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    customdata = equinix_metal.models.customdata.customdata(), 
-                    devices = [
-                        equinix_metal.models.href.Href(
-                            href = '', )
-                        ], 
                     href = '', 
-                    id = '', 
-                    invitations = [
-                        
-                        ], 
-                    max_devices = equinix_metal.models.max_devices.max_devices(), 
-                    members = [
-                        
-                        ], 
-                    memberships = [
-                        
-                        ], 
-                    name = '', 
-                    network_status = equinix_metal.models.network_status.network_status(), 
-                    organization = , 
-                    payment_method = , 
-                    ssh_keys = [
-                        
-                        ], 
-                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    volumes = [
-                        
-                        ], ), 
-                updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                virtual_circuits = [
-                    equinix_metal.models.vrf_virtual_circuit.VrfVirtualCircuit(
+                    last = equinix_metal.models.href.Href(
+                        href = '', ), 
+                    last_page = 56, 
+                    next = , 
+                    previous = , 
+                    self = , 
+                    total = 56, ), 
+                routes = [
+                    equinix_metal.models.vrf_route.VrfRoute(
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        customer_ip = '12.0.0.2', 
-                        description = '', 
-                        href = '', 
-                        id = '', 
-                        md5 = '', 
-                        metal_ip = '12.0.0.1', 
-                        name = '', 
-                        nni_vlan = 56, 
-                        peer_asn = 56, 
-                        port = equinix_metal.models.href.Href(
-                            href = '', ), 
-                        project = equinix_metal.models.href.Href(
-                            href = '', ), 
-                        speed = 56, 
-                        status = '', 
-                        subnet = '12.0.0.0/30', 
-                        tags = [
-                            ''
-                            ], 
-                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        vrf = equinix_metal.models.vrf.Vrf(
-                            bgp_dynamic_neighbors_bfd_enabled = True, 
-                            bgp_dynamic_neighbors_enabled = True, 
-                            bgp_dynamic_neighbors_export_route_map = True, 
-                            bill = True, 
+                        href = '/routes/e1ff9c2b-051a-4688-965f-153e274f77e0', 
+                        id = 'e1ff9c2b-051a-4688-965f-153e274f77e0', 
+                        metal_gateway = equinix_metal.models.vrf_metal_gateway.VrfMetalGateway(
                             created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                            created_by = equinix_metal.models.user.User(
-                                avatar_thumb_url = '', 
-                                avatar_url = '', 
+                            created_by = equinix_metal.models.href.Href(
+                                href = '', ), 
+                            href = '', 
+                            id = '', 
+                            ip_reservation = equinix_metal.models.vrf_ip_reservation.VrfIpReservation(
+                                address = '', 
+                                address_family = 56, 
+                                bill = True, 
+                                cidr = 56, 
                                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                                 customdata = equinix_metal.models.customdata.customdata(), 
-                                email = '', 
-                                emails = [
+                                details = '', 
+                                gateway = '', 
+                                href = '', 
+                                id = '', 
+                                manageable = True, 
+                                management = True, 
+                                metro = equinix_metal.models.metro.Metro(
+                                    code = '', 
+                                    country = '', 
+                                    href = '', 
+                                    id = '', 
+                                    name = '', ), 
+                                netmask = '', 
+                                network = '', 
+                                project = equinix_metal.models.project.Project(
+                                    backend_transfer_enabled = True, 
+                                    bgp_config = equinix_metal.models.href.Href(
+                                        href = '', ), 
+                                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                                    customdata = equinix_metal.models.customdata.customdata(), 
+                                    devices = [
+                                        
+                                        ], 
+                                    href = '', 
+                                    id = '', 
+                                    invitations = [
+                                        
+                                        ], 
+                                    max_devices = equinix_metal.models.max_devices.max_devices(), 
+                                    members = [
+                                        
+                                        ], 
+                                    memberships = [
+                                        
+                                        ], 
+                                    name = '', 
+                                    network_status = equinix_metal.models.network_status.network_status(), 
+                                    organization = , 
+                                    payment_method = , 
+                                    ssh_keys = [
+                                        
+                                        ], 
+                                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                                    volumes = [
+                                        
+                                        ], ), 
+                                project_lite = equinix_metal.models.project.Project(
+                                    backend_transfer_enabled = True, 
+                                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                                    customdata = equinix_metal.models.customdata.customdata(), 
+                                    href = '', 
+                                    id = '', 
+                                    max_devices = equinix_metal.models.max_devices.max_devices(), 
+                                    name = '', 
+                                    network_status = equinix_metal.models.network_status.network_status(), 
+                                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ), 
+                                public = True, 
+                                state = '', 
+                                tags = [
+                                    ''
+                                    ], 
+                                type = 'vrf', 
+                                vrf = equinix_metal.models.vrf.Vrf(
+                                    bgp_dynamic_neighbors_bfd_enabled = True, 
+                                    bgp_dynamic_neighbors_enabled = True, 
+                                    bgp_dynamic_neighbors_export_route_map = True, 
+                                    bill = True, 
+                                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                                    description = '', 
+                                    href = '', 
+                                    id = '', 
+                                    ip_ranges = [
+                                        ''
+                                        ], 
+                                    local_asn = 56, 
+                                    name = '', 
+                                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                                    virtual_circuits = [
+                                        equinix_metal.models.vrf_virtual_circuit.VrfVirtualCircuit(
+                                            created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                                            customer_ip = '12.0.0.2', 
+                                            description = '', 
+                                            href = '', 
+                                            id = '', 
+                                            md5 = '', 
+                                            metal_ip = '12.0.0.1', 
+                                            name = '', 
+                                            nni_vlan = 56, 
+                                            peer_asn = 56, 
+                                            port = , 
+                                            speed = 56, 
+                                            status = '', 
+                                            subnet = '12.0.0.0/30', 
+                                            updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
+                                        ], ), ), 
+                            project = , 
+                            state = 'ready', 
+                            updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            virtual_network = equinix_metal.models.virtual_network.VirtualNetwork(
+                                assigned_to = , 
+                                assigned_to_virtual_circuit = True, 
+                                description = '', 
+                                facility = , 
+                                href = '', 
+                                id = '', 
+                                instances = [
                                     
                                     ], 
-                                first_name = '', 
-                                fraud_score = '', 
-                                full_name = '', 
+                                metal_gateways = [
+                                    equinix_metal.models.metal_gateway_lite.MetalGatewayLite(
+                                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                                        gateway_address = '10.1.2.1/27', 
+                                        href = '', 
+                                        id = '', 
+                                        state = 'ready', 
+                                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                                        vlan = 1001, )
+                                    ], 
+                                metro_code = '', 
+                                vxlan = 56, ), 
+                            vrf = equinix_metal.models.vrf.Vrf(
+                                bgp_dynamic_neighbors_bfd_enabled = True, 
+                                bgp_dynamic_neighbors_enabled = True, 
+                                bgp_dynamic_neighbors_export_route_map = True, 
+                                bill = True, 
+                                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                                description = '', 
                                 href = '', 
                                 id = '', 
-                                last_login_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                                last_name = '', 
-                                max_organizations = 56, 
-                                max_projects = 56, 
-                                phone_number = '', 
-                                short_id = '', 
-                                timezone = '', 
-                                two_factor_auth = '', 
-                                updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ), 
+                                local_asn = 56, 
+                                name = '', 
+                                updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ), ), 
+                        next_hop = '192.168.1.254', 
+                        prefix = '0.0.0.0/0', 
+                        status = 'active', 
+                        type = 'static', 
+                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        virtual_network = equinix_metal.models.virtual_network.VirtualNetwork(
+                            assigned_to_virtual_circuit = True, 
                             description = '', 
                             href = '', 
                             id = '', 
-                            ip_ranges = [
-                                ''
-                                ], 
-                            local_asn = 56, 
-                            metro = equinix_metal.models.metro.Metro(
-                                code = '', 
-                                country = '', 
-                                href = '', 
-                                id = '', 
-                                name = '', ), 
-                            name = '', 
-                            updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ), )
+                            metro_code = '', 
+                            vxlan = 56, ), 
+                        vrf = , )
                     ]
             )
         else :
-            return VrfRouteVrf(
-                href = '',
+            return VrfRouteList(
         )
         """
 
-    def testVrfRouteVrf(self):
-        """Test VrfRouteVrf"""
+    def testVrfRouteList(self):
+        """Test VrfRouteList"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `equinix-metal-0.2.1/test/test_vrf_update_input.py` & `equinix-metal-0.2.2/test/test_vrf_route_update_input.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,52 +15,45 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import equinix_metal
-from equinix_metal.models.vrf_update_input import VrfUpdateInput  # noqa: E501
+from equinix_metal.models.vrf_route_update_input import VrfRouteUpdateInput  # noqa: E501
 from equinix_metal.rest import ApiException
 
-class TestVrfUpdateInput(unittest.TestCase):
-    """VrfUpdateInput unit test stubs"""
+class TestVrfRouteUpdateInput(unittest.TestCase):
+    """VrfRouteUpdateInput unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test VrfUpdateInput
+        """Test VrfRouteUpdateInput
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `VrfUpdateInput`
+        # uncomment below to create an instance of `VrfRouteUpdateInput`
         """
-        model = equinix_metal.models.vrf_update_input.VrfUpdateInput()  # noqa: E501
+        model = equinix_metal.models.vrf_route_update_input.VrfRouteUpdateInput()  # noqa: E501
         if include_optional :
-            return VrfUpdateInput(
-                bgp_dynamic_neighbors_bfd_enabled = True, 
-                bgp_dynamic_neighbors_enabled = True, 
-                bgp_dynamic_neighbors_export_route_map = True, 
-                description = '', 
+            return VrfRouteUpdateInput(
                 href = '', 
-                ip_ranges = [
-                    ''
-                    ], 
-                local_asn = 56, 
-                name = ''
+                next_hop = '192.168.1.254', 
+                prefix = '0.0.0.0/0'
             )
         else :
-            return VrfUpdateInput(
+            return VrfRouteUpdateInput(
         )
         """
 
-    def testVrfUpdateInput(self):
-        """Test VrfUpdateInput"""
+    def testVrfRouteUpdateInput(self):
+        """Test VrfRouteUpdateInput"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `equinix-metal-0.2.1/test/test_vrf_virtual_circuit_create_input.py` & `equinix-metal-0.2.2/test/test_vrf_virtual_circuit_create_input.py`

 * *Files identical despite different names*

### Comparing `equinix-metal-0.2.1/test/test_vrf_virtual_circuit_update_input.py` & `equinix-metal-0.2.2/test/test_metal_gateway_elastic_ip_create_input.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,54 +15,49 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import equinix_metal
-from equinix_metal.models.vrf_virtual_circuit_update_input import VrfVirtualCircuitUpdateInput  # noqa: E501
+from equinix_metal.models.metal_gateway_elastic_ip_create_input import MetalGatewayElasticIpCreateInput  # noqa: E501
 from equinix_metal.rest import ApiException
 
-class TestVrfVirtualCircuitUpdateInput(unittest.TestCase):
-    """VrfVirtualCircuitUpdateInput unit test stubs"""
+class TestMetalGatewayElasticIpCreateInput(unittest.TestCase):
+    """MetalGatewayElasticIpCreateInput unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test VrfVirtualCircuitUpdateInput
+        """Test MetalGatewayElasticIpCreateInput
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `VrfVirtualCircuitUpdateInput`
+        # uncomment below to create an instance of `MetalGatewayElasticIpCreateInput`
         """
-        model = equinix_metal.models.vrf_virtual_circuit_update_input.VrfVirtualCircuitUpdateInput()  # noqa: E501
+        model = equinix_metal.models.metal_gateway_elastic_ip_create_input.MetalGatewayElasticIpCreateInput()  # noqa: E501
         if include_optional :
-            return VrfVirtualCircuitUpdateInput(
-                customer_ip = '12.0.0.2', 
-                description = '', 
+            return MetalGatewayElasticIpCreateInput(
+                address = '147.75.234.8/31', 
+                customdata = { }, 
                 href = '', 
-                md5 = '', 
-                metal_ip = '12.0.0.1', 
-                name = '', 
-                peer_asn = 56, 
-                speed = '', 
-                subnet = '12.0.0.0/30', 
-                tags = [
-                    ''
-                    ]
+                next_hop = '192.168.12.13', 
+                tags = ["NY","prod","public"]
             )
         else :
-            return VrfVirtualCircuitUpdateInput(
+            return MetalGatewayElasticIpCreateInput(
+                address = '147.75.234.8/31',
+                next_hop = '192.168.12.13',
         )
         """
 
-    def testVrfVirtualCircuitUpdateInput(self):
-        """Test VrfVirtualCircuitUpdateInput"""
+    def testMetalGatewayElasticIpCreateInput(self):
+        """Test MetalGatewayElasticIpCreateInput"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `equinix-metal-0.2.1/test/test_vrfs_api.py` & `equinix-metal-0.2.2/test/test_vrfs_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,28 +27,49 @@
 
     def setUp(self):
         self.api = equinix_metal.api.vrfs_api.VRFsApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
+    def test_bgp_dynamic_neighbors_id_get(self):
+        """Test case for bgp_dynamic_neighbors_id_get
+
+        Retrieve a BGP Dynamic Neighbor  # noqa: E501
+        """
+        pass
+
+    def test_create_bgp_dynamic_neighbor(self):
+        """Test case for create_bgp_dynamic_neighbor
+
+        Create a VRF BGP Dynamic Neighbor range  # noqa: E501
+        """
+        pass
+
     def test_create_vrf(self):
         """Test case for create_vrf
 
         Create a new VRF in the specified project  # noqa: E501
         """
         pass
 
     def test_create_vrf_route(self):
         """Test case for create_vrf_route
 
         Create a VRF route  # noqa: E501
         """
         pass
 
+    def test_delete_bgp_dynamic_neighbor_by_id(self):
+        """Test case for delete_bgp_dynamic_neighbor_by_id
+
+        Delete a VRF BGP Dynamic Neighbor  # noqa: E501
+        """
+        pass
+
     def test_delete_vrf(self):
         """Test case for delete_vrf
 
         Delete the VRF  # noqa: E501
         """
         pass
 
@@ -90,14 +111,21 @@
     def test_find_vrfs(self):
         """Test case for find_vrfs
 
         Retrieve all VRFs in the project  # noqa: E501
         """
         pass
 
+    def test_get_bgp_dynamic_neighbors(self):
+        """Test case for get_bgp_dynamic_neighbors
+
+        List BGP Dynamic Neighbors  # noqa: E501
+        """
+        pass
+
     def test_get_vrf_routes(self):
         """Test case for get_vrf_routes
 
         Retrieve all routes in the VRF  # noqa: E501
         """
         pass
```

