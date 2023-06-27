# Comparing `tmp/ntc_templates-3.4.0.tar.gz` & `tmp/ntc_templates-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntc_templates-3.4.0.tar", max compression
+gzip compressed data, was "ntc_templates-3.5.0.tar", max compression
```

## Comparing `ntc_templates-3.4.0.tar` & `ntc_templates-3.5.0.tar`

### file list

```diff
@@ -1,592 +1,594 @@
--rw-r--r--   0        0        0      601 2023-06-11 21:19:30.876631 ntc_templates-3.4.0/LICENSE
--rw-r--r--   0        0        0     2842 2023-06-11 21:19:30.876631 ntc_templates-3.4.0/README.md
--rw-r--r--   0        0        0      260 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/__init__.py
--rw-r--r--   0        0        0     2180 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/parse.py
--rw-r--r--   0        0        0      700 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_aos_show_vlan.textfsm
--rw-r--r--   0        0        0      170 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_oam_mac-ping.textfsm
--rw-r--r--   0        0        0      371 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_lag.textfsm
--rw-r--r--   0        0        0      641 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_port.textfsm
--rw-r--r--   0        0        0      434 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_bgp_routes_vpn-ipv4.textfsm
--rw-r--r--   0        0        0      526 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_bgp_summary_family.textfsm
--rw-r--r--   0        0        0      662 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_interface.textfsm
--rw-r--r--   0        0        0      318 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_isis_adjacency.textfsm
--rw-r--r--   0        0        0      336 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_isis_interface.textfsm
--rw-r--r--   0        0        0      619 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_ldp_interface.textfsm
--rw-r--r--   0        0        0      608 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_mpls_interface.textfsm
--rw-r--r--   0        0        0      512 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_mpls_lsp.textfsm
--rw-r--r--   0        0        0      547 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_ospf_interface.textfsm
--rw-r--r--   0        0        0      425 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_pim_interface.textfsm
--rw-r--r--   0        0        0      649 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_rsvp_interface.textfsm
--rw-r--r--   0        0        0      544 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_service_id_base.textfsm
--rw-r--r--   0        0        0      665 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_service_sap-using.textfsm
--rw-r--r--   0        0        0      598 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_service_sdp-using.textfsm
--rw-r--r--   0        0        0      642 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_service_sdp.textfsm
--rw-r--r--   0        0        0      522 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_system_cpu.textfsm
--rw-r--r--   0        0        0      371 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_bash_df_-h.textfsm
--rw-r--r--   0        0        0      430 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_dir_flash.textfsm
--rw-r--r--   0        0        0      121 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_boot-config.textfsm
--rw-r--r--   0        0        0      226 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_clock.textfsm
--rw-r--r--   0        0        0      524 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_environment_cooling.textfsm
--rw-r--r--   0        0        0      525 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_environment_temperature.textfsm
--rw-r--r--   0        0        0      107 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_hostname.textfsm
--rw-r--r--   0        0        0      888 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_interfaces.textfsm
--rw-r--r--   0        0        0      427 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_interfaces_description.textfsm
--rw-r--r--   0        0        0      399 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_interfaces_status.textfsm
--rw-r--r--   0        0        0      313 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_interfaces_transceiver.textfsm
--rw-r--r--   0        0        0      757 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_interfaces_transceiver_detail.textfsm
--rw-r--r--   0        0        0      666 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_inventory.textfsm
--rw-r--r--   0        0        0      517 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_access-lists.textfsm
--rw-r--r--   0        0        0      159 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_arp.textfsm
--rw-r--r--   0        0        0      651 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_bgp.textfsm
--rw-r--r--   0        0        0     1568 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_bgp_summary.textfsm
--rw-r--r--   0        0        0      246 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_helper-address.textfsm
--rw-r--r--   0        0        0      169 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_interface_brief.textfsm
--rw-r--r--   0        0        0      736 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_ospf_database.textfsm
--rw-r--r--   0        0        0      387 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_ospf_interface_brief.textfsm
--rw-r--r--   0        0        0      462 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_ospf_neighbor.textfsm
--rw-r--r--   0        0        0      734 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_ospf_summary.textfsm
--rw-r--r--   0        0        0     1035 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_route.textfsm
--rw-r--r--   0        0        0     1101 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ipv6_bgp_summary.textfsm
--rw-r--r--   0        0        0      358 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_isis_neighbors.textfsm
--rw-r--r--   0        0        0      190 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_lldp_neighbors.textfsm
--rw-r--r--   0        0        0      627 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_lldp_neighbors_detail.textfsm
--rw-r--r--   0        0        0     1662 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_mac_address-table.textfsm
--rw-r--r--   0        0        0      257 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_mac_security_interface.textfsm
--rw-r--r--   0        0        0      303 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_mac_security_mka_counters.textfsm
--rw-r--r--   0        0        0     1431 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_mac_security_participants_detail.textfsm
--rw-r--r--   0        0        0      279 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_mlag.textfsm
--rw-r--r--   0        0        0      716 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_module.textfsm
--rw-r--r--   0        0        0      557 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_pim_ipv4_interface.textfsm
--rw-r--r--   0        0        0      403 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_pim_ipv4_neighbor.textfsm
--rw-r--r--   0        0        0     1222 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_port-channel_summary.textfsm
--rw-r--r--   0        0        0     5405 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_processes_top_once.textfsm
--rw-r--r--   0        0        0      573 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_reload_cause.textfsm
--rw-r--r--   0        0        0      275 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_snmp_community.textfsm
--rw-r--r--   0        0        0      424 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_version.textfsm
--rw-r--r--   0        0        0     6187 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_vlan.textfsm
--rw-r--r--   0        0        0     4153 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_vrf.textfsm
--rw-r--r--   0        0        0      701 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_aaa_authentication_port-access_interface_all_client-status.textfsm
--rw-r--r--   0        0        0      322 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_arp_all-vrfs.textfsm
--rw-r--r--   0        0        0      596 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_bfd_all-vrfs.textfsm
--rw-r--r--   0        0        0      531 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_bgp_all-vrfs_all_summary.textfsm
--rw-r--r--   0        0        0      531 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_bgp_all_all-vrfs_summary.textfsm
--rw-r--r--   0        0        0     2201 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_interface.textfsm
--rw-r--r--   0        0        0     4761 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_interface_dom_detail.textfsm
--rw-r--r--   0        0        0      348 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_ip_route_all-vrfs.textfsm
--rw-r--r--   0        0        0      827 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_lldp_neighbors-info_detail.textfsm
--rw-r--r--   0        0        0      240 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_mac-address-table.textfsm
--rw-r--r--   0        0        0      380 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_ntp_associations.textfsm
--rw-r--r--   0        0        0      662 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_vsf_detail.textfsm
--rw-r--r--   0        0        0      917 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_ap_bss-table_details.textfsm
--rw-r--r--   0        0        0      768 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_ap_database.textfsm
--rw-r--r--   0        0        0     1028 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_ap_database_long.textfsm
--rw-r--r--   0        0        0      977 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_ap_radio-database.textfsm
--rw-r--r--   0        0        0      735 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_arp.textfsm
--rw-r--r--   0        0        0      176 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_ip_interface_brief.textfsm
--rw-r--r--   0        0        0      287 2023-06-11 21:19:30.880631 ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_ipv6_interface_brief.textfsm
--rw-r--r--   0        0        0      119 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_interface_name.textfsm
--rw-r--r--   0        0        0      702 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_logging_config.textfsm
--rw-r--r--   0        0        0      181 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_mac-address-table.textfsm
--rw-r--r--   0        0        0      878 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_mlt.textfsm
--rw-r--r--   0        0        0      607 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_mlt_all-members.textfsm
--rw-r--r--   0        0        0     1825 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_sys-info.textfsm
--rw-r--r--   0        0        0      470 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_vlan.textfsm
--rw-r--r--   0        0        0      367 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/avaya_vsp_show_software.textfsm
--rw-r--r--   0        0        0      583 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/broadcom_icos_show_isdp_neighbors.textfsm
--rw-r--r--   0        0        0      631 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/broadcom_icos_show_lldp_remote-device_all.textfsm
--rw-r--r--   0        0        0      458 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/broadcom_icos_show_mac-addr-table.textfsm
--rw-r--r--   0        0        0     1497 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/broadcom_icos_show_version.textfsm
--rw-r--r--   0        0        0      372 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/broadcom_icos_show_vlan_brief.textfsm
--rw-r--r--   0        0        0      358 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_arp.textfsm
--rw-r--r--   0        0        0     5683 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_interfaces.textfsm
--rw-r--r--   0        0        0      695 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_interfaces_brief.textfsm
--rw-r--r--   0        0        0      367 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_lag_brief.textfsm
--rw-r--r--   0        0        0      416 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_lldp_neighbors.textfsm
--rw-r--r--   0        0        0      906 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_lldp_neighbors_detail.textfsm
--rw-r--r--   0        0        0      375 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_mac-address.textfsm
--rw-r--r--   0        0        0     1120 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_metro.textfsm
--rw-r--r--   0        0        0      301 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_monitor.textfsm
--rw-r--r--   0        0        0     2278 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_running-config_vlan.textfsm
--rw-r--r--   0        0        0      851 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_span.textfsm
--rw-r--r--   0        0        0      351 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_topo.textfsm
--rw-r--r--   0        0        0     2990 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_trunk.textfsm
--rw-r--r--   0        0        0     1629 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_version.textfsm
--rw-r--r--   0        0        0     6614 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_interfaces.textfsm
--rw-r--r--   0        0        0      430 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_interfaces_brief.textfsm
--rw-r--r--   0        0        0      367 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_lag_brief.textfsm
--rw-r--r--   0        0        0      906 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_lldp_neighbors_detail.textfsm
--rw-r--r--   0        0        0     1071 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_metro.textfsm
--rw-r--r--   0        0        0      311 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_monitor_actual.textfsm
--rw-r--r--   0        0        0     1618 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_running-config_interface.textfsm
--rw-r--r--   0        0        0     2277 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_running-config_vlan.textfsm
--rw-r--r--   0        0        0      739 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_span.textfsm
--rw-r--r--   0        0        0      591 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_topo.textfsm
--rw-r--r--   0        0        0      167 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_fw_stat.textfsm
--rw-r--r--   0        0        0      170 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_arp_dynamic_all.textfsm
--rw-r--r--   0        0        0      148 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_asset_all.textfsm
--rw-r--r--   0        0        0      189 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_dns.textfsm
--rw-r--r--   0        0        0       71 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_domainname.textfsm
--rw-r--r--   0        0        0      786 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_interfaces_all.textfsm
--rw-r--r--   0        0        0      482 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_ipv6_route.textfsm
--rw-r--r--   0        0        0      159 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_lom.textfsm
--rw-r--r--   0        0        0      208 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_ntp_servers.textfsm
--rw-r--r--   0        0        0      550 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_route.textfsm
--rw-r--r--   0        0        0      236 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_version_all.textfsm
--rw-r--r--   0        0        0      419 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_chassis_show_temperature.textfsm
--rw-r--r--   0        0        0     1010 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_port_show.textfsm
--rw-r--r--   0        0        0      945 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_rstp_show.textfsm
--rw-r--r--   0        0        0      623 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_software_show.textfsm
--rw-r--r--   0        0        0      289 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_ssh_server_show_key.textfsm
--rw-r--r--   0        0        0      556 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_traffic-profiling_standard-profile_show.textfsm
--rw-r--r--   0        0        0      636 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_vlan_show.textfsm
--rw-r--r--   0        0        0      714 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_apic_fabric_show_vlan_extended.textfsm
--rw-r--r--   0        0        0      663 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_dir.textfsm
--rw-r--r--   0        0        0      661 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_ping.textfsm
--rw-r--r--   0        0        0     4925 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_access-list.textfsm
--rw-r--r--   0        0        0      325 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_arp.textfsm
--rw-r--r--   0        0        0     9761 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_asp_drop.textfsm
--rw-r--r--   0        0        0      829 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_asp_table_vpn-context_detail.textfsm
--rw-r--r--   0        0        0     1377 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_bgp_summary.textfsm
--rw-r--r--   0        0        0      917 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_cpu_usage_detailed.textfsm
--rw-r--r--   0        0        0      438 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_crypto_ikev1_sa_detail.textfsm
--rw-r--r--   0        0        0     6136 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_crypto_ipsec_sa.textfsm
--rw-r--r--   0        0        0     3036 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_failover.textfsm
--rw-r--r--   0        0        0     4402 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_interface.textfsm
--rw-r--r--   0        0        0     7080 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_interface_detail.textfsm
--rw-r--r--   0        0        0      268 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_interface_ip_brief.textfsm
--rw-r--r--   0        0        0      320 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_inventory.textfsm
--rw-r--r--   0        0        0     4240 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_license_all.textfsm
--rw-r--r--   0        0        0     2352 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_logging.textfsm
--rw-r--r--   0        0        0       89 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_name.textfsm
--rw-r--r--   0        0        0     1624 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_nat.textfsm
--rw-r--r--   0        0        0      561 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_object-group_network.textfsm
--rw-r--r--   0        0        0      403 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_ospf_interface_brief.textfsm
--rw-r--r--   0        0        0      374 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_ospf_neighbor.textfsm
--rw-r--r--   0        0        0     1208 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_port-channel_summary.textfsm
--rw-r--r--   0        0        0      425 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_resource_usage.textfsm
--rw-r--r--   0        0        0     1606 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_route.textfsm
--rw-r--r--   0        0        0     2300 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_running-config_all_crypto_map.textfsm
--rw-r--r--   0        0        0      437 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_running-config_crypto_ikev1.textfsm
--rw-r--r--   0        0        0     1212 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_running-config_crypto_map.textfsm
--rw-r--r--   0        0        0     1726 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_running-config_ipsec.textfsm
--rw-r--r--   0        0        0      474 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_running-config_object_network.textfsm
--rw-r--r--   0        0        0     4906 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_running-config_tunnel-group.textfsm
--rw-r--r--   0        0        0      967 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_version.textfsm
--rw-r--r--   0        0        0     1625 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb.textfsm
--rw-r--r--   0        0        0     1822 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_anyconnect.textfsm
--rw-r--r--   0        0        0     7479 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_detail_l2l.textfsm
--rw-r--r--   0        0        0     1126 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_xlate.textfsm
--rw-r--r--   0        0        0      481 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_dir.textfsm
--rw-r--r--   0        0        0      859 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_ping.textfsm
--rw-r--r--   0        0        0     1584 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_access-list.textfsm
--rw-r--r--   0        0        0      416 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_access-session.textfsm
--rw-r--r--   0        0        0      953 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_adjacency.textfsm
--rw-r--r--   0        0        0      355 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_alert_counters.textfsm
--rw-r--r--   0        0        0      310 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_aliases.textfsm
--rw-r--r--   0        0        0      523 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ap_summary.textfsm
--rw-r--r--   0        0        0      615 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_archive.textfsm
--rw-r--r--   0        0        0      403 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_authentication_sessions.textfsm
--rw-r--r--   0        0        0     2496 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_bfd_neighbors_details.textfsm
--rw-r--r--   0        0        0     1700 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_boot.textfsm
--rw-r--r--   0        0        0      264 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_capability_feature_routing.textfsm
--rw-r--r--   0        0        0      538 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors.textfsm
--rw-r--r--   0        0        0      937 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors_detail.textfsm
--rw-r--r--   0        0        0      317 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_clock.textfsm
--rw-r--r--   0        0        0     2327 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_controller_t1.textfsm
--rw-r--r--   0        0        0     6120 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_crypto_ipsec_sa_detail.textfsm
--rw-r--r--   0        0        0     2174 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_crypto_pki_certificates.textfsm
--rw-r--r--   0        0        0     1418 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_crypto_session_detail.textfsm
--rw-r--r--   0        0        0     1041 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_dhcp_lease.textfsm
--rw-r--r--   0        0        0      491 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_dmvpn.textfsm
--rw-r--r--   0        0        0     1367 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_dot1x_all.textfsm
--rw-r--r--   0        0        0      413 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_environment_power_all.textfsm
--rw-r--r--   0        0        0     1603 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_environment_temperature.textfsm
--rw-r--r--   0        0        0     1188 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_etherchannel_summary.textfsm
--rw-r--r--   0        0        0      454 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_hosts_summary.textfsm
--rw-r--r--   0        0        0     1226 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_interface_link.textfsm
--rw-r--r--   0        0        0      312 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_interface_transceiver.textfsm
--rw-r--r--   0        0        0     2729 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_interfaces.textfsm
--rw-r--r--   0        0        0      409 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_interfaces_description.textfsm
--rw-r--r--   0        0        0      898 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_interfaces_status.textfsm
--rw-r--r--   0        0        0     1512 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_interfaces_switchport.textfsm
--rw-r--r--   0        0        0      570 2023-06-11 21:19:30.884631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_inventory.textfsm
--rw-r--r--   0        0        0     2587 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_access-lists.textfsm
--rw-r--r--   0        0        0      525 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_arp.textfsm
--rw-r--r--   0        0        0     2029 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_bgp.textfsm
--rw-r--r--   0        0        0     1706 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors.textfsm
--rw-r--r--   0        0        0     2011 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors_advertised-routes.textfsm
--rw-r--r--   0        0        0      589 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_bgp_summary.textfsm
--rw-r--r--   0        0        0     1761 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_bgp_vpnv4_all_neighbors.textfsm
--rw-r--r--   0        0        0     1207 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_cef.textfsm
--rw-r--r--   0        0        0     3244 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_cef_detail.textfsm
--rw-r--r--   0        0        0      711 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_device_tracking_all.textfsm
--rw-r--r--   0        0        0     2669 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_interfaces_detail.textfsm
--rw-r--r--   0        0        0      773 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_neighbors.textfsm
--rw-r--r--   0        0        0     2597 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_topology.textfsm
--rwxr-xr-x   0        0        0      459 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_flow_toptalkers.textfsm
--rw-r--r--   0        0        0     4260 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_http_server_status.textfsm
--rw-r--r--   0        0        0     1909 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_interface.textfsm
--rw-r--r--   0        0        0      288 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_interface_brief.textfsm
--rw-r--r--   0        0        0     1378 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_mroute.textfsm
--rw-r--r--   0        0        0      645 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_nat_translations.textfsm
--rw-r--r--   0        0        0      778 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database.textfsm
--rw-r--r--   0        0        0     1362 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_network.textfsm
--rw-r--r--   0        0        0     1807 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_router.textfsm
--rw-r--r--   0        0        0      396 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_ospf_interface_brief.textfsm
--rw-r--r--   0        0        0      383 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_ospf_neighbor.textfsm
--rw-r--r--   0        0        0      436 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_prefix-list.textfsm
--rw-r--r--   0        0        0     2499 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_route.textfsm
--rw-r--r--   0        0        0     1389 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_route_summary.textfsm
--rw-r--r--   0        0        0      555 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_source_binding.textfsm
--rw-r--r--   0        0        0      472 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_vrf_interfaces.textfsm
--rw-r--r--   0        0        0      917 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ipv6_access-lists.textfsm
--rw-r--r--   0        0        0      399 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ipv6_interface_brief.textfsm
--rw-r--r--   0        0        0      371 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ipv6_neighbors.textfsm
--rw-r--r--   0        0        0      523 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ipv6_route.textfsm
--rw-r--r--   0        0        0      956 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_isdn_status.textfsm
--rw-r--r--   0        0        0      412 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_isis_neighbors.textfsm
--rw-r--r--   0        0        0      547 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_license.textfsm
--rw-r--r--   0        0        0      479 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_lldp_neighbors.textfsm
--rw-r--r--   0        0        0     2655 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_lldp_neighbors_detail.textfsm
--rw-r--r--   0        0        0     5593 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_logging.textfsm
--rw-r--r--   0        0        0     4086 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_mac-address-table.textfsm
--rw-r--r--   0        0        0     1017 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_module.textfsm
--rw-r--r--   0        0        0      585 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_module_online_diag.textfsm
--rw-r--r--   0        0        0     1062 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_module_status.textfsm
--rw-r--r--   0        0        0      760 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_module_submodule.textfsm
--rw-r--r--   0        0        0      350 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_mpls_interfaces.textfsm
--rw-r--r--   0        0        0      377 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_nve_peers.textfsm
--rw-r--r--   0        0        0      346 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_nve_vni.textfsm
--rw-r--r--   0        0        0     1215 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_object-group.textfsm
--rw-r--r--   0        0        0     1072 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_platform_diag.textfsm
--rw-r--r--   0        0        0      974 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_port-security_interface_interface.textfsm
--rw-r--r--   0        0        0      922 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_power_available.textfsm
--rw-r--r--   0        0        0      684 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_power_status.textfsm
--rw-r--r--   0        0        0      314 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_power_supplies.textfsm
--rw-r--r--   0        0        0      344 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_processes_cpu.textfsm
--rw-r--r--   0        0        0      640 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_processes_memory_sorted.textfsm
--rw-r--r--   0        0        0     3950 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_redundancy.textfsm
--rw-r--r--   0        0        0      784 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_route-map.textfsm
--rw-r--r--   0        0        0     3318 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_running-config_partition_access-list.textfsm
--rw-r--r--   0        0        0     1034 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_running-config_partition_route-map.textfsm
--rw-r--r--   0        0        0      359 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_snmp_community.textfsm
--rw-r--r--   0        0        0      802 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_snmp_group.textfsm
--rw-r--r--   0        0        0      668 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_snmp_user.textfsm
--rw-r--r--   0        0        0      413 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_spanning-tree.textfsm
--rw-r--r--   0        0        0     2018 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_standby.textfsm
--rw-r--r--   0        0        0      621 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_standby_brief.textfsm
--rw-r--r--   0        0        0      495 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_switch_detail.textfsm
--rw-r--r--   0        0        0      357 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_switch_detail_stack_ports.textfsm
--rw-r--r--   0        0        0     1009 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_tacacs.textfsm
--rw-r--r--   0        0        0     1735 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_version.textfsm
--rw-r--r--   0        0        0     6327 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vlan.textfsm
--rw-r--r--   0        0        0      534 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vrf.textfsm
--rw-r--r--   0        0        0     1047 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vrf_detail.textfsm
--rw-r--r--   0        0        0     1596 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vrrp_all.textfsm
--rw-r--r--   0        0        0     1655 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vrrp_brief.textfsm
--rw-r--r--   0        0        0     1109 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vtp_status.textfsm
--rw-r--r--   0        0        0     1660 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_traceroute.textfsm
--rw-r--r--   0        0        0     1781 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_access-lists.textfsm
--rw-r--r--   0        0        0      461 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_cdp_neighbors.textfsm
--rw-r--r--   0        0        0      689 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_cdp_neighbors_detail.textfsm
--rw-r--r--   0        0        0      203 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_clock.textfsm
--rw-r--r--   0        0        0      210 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_configuration_session_summary.textfsm
--rw-r--r--   0        0        0      954 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_cts_interface_all.textfsm
--rw-r--r--   0        0        0      233 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_cts_interface_brief.textfsm
--rw-r--r--   0        0        0     2143 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_environment.textfsm
--rw-r--r--   0        0        0      384 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_environment_temperature.textfsm
--rw-r--r--   0        0        0      147 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_feature.textfsm
--rw-r--r--   0        0        0      178 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_fex.textfsm
--rw-r--r--   0        0        0     1002 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_fex_id.textfsm
--rw-r--r--   0        0        0      491 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_flogi_database.textfsm
--rw-r--r--   0        0        0     1083 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_forwarding_adjacency.textfsm
--rw-r--r--   0        0        0      979 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_forwarding_ipv4_route.textfsm
--rw-r--r--   0        0        0       57 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_hostname.textfsm
--rw-r--r--   0        0        0     2323 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_hsrp_all.textfsm
--rw-r--r--   0        0        0     1491 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interface.textfsm
--rw-r--r--   0        0        0     1717 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interface_brief.textfsm
--rw-r--r--   0        0        0      358 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interface_description.textfsm
--rw-r--r--   0        0        0      364 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interface_status.textfsm
--rw-r--r--   0        0        0      518 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver.textfsm
--rw-r--r--   0        0        0     2240 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver_details.textfsm
--rw-r--r--   0        0        0      800 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interfaces_switchport.textfsm
--rw-r--r--   0        0        0      500 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_inventory.textfsm
--rw-r--r--   0        0        0      698 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_adjacency.textfsm
--rw-r--r--   0        0        0      300 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_arp.textfsm
--rw-r--r--   0        0        0      426 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_arp_detail.textfsm
--rw-r--r--   0        0        0     2011 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_bgp.textfsm
--rw-r--r--   0        0        0     4318 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_neighbors.textfsm
--rw-r--r--   0        0        0      974 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary.textfsm
--rw-r--r--   0        0        0     1014 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary_vrf.textfsm
--rw-r--r--   0        0        0      714 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_community-list.textfsm
--rw-r--r--   0        0        0      283 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_dhcp_relay_address.textfsm
--rw-r--r--   0        0        0     3956 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_dhcp_snooping_statistics.textfsm
--rw-r--r--   0        0        0     5936 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_interface.textfsm
--rw-r--r--   0        0        0      356 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_interface_brief.textfsm
--rw-r--r--   0        0        0     2403 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_interface_vrf_all.textfsm
--rw-r--r--   0        0        0      665 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_msdp_summary_vrf_all.textfsm
--rw-r--r--   0        0        0      680 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_database.textfsm
--rw-r--r--   0        0        0      526 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_interface_brief.textfsm
--rw-r--r--   0        0        0      387 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_neighbor.textfsm
--rw-r--r--   0        0        0      453 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_pim_group-range_vrf_all.textfsm
--rw-r--r--   0        0        0      480 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_pim_interface_brief_vrf_all.textfsm
--rw-r--r--   0        0        0      599 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_pim_neighbor_vrf_all.textfsm
--rw-r--r--   0        0        0      546 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_pim_rp_vrf_all.textfsm
--rw-r--r--   0        0        0     2072 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_route.textfsm
--rw-r--r--   0        0        0      222 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ipv6_interface_brief.textfsm
--rw-r--r--   0        0        0      244 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_l2rib_internal_permanently-frozen-list.textfsm
--rw-r--r--   0        0        0      411 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_license_usage.textfsm
--rw-r--r--   0        0        0      297 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_lldp_neighbors.textfsm
--rw-r--r--   0        0        0      727 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_lldp_neighbors_detail.textfsm
--rw-r--r--   0        0        0      290 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_mac_address-table.textfsm
--rw-r--r--   0        0        0      351 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_module.textfsm
--rw-r--r--   0        0        0      288 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_nve_peers.textfsm
--rw-r--r--   0        0        0      495 2023-06-11 21:19:30.888631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_nve_vni.textfsm
--rw-r--r--   0        0        0     2346 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_port-channel_summary.textfsm
--rw-r--r--   0        0        0      234 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_processes_cpu.textfsm
--rw-r--r--   0        0        0      698 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_route-map.textfsm
--rw-r--r--   0        0        0      489 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_spanning-tree_root.textfsm
--rw-r--r--   0        0        0      296 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_vdc.textfsm
--rwxr-xr-x   0        0        0      697 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_version.textfsm
--rw-r--r--   0        0        0     6310 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_vlan.textfsm
--rw-r--r--   0        0        0       99 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_vpc.textfsm
--rw-r--r--   0        0        0      279 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_vrf.textfsm
--rw-r--r--   0        0        0      239 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_vrf_interface.textfsm
--rw-r--r--   0        0        0      594 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_s300_show_interfaces_status.textfsm
--rw-r--r--   0        0        0      411 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_s300_show_lldp_neighbors.textfsm
--rw-r--r--   0        0        0      330 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_s300_show_mac_address-table.textfsm
--rw-r--r--   0        0        0      442 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_s300_show_version.textfsm
--rw-r--r--   0        0        0     3155 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a.textfsm
--rw-r--r--   0        0        0     4795 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a_cleanair_config.textfsm
--rw-r--r--   0        0        0     1683 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_advanced_802.11a_channel.textfsm
--rw-r--r--   0        0        0     2697 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_config_general.textfsm
--rw-r--r--   0        0        0      643 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_image_all.textfsm
--rw-r--r--   0        0        0      492 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_summary.textfsm
--rw-r--r--   0        0        0      780 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_band-select.textfsm
--rw-r--r--   0        0        0      661 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_cdp_neighbors_detail.textfsm
--rw-r--r--   0        0        0     1429 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_client_detail.textfsm
--rw-r--r--   0        0        0      276 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_exclusionlist.textfsm
--rw-r--r--   0        0        0      355 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_flexconnect_group_summary.textfsm
--rw-r--r--   0        0        0     1437 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_detailed_id.textfsm
--rw-r--r--   0        0        0      347 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_group_summary.textfsm
--rw-r--r--   0        0        0      480 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_summary.textfsm
--rw-r--r--   0        0        0      436 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_inventory.textfsm
--rw-r--r--   0        0        0      463 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_mobility_anchor.textfsm
--rw-r--r--   0        0        0      737 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_mobility_sum.textfsm
--rw-r--r--   0        0        0      655 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_port_summary.textfsm
--rw-r--r--   0        0        0     2799 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_radius_summary.textfsm
--rw-r--r--   0        0        0      842 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_detail.textfsm
--rw-r--r--   0        0        0      970 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_summary.textfsm
--rw-r--r--   0        0        0      417 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_rf-profile_summary.textfsm
--rw-r--r--   0        0        0      997 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_stats_port_summary.textfsm
--rw-r--r--   0        0        0     1238 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_sysinfo.textfsm
--rw-r--r--   0        0        0     1450 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_tacacs_summary.textfsm
--rw-r--r--   0        0        0      906 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_time.textfsm
--rw-r--r--   0        0        0      420 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_wlan_sum.textfsm
--rw-r--r--   0        0        0     6223 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_admin_show_controller_fabric_health.textfsm
--rw-r--r--   0        0        0     1379 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_admin_show_environment_fan.textfsm
--rw-r--r--   0        0        0      309 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_admin_show_environment_power.textfsm
--rw-r--r--   0        0        0      398 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_admin_show_inventory.textfsm
--rw-r--r--   0        0        0      179 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_admin_show_platform.textfsm
--rw-r--r--   0        0        0      419 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_admin_show_vm.textfsm
--rw-r--r--   0        0        0      515 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_arp.textfsm
--rw-r--r--   0        0        0      838 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_asic-errors_all_location.textfsm
--rw-r--r--   0        0        0      179 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_bfd_sessions.textfsm
--rw-r--r--   0        0        0     1905 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_bgp.textfsm
--rw-r--r--   0        0        0      725 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_bgp_instance_all_summary.textfsm
--rw-r--r--   0        0        0     5397 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_bgp_neighbors.textfsm
--rw-r--r--   0        0        0      156 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_bgp_vrf_all_ipv4_unicast_summary.textfsm
--rw-r--r--   0        0        0      513 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_cdp_neighbors_detail.textfsm
--rw-r--r--   0        0        0     1544 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_cef_drops_location.textfsm
--rw-r--r--   0        0        0      337 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_configuration_commit_list.textfsm
--rw-r--r--   0        0        0      347 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controller_fabric_plane_all.textfsm
--rw-r--r--   0        0        0     2208 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_HundredGigabitEthernet.textfsm
--rw-r--r--   0        0        0     2281 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_all_phy.textfsm
--rw-r--r--   0        0        0     2823 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_egress_location.textfsm
--rw-r--r--   0        0        0     1961 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_ingress_location.textfsm
--rw-r--r--   0        0        0      426 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_errors_egress_location.textfsm
--rw-r--r--   0        0        0     1406 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_errors_ingress_location.textfsm
--rw-r--r--   0        0        0     4953 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_hundredgige_all.textfsm
--rw-r--r--   0        0        0      266 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_dhcp_ipv4_proxy_binding.textfsm
--rw-r--r--   0        0        0     7430 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_drops_np_all.textfsm
--rw-r--r--   0        0        0      518 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_hsrp.textfsm
--rw-r--r--   0        0        0      665 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_install_active.textfsm
--rw-r--r--   0        0        0      268 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_interface_brief.textfsm
--rw-r--r--   0        0        0      835 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_interfaces.textfsm
--rw-r--r--   0        0        0      353 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_interfaces_summary.textfsm
--rw-r--r--   0        0        0      571 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ip_bgp_summary.textfsm
--rw-r--r--   0        0        0      178 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ip_interface_brief.textfsm
--rw-r--r--   0        0        0     1094 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ip_route.textfsm
--rw-r--r--   0        0        0      769 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ipv4_interface.textfsm
--rw-r--r--   0        0        0      270 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ipv4_vrf_all_interface_brief.textfsm
--rw-r--r--   0        0        0      405 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ipv6_neighbors.textfsm
--rw-r--r--   0        0        0      288 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_isis_neighbors.textfsm
--rw-r--r--   0        0        0      380 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_lldp_neighbors.textfsm
--rw-r--r--   0        0        0      694 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_lpts_pifib_hardware_police_location.textfsm
--rw-r--r--   0        0        0      398 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_mpls_ldp_neighbor_brief.textfsm
--rw-r--r--   0        0        0      356 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ospf_neighbor.textfsm
--rw-r--r--   0        0        0      440 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ospf_vrf_all_interface_brief.textfsm
--rw-r--r--   0        0        0      474 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ospf_vrf_all_neighbor.textfsm
--rw-r--r--   0        0        0      359 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_pim_ipv4_group-map.textfsm
--rw-r--r--   0        0        0      481 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_pim_ipv4_interface.textfsm
--rw-r--r--   0        0        0      447 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_pim_ipv4_neighbor.textfsm
--rw-r--r--   0        0        0      262 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_pim_neighbor.textfsm
--rw-r--r--   0        0        0     1074 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_platform_summary_location_all.textfsm
--rw-r--r--   0        0        0      205 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_processes_cpu.textfsm
--rw-r--r--   0        0        0      187 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_redundancy_summary.textfsm
--rw-r--r--   0        0        0      226 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_rsvp_neighbors.textfsm
--rw-r--r--   0        0        0      856 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_version.textfsm
--rw-r--r--   0        0        0      339 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_version_brief.textfsm
--rw-r--r--   0        0        0      422 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_vrf_all_detail.textfsm
--rw-r--r--   0        0        0      290 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/dell_force10_show_arp.textfsm
--rw-r--r--   0        0        0      213 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/dell_force10_show_ip_interface_brief.textfsm
--rw-r--r--   0        0        0      211 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/dell_force10_show_version.textfsm
--rw-r--r--   0        0        0      815 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/dell_force10_show_vlan.textfsm
--rw-r--r--   0        0        0      248 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/dell_force10_show_vlan_brief.textfsm
--rw-r--r--   0        0        0      289 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/dell_powerconnect_show_bridge_address_table.textfsm
--rw-r--r--   0        0        0      193 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/dell_powerconnect_show_interfaces_description.textfsm
--rw-r--r--   0        0        0      592 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/dell_powerconnect_show_interfaces_status.textfsm
--rw-r--r--   0        0        0      301 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/dlink_ds_show_arpentry.textfsm
--rw-r--r--   0        0        0      647 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/ericsson_ipos_show_arp.textfsm
--rw-r--r--   0        0        0      433 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/ericsson_ipos_show_isis_adjacency.textfsm
--rw-r--r--   0        0        0      168 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/ericsson_ipos_show_version.textfsm
--rw-r--r--   0        0        0      574 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_router_info_bgp_summary.textfsm
--rw-r--r--   0        0        0      230 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_system_arp.textfsm
--rw-r--r--   0        0        0     2048 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_system_ha_status.textfsm
--rw-r--r--   0        0        0     8998 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_system_interface.textfsm
--rw-r--r--   0        0        0      657 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_system_interface_physical.textfsm
--rw-r--r--   0        0        0     2528 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_system_status.textfsm
--rw-r--r--   0        0        0      238 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_arp.textfsm
--rw-r--r--   0        0        0      200 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_clock.textfsm
--rw-r--r--   0        0        0      519 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_counters_bound_interface.textfsm
--rw-r--r--   0        0        0      666 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_device_manuinfo.textfsm
--rw-r--r--   0        0        0     8519 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_interface.textfsm
--rw-r--r--   0        0        0     1573 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_ip_interface.textfsm
--rw-r--r--   0        0        0      616 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_ip_routing-table.textfsm
--rw-r--r--   0        0        0      195 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_ip_vpn-instance.textfsm
--rw-r--r--   0        0        0     5480 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_ip_vpn-instance_instance-name.textfsm
--rw-r--r--   0        0        0      777 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_link-aggregation_verbose.textfsm
--rw-r--r--   0        0        0      647 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_list.textfsm
--rw-r--r--   0        0        0      926 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_verbose.textfsm
--rw-r--r--   0        0        0      187 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_mac-address.textfsm
--rw-r--r--   0        0        0      632 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_vlan_all.textfsm
--rw-r--r--   0        0        0      106 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_vlan_brief.textfsm
--rw-r--r--   0        0        0      179 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_arp.textfsm
--rw-r--r--   0        0        0      710 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_interfaces.textfsm
--rw-r--r--   0        0        0      917 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_interfaces_brief.textfsm
--rw-r--r--   0        0        0      706 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device.textfsm
--rw-r--r--   0        0        0     1699 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device_detail.textfsm
--rw-r--r--   0        0        0      222 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_mac-address.textfsm
--rw-r--r--   0        0        0      453 2023-06-11 21:19:30.892631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_port-security.textfsm
--rw-r--r--   0        0        0     1329 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_system.textfsm
--rw-r--r--   0        0        0      385 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_tech_buffers.textfsm
--rw-r--r--   0        0        0      407 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_trunks.textfsm
--rw-r--r--   0        0        0      290 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_vlans.textfsm
--rw-r--r--   0        0        0     1392 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_acl_all.textfsm
--rw-r--r--   0        0        0      551 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_arp_all.textfsm
--rw-r--r--   0        0        0      491 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_arp_brief.textfsm
--rw-r--r--   0        0        0     3608 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_interface.textfsm
--rw-r--r--   0        0        0      498 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_interface_brief.textfsm
--rw-r--r--   0        0        0      376 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_interface_description.textfsm
--rw-r--r--   0        0        0     2059 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_ip_routing-table_verbose.textfsm
--rw-r--r--   0        0        0      843 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_ipv6_neighbors.textfsm
--rw-r--r--   0        0        0      435 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_isis_peer.textfsm
--rw-r--r--   0        0        0     1811 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_lldp_neighbor.textfsm
--rw-r--r--   0        0        0      713 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_nat_server.textfsm
--rw-r--r--   0        0        0     7310 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_port_vlan.textfsm
--rw-r--r--   0        0        0      193 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_service-set_all.textfsm
--rw-r--r--   0        0        0     1084 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_service-set_id_id.textfsm
--rw-r--r--   0        0        0       96 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_sn_license.textfsm
--rw-r--r--   0        0        0      424 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_snmp-agent_community_read.textfsm
--rw-r--r--   0        0        0     1346 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_startup.textfsm
--rw-r--r--   0        0        0      390 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_temperature.textfsm
--rw-r--r--   0        0        0      522 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_traffic-filter_applied-record.textfsm
--rw-r--r--   0        0        0      505 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_version.textfsm
--rw-r--r--   0        0        0    52562 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/index
--rw-r--r--   0        0        0      536 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ipinfusion_ocnos_show_lldp_table.textfsm
--rw-r--r--   0        0        0      303 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_arp_no-resolve.textfsm
--rw-r--r--   0        0        0     3195 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_interfaces.textfsm
--rw-r--r--   0        0        0      803 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_status.textfsm
--rw-r--r--   0        0        0      341 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_chassis_firmware.textfsm
--rw-r--r--   0        0        0      855 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_chassis_hardware.textfsm
--rw-r--r--   0        0        0      729 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_ethernet-switching_table.textfsm
--rw-r--r--   0        0        0      553 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_interfaces.textfsm
--rw-r--r--   0        0        0      267 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_isis_adjacency.textfsm
--rw-r--r--   0        0        0      630 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_lacp_interfaces.textfsm
--rw-r--r--   0        0        0      389 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_lldp_neighbors.textfsm
--rw-r--r--   0        0        0      292 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_ospf_neighbor.textfsm
--rw-r--r--   0        0        0     1374 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_system_uptime.textfsm
--rw-r--r--   0        0        0     4359 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_version.textfsm
--rw-r--r--   0        0        0      318 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_vlans.textfsm
--rw-r--r--   0        0        0      768 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/juniper_screenos_get_route.textfsm
--rw-r--r--   0        0        0      338 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/linux_arp_-a.textfsm
--rw-r--r--   0        0        0      915 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/linux_ip_address_show.textfsm
--rw-r--r--   0        0        0     1092 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/linux_ip_link_show.textfsm
--rw-r--r--   0        0        0      618 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/linux_ip_route_show.textfsm
--rw-r--r--   0        0        0      134 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/linux_ip_vrf_show.textfsm
--rw-r--r--   0        0        0      660 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_interface_ethernet_monitor_name_once.textfsm
--rw-r--r--   0        0        0      364 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ip_arp_print_without-paging.textfsm
--rw-r--r--   0        0        0      899 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ip_dhcp-server_lease_print_without-paging.textfsm
--rw-r--r--   0        0        0      331 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_address-list_print_terse.textfsm
--rw-r--r--   0        0        0     2499 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_filter_print_all_without-paging.textfsm
--rw-r--r--   0        0        0     2229 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_nat_print_all_without-paging.textfsm
--rw-r--r--   0        0        0      546 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ip_route_print_terse.textfsm
--rw-r--r--   0        0        0      400 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ipv6_neighbor_print_without-paging.textfsm
--rw-r--r--   0        0        0      483 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_snmp_community_print_without-paging.textfsm
--rw-r--r--   0        0        0      673 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_system_routerboard_print.textfsm
--rw-r--r--   0        0        0      169 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_debug_swm_status.textfsm
--rw-r--r--   0        0        0      337 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_arp_all.textfsm
--rw-r--r--   0        0        0      249 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_counter_global.textfsm
--rw-r--r--   0        0        0     1943 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_high-availability_all.textfsm
--rw-r--r--   0        0        0      293 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_interface_hardware.textfsm
--rw-r--r--   0        0        0      256 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_interface_logical.textfsm
--rw-r--r--   0        0        0      962 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_interface_management.textfsm
--rw-r--r--   0        0        0      415 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_jobs_all.textfsm
--rw-r--r--   0        0        0      236 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_mac_all.textfsm
--rw-r--r--   0        0        0      729 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_running_nat-policy.textfsm
--rw-r--r--   0        0        0      794 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_running_security-policy.textfsm
--rw-r--r--   0        0        0      840 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_system_info.textfsm
--rw-r--r--   0        0        0      975 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_test_security-policy-match.textfsm
--rw-r--r--   0        0        0      908 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_arp.textfsm
--rw-r--r--   0        0        0      693 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_interfaces.textfsm
--rw-r--r--   0        0        0      602 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_interfaces_brief.textfsm
--rw-r--r--   0        0        0      279 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_mac-address.textfsm
--rw-r--r--   0        0        0      263 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_media_validation.textfsm
--rw-r--r--   0        0        0     1049 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_version.textfsm
--rw-r--r--   0        0        0     2669 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_vlan.textfsm
--rw-r--r--   0        0        0      401 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgerouter_show_arp.textfsm
--rw-r--r--   0        0        0      372 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgerouter_show_dhcp_leases.textfsm
--rw-r--r--   0        0        0      270 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgerouter_show_dhcpv6_server_leases.textfsm
--rw-r--r--   0        0        0      293 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgerouter_show_interfaces.textfsm
--rw-r--r--   0        0        0      307 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgerouter_show_interfaces_ethernet_physical.textfsm
--rw-r--r--   0        0        0      662 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgerouter_show_ip_route.textfsm
--rw-r--r--   0        0        0      233 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgerouter_show_ipv6_neighbors.textfsm
--rw-r--r--   0        0        0      471 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgerouter_show_ipv6_route.textfsm
--rw-r--r--   0        0        0      380 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgerouter_show_version.textfsm
--rw-r--r--   0        0        0      314 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgeswitch_show_arp.textfsm
--rw-r--r--   0        0        0      553 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgeswitch_show_version.textfsm
--rw-r--r--   0        0        0      209 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgeswitch_show_vlan.textfsm
--rw-r--r--   0        0        0      470 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/vmware_nsxv_show_ip_bgp_neighbors.textfsm
--rw-r--r--   0        0        0      259 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/vmware_nsxv_show_ip_route.textfsm
--rw-r--r--   0        0        0      281 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/vyatta_vyos_show_arp.textfsm
--rw-r--r--   0        0        0      374 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/vyatta_vyos_show_interfaces.textfsm
--rw-r--r--   0        0        0      859 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/vyatta_vyos_show_ip_bgp_summary.textfsm
--rw-r--r--   0        0        0      231 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/watchguard_firebox_show_arp.textfsm
--rw-r--r--   0        0        0     1181 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/yamaha_show_environment.textfsm
--rw-r--r--   0        0        0      472 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/yamaha_show_ip_route.textfsm
--rw-r--r--   0        0        0      626 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_firewall_acl_get.textfsm
--rw-r--r--   0        0        0      402 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_intf_group_get.textfsm
--rw-r--r--   0        0        0      563 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_ipalias_get.textfsm
--rw-r--r--   0        0        0      409 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_lan_get.textfsm
--rw-r--r--   0        0        0      662 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_lan_get_--Name_name.textfsm
--rw-r--r--   0        0        0      411 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_lanhosts_get.textfsm
--rw-r--r--   0        0        0      664 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_nat_addr_map_get.textfsm
--rw-r--r--   0        0        0      751 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_nat_get.textfsm
--rw-r--r--   0        0        0      629 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_snmp_get.textfsm
--rw-r--r--   0        0        0      339 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_static_dhcp_get.textfsm
--rw-r--r--   0        0        0      625 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_static_route_get.textfsm
--rw-r--r--   0        0        0      539 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_wlan_get.textfsm
--rw-r--r--   0        0        0      857 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_sys_atsh.textfsm
--rw-r--r--   0        0        0      337 2023-06-11 21:19:30.896631 ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_zycli_Ethctl_media-type.textfsm
--rw-r--r--   0        0        0     3098 2023-06-11 21:19:43.932714 ntc_templates-3.4.0/pyproject.toml
--rw-r--r--   0        0        0     3871 1970-01-01 00:00:00.000000 ntc_templates-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0      601 2023-06-27 15:17:15.888029 ntc_templates-3.5.0/LICENSE
+-rw-r--r--   0        0        0     2842 2023-06-27 15:17:15.888029 ntc_templates-3.5.0/README.md
+-rw-r--r--   0        0        0      260 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/__init__.py
+-rw-r--r--   0        0        0     2180 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/parse.py
+-rw-r--r--   0        0        0      700 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/alcatel_aos_show_vlan.textfsm
+-rw-r--r--   0        0        0      170 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_oam_mac-ping.textfsm
+-rw-r--r--   0        0        0      371 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_lag.textfsm
+-rw-r--r--   0        0        0      641 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_port.textfsm
+-rw-r--r--   0        0        0      434 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_router_bgp_routes_vpn-ipv4.textfsm
+-rw-r--r--   0        0        0      526 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_router_bgp_summary_family.textfsm
+-rw-r--r--   0        0        0      662 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_router_interface.textfsm
+-rw-r--r--   0        0        0      318 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_router_isis_adjacency.textfsm
+-rw-r--r--   0        0        0      336 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_router_isis_interface.textfsm
+-rw-r--r--   0        0        0      619 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_router_ldp_interface.textfsm
+-rw-r--r--   0        0        0      608 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_router_mpls_interface.textfsm
+-rw-r--r--   0        0        0      512 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_router_mpls_lsp.textfsm
+-rw-r--r--   0        0        0      547 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_router_ospf_interface.textfsm
+-rw-r--r--   0        0        0      425 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_router_pim_interface.textfsm
+-rw-r--r--   0        0        0      649 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_router_rsvp_interface.textfsm
+-rw-r--r--   0        0        0      544 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_service_id_base.textfsm
+-rw-r--r--   0        0        0      665 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_service_sap-using.textfsm
+-rw-r--r--   0        0        0      598 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_service_sdp-using.textfsm
+-rw-r--r--   0        0        0      642 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_service_sdp.textfsm
+-rw-r--r--   0        0        0      522 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_system_cpu.textfsm
+-rw-r--r--   0        0        0      371 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_bash_df_-h.textfsm
+-rw-r--r--   0        0        0      430 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_dir_flash.textfsm
+-rw-r--r--   0        0        0      121 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_boot-config.textfsm
+-rw-r--r--   0        0        0      226 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_clock.textfsm
+-rw-r--r--   0        0        0      524 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_environment_cooling.textfsm
+-rw-r--r--   0        0        0      525 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_environment_temperature.textfsm
+-rw-r--r--   0        0        0      107 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_hostname.textfsm
+-rw-r--r--   0        0        0      888 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_interfaces.textfsm
+-rw-r--r--   0        0        0      427 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_interfaces_description.textfsm
+-rw-r--r--   0        0        0      399 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_interfaces_status.textfsm
+-rw-r--r--   0        0        0      313 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_interfaces_transceiver.textfsm
+-rw-r--r--   0        0        0      757 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_interfaces_transceiver_detail.textfsm
+-rw-r--r--   0        0        0      666 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_inventory.textfsm
+-rw-r--r--   0        0        0      517 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_ip_access-lists.textfsm
+-rw-r--r--   0        0        0      159 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_ip_arp.textfsm
+-rw-r--r--   0        0        0      651 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_ip_bgp.textfsm
+-rw-r--r--   0        0        0     1577 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_ip_bgp_summary.textfsm
+-rw-r--r--   0        0        0      246 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_ip_helper-address.textfsm
+-rw-r--r--   0        0        0      169 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_ip_interface_brief.textfsm
+-rw-r--r--   0        0        0      736 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_ip_ospf_database.textfsm
+-rw-r--r--   0        0        0      387 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_ip_ospf_interface_brief.textfsm
+-rw-r--r--   0        0        0      462 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_ip_ospf_neighbor.textfsm
+-rw-r--r--   0        0        0      734 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_ip_ospf_summary.textfsm
+-rw-r--r--   0        0        0     1035 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_ip_route.textfsm
+-rw-r--r--   0        0        0     1101 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_ipv6_bgp_summary.textfsm
+-rw-r--r--   0        0        0      358 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_isis_neighbors.textfsm
+-rw-r--r--   0        0        0      190 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_lldp_neighbors.textfsm
+-rw-r--r--   0        0        0      627 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_lldp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0     1662 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_mac_address-table.textfsm
+-rw-r--r--   0        0        0      257 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_mac_security_interface.textfsm
+-rw-r--r--   0        0        0      303 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_mac_security_mka_counters.textfsm
+-rw-r--r--   0        0        0     1431 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_mac_security_participants_detail.textfsm
+-rw-r--r--   0        0        0      279 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_mlag.textfsm
+-rw-r--r--   0        0        0      716 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_module.textfsm
+-rw-r--r--   0        0        0      557 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_pim_ipv4_interface.textfsm
+-rw-r--r--   0        0        0      403 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_pim_ipv4_neighbor.textfsm
+-rw-r--r--   0        0        0     1222 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_port-channel_summary.textfsm
+-rw-r--r--   0        0        0     5405 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_processes_top_once.textfsm
+-rw-r--r--   0        0        0      573 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_reload_cause.textfsm
+-rw-r--r--   0        0        0      275 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_snmp_community.textfsm
+-rw-r--r--   0        0        0      424 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_version.textfsm
+-rw-r--r--   0        0        0     6187 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_vlan.textfsm
+-rw-r--r--   0        0        0     4153 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_vrf.textfsm
+-rw-r--r--   0        0        0      701 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/aruba_aoscx_show_aaa_authentication_port-access_interface_all_client-status.textfsm
+-rw-r--r--   0        0        0      322 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/aruba_aoscx_show_arp_all-vrfs.textfsm
+-rw-r--r--   0        0        0      596 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/aruba_aoscx_show_bfd_all-vrfs.textfsm
+-rw-r--r--   0        0        0      531 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/aruba_aoscx_show_bgp_all-vrfs_all_summary.textfsm
+-rw-r--r--   0        0        0      531 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/aruba_aoscx_show_bgp_all_all-vrfs_summary.textfsm
+-rw-r--r--   0        0        0     2201 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/aruba_aoscx_show_interface.textfsm
+-rw-r--r--   0        0        0     4761 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/aruba_aoscx_show_interface_dom_detail.textfsm
+-rw-r--r--   0        0        0      348 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/aruba_aoscx_show_ip_route_all-vrfs.textfsm
+-rw-r--r--   0        0        0      827 2023-06-27 15:17:15.892029 ntc_templates-3.5.0/ntc_templates/templates/aruba_aoscx_show_lldp_neighbors-info_detail.textfsm
+-rw-r--r--   0        0        0      240 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/aruba_aoscx_show_mac-address-table.textfsm
+-rw-r--r--   0        0        0      380 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/aruba_aoscx_show_ntp_associations.textfsm
+-rw-r--r--   0        0        0      956 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/aruba_aoscx_show_system.textfsm
+-rw-r--r--   0        0        0      662 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/aruba_aoscx_show_vsf_detail.textfsm
+-rw-r--r--   0        0        0      917 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/aruba_os_show_ap_bss-table_details.textfsm
+-rw-r--r--   0        0        0      768 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/aruba_os_show_ap_database.textfsm
+-rw-r--r--   0        0        0     1028 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/aruba_os_show_ap_database_long.textfsm
+-rw-r--r--   0        0        0      977 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/aruba_os_show_ap_radio-database.textfsm
+-rw-r--r--   0        0        0      735 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/aruba_os_show_arp.textfsm
+-rw-r--r--   0        0        0      176 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/aruba_os_show_ip_interface_brief.textfsm
+-rw-r--r--   0        0        0      287 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/aruba_os_show_ipv6_interface_brief.textfsm
+-rw-r--r--   0        0        0      119 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/avaya_ers_show_interface_name.textfsm
+-rw-r--r--   0        0        0      702 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/avaya_ers_show_logging_config.textfsm
+-rw-r--r--   0        0        0      181 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/avaya_ers_show_mac-address-table.textfsm
+-rw-r--r--   0        0        0      878 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/avaya_ers_show_mlt.textfsm
+-rw-r--r--   0        0        0      607 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/avaya_ers_show_mlt_all-members.textfsm
+-rw-r--r--   0        0        0     1825 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/avaya_ers_show_sys-info.textfsm
+-rw-r--r--   0        0        0      470 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/avaya_ers_show_vlan.textfsm
+-rw-r--r--   0        0        0      367 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/avaya_vsp_show_software.textfsm
+-rw-r--r--   0        0        0      583 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/broadcom_icos_show_isdp_neighbors.textfsm
+-rw-r--r--   0        0        0      631 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/broadcom_icos_show_lldp_remote-device_all.textfsm
+-rw-r--r--   0        0        0      458 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/broadcom_icos_show_mac-addr-table.textfsm
+-rw-r--r--   0        0        0     1497 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/broadcom_icos_show_version.textfsm
+-rw-r--r--   0        0        0      372 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/broadcom_icos_show_vlan_brief.textfsm
+-rw-r--r--   0        0        0      358 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_arp.textfsm
+-rw-r--r--   0        0        0     5683 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_interfaces.textfsm
+-rw-r--r--   0        0        0      695 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_interfaces_brief.textfsm
+-rw-r--r--   0        0        0      367 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_lag_brief.textfsm
+-rw-r--r--   0        0        0      416 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_lldp_neighbors.textfsm
+-rw-r--r--   0        0        0      906 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_lldp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0      375 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_mac-address.textfsm
+-rw-r--r--   0        0        0     1120 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_metro.textfsm
+-rw-r--r--   0        0        0      301 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_monitor.textfsm
+-rw-r--r--   0        0        0     2278 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_running-config_vlan.textfsm
+-rw-r--r--   0        0        0      851 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_span.textfsm
+-rw-r--r--   0        0        0      351 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_topo.textfsm
+-rw-r--r--   0        0        0     2990 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_trunk.textfsm
+-rw-r--r--   0        0        0     1629 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_version.textfsm
+-rw-r--r--   0        0        0     6614 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_netiron_show_interfaces.textfsm
+-rw-r--r--   0        0        0      430 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_netiron_show_interfaces_brief.textfsm
+-rw-r--r--   0        0        0      367 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_netiron_show_lag_brief.textfsm
+-rw-r--r--   0        0        0      906 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_netiron_show_lldp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0     1071 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_netiron_show_metro.textfsm
+-rw-r--r--   0        0        0      311 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_netiron_show_monitor_actual.textfsm
+-rw-r--r--   0        0        0     1618 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_netiron_show_running-config_interface.textfsm
+-rw-r--r--   0        0        0     2277 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_netiron_show_running-config_vlan.textfsm
+-rw-r--r--   0        0        0      739 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_netiron_show_span.textfsm
+-rw-r--r--   0        0        0      591 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/brocade_netiron_show_topo.textfsm
+-rw-r--r--   0        0        0      167 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/checkpoint_gaia_fw_stat.textfsm
+-rw-r--r--   0        0        0      170 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/checkpoint_gaia_show_arp_dynamic_all.textfsm
+-rw-r--r--   0        0        0      148 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/checkpoint_gaia_show_asset_all.textfsm
+-rw-r--r--   0        0        0      189 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/checkpoint_gaia_show_dns.textfsm
+-rw-r--r--   0        0        0       71 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/checkpoint_gaia_show_domainname.textfsm
+-rw-r--r--   0        0        0      786 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/checkpoint_gaia_show_interfaces_all.textfsm
+-rw-r--r--   0        0        0      482 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/checkpoint_gaia_show_ipv6_route.textfsm
+-rw-r--r--   0        0        0      159 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/checkpoint_gaia_show_lom.textfsm
+-rw-r--r--   0        0        0      208 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/checkpoint_gaia_show_ntp_servers.textfsm
+-rw-r--r--   0        0        0      550 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/checkpoint_gaia_show_route.textfsm
+-rw-r--r--   0        0        0      236 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/checkpoint_gaia_show_version_all.textfsm
+-rw-r--r--   0        0        0      419 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/ciena_saos_chassis_show_temperature.textfsm
+-rw-r--r--   0        0        0     1010 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/ciena_saos_port_show.textfsm
+-rw-r--r--   0        0        0      945 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/ciena_saos_rstp_show.textfsm
+-rw-r--r--   0        0        0      623 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/ciena_saos_software_show.textfsm
+-rw-r--r--   0        0        0      289 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/ciena_saos_ssh_server_show_key.textfsm
+-rw-r--r--   0        0        0      556 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/ciena_saos_traffic-profiling_standard-profile_show.textfsm
+-rw-r--r--   0        0        0      636 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/ciena_saos_vlan_show.textfsm
+-rw-r--r--   0        0        0      714 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_apic_fabric_show_vlan_extended.textfsm
+-rw-r--r--   0        0        0      663 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_dir.textfsm
+-rw-r--r--   0        0        0      661 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_ping.textfsm
+-rw-r--r--   0        0        0     6125 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_access-list.textfsm
+-rw-r--r--   0        0        0      325 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_arp.textfsm
+-rw-r--r--   0        0        0     9761 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_asp_drop.textfsm
+-rw-r--r--   0        0        0      829 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_asp_table_vpn-context_detail.textfsm
+-rw-r--r--   0        0        0     1377 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_bgp_summary.textfsm
+-rw-r--r--   0        0        0      917 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_cpu_usage_detailed.textfsm
+-rw-r--r--   0        0        0      438 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_crypto_ikev1_sa_detail.textfsm
+-rw-r--r--   0        0        0     6136 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_crypto_ipsec_sa.textfsm
+-rw-r--r--   0        0        0     3036 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_failover.textfsm
+-rw-r--r--   0        0        0     4402 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_interface.textfsm
+-rw-r--r--   0        0        0     7080 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_interface_detail.textfsm
+-rw-r--r--   0        0        0      268 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_interface_ip_brief.textfsm
+-rw-r--r--   0        0        0      320 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_inventory.textfsm
+-rw-r--r--   0        0        0     6025 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_license_all.textfsm
+-rw-r--r--   0        0        0     2352 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_logging.textfsm
+-rw-r--r--   0        0        0       89 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_name.textfsm
+-rw-r--r--   0        0        0     1624 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_nat.textfsm
+-rw-r--r--   0        0        0      561 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_object-group_network.textfsm
+-rw-r--r--   0        0        0      403 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_ospf_interface_brief.textfsm
+-rw-r--r--   0        0        0      374 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_ospf_neighbor.textfsm
+-rw-r--r--   0        0        0     1208 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_port-channel_summary.textfsm
+-rw-r--r--   0        0        0      425 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_resource_usage.textfsm
+-rw-r--r--   0        0        0     1606 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_route.textfsm
+-rw-r--r--   0        0        0     2300 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_running-config_all_crypto_map.textfsm
+-rw-r--r--   0        0        0      437 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_running-config_crypto_ikev1.textfsm
+-rw-r--r--   0        0        0     1212 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_running-config_crypto_map.textfsm
+-rw-r--r--   0        0        0     1726 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_running-config_ipsec.textfsm
+-rw-r--r--   0        0        0      474 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_running-config_object_network.textfsm
+-rw-r--r--   0        0        0     4906 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_running-config_tunnel-group.textfsm
+-rw-r--r--   0        0        0      967 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_version.textfsm
+-rw-r--r--   0        0        0     1625 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb.textfsm
+-rw-r--r--   0        0        0     1822 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_anyconnect.textfsm
+-rw-r--r--   0        0        0     7479 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_detail_l2l.textfsm
+-rw-r--r--   0        0        0     1126 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_xlate.textfsm
+-rw-r--r--   0        0        0      481 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_dir.textfsm
+-rw-r--r--   0        0        0      859 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_ping.textfsm
+-rw-r--r--   0        0        0     1584 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_access-list.textfsm
+-rw-r--r--   0        0        0      416 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_access-session.textfsm
+-rw-r--r--   0        0        0      953 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_adjacency.textfsm
+-rw-r--r--   0        0        0      355 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_alert_counters.textfsm
+-rw-r--r--   0        0        0      310 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_aliases.textfsm
+-rw-r--r--   0        0        0      523 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ap_summary.textfsm
+-rw-r--r--   0        0        0      615 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_archive.textfsm
+-rw-r--r--   0        0        0      403 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_authentication_sessions.textfsm
+-rw-r--r--   0        0        0     2496 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_bfd_neighbors_details.textfsm
+-rw-r--r--   0        0        0     1700 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_boot.textfsm
+-rw-r--r--   0        0        0      264 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_capability_feature_routing.textfsm
+-rw-r--r--   0        0        0      538 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors.textfsm
+-rw-r--r--   0        0        0      937 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0      317 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_clock.textfsm
+-rw-r--r--   0        0        0     2327 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_controller_t1.textfsm
+-rw-r--r--   0        0        0     6120 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_crypto_ipsec_sa_detail.textfsm
+-rw-r--r--   0        0        0     2174 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_crypto_pki_certificates.textfsm
+-rw-r--r--   0        0        0     1418 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_crypto_session_detail.textfsm
+-rw-r--r--   0        0        0     1041 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_dhcp_lease.textfsm
+-rw-r--r--   0        0        0      491 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_dmvpn.textfsm
+-rw-r--r--   0        0        0     1367 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_dot1x_all.textfsm
+-rw-r--r--   0        0        0      413 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_environment_power_all.textfsm
+-rw-r--r--   0        0        0     1603 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_environment_temperature.textfsm
+-rw-r--r--   0        0        0     1188 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_etherchannel_summary.textfsm
+-rw-r--r--   0        0        0      454 2023-06-27 15:17:15.896029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_hosts_summary.textfsm
+-rw-r--r--   0        0        0     1226 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_interface_link.textfsm
+-rw-r--r--   0        0        0      312 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_interface_transceiver.textfsm
+-rw-r--r--   0        0        0     2729 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_interfaces.textfsm
+-rw-r--r--   0        0        0      409 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_interfaces_description.textfsm
+-rw-r--r--   0        0        0      898 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_interfaces_status.textfsm
+-rw-r--r--   0        0        0     1512 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_interfaces_switchport.textfsm
+-rw-r--r--   0        0        0      570 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_inventory.textfsm
+-rw-r--r--   0        0        0     2587 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_access-lists.textfsm
+-rw-r--r--   0        0        0      525 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_arp.textfsm
+-rw-r--r--   0        0        0     2029 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_bgp.textfsm
+-rw-r--r--   0        0        0     1706 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors.textfsm
+-rw-r--r--   0        0        0     2011 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors_advertised-routes.textfsm
+-rw-r--r--   0        0        0      589 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_bgp_summary.textfsm
+-rw-r--r--   0        0        0     1761 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_bgp_vpnv4_all_neighbors.textfsm
+-rw-r--r--   0        0        0     1207 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_cef.textfsm
+-rw-r--r--   0        0        0     3244 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_cef_detail.textfsm
+-rw-r--r--   0        0        0      711 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_device_tracking_all.textfsm
+-rw-r--r--   0        0        0     2669 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_interfaces_detail.textfsm
+-rw-r--r--   0        0        0      773 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_neighbors.textfsm
+-rw-r--r--   0        0        0     2597 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_topology.textfsm
+-rwxr-xr-x   0        0        0      459 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_flow_toptalkers.textfsm
+-rw-r--r--   0        0        0     4260 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_http_server_status.textfsm
+-rw-r--r--   0        0        0     1909 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_interface.textfsm
+-rw-r--r--   0        0        0      288 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_interface_brief.textfsm
+-rw-r--r--   0        0        0     1378 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_mroute.textfsm
+-rw-r--r--   0        0        0      645 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_nat_translations.textfsm
+-rw-r--r--   0        0        0      778 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database.textfsm
+-rw-r--r--   0        0        0     1362 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_network.textfsm
+-rw-r--r--   0        0        0     1807 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_router.textfsm
+-rw-r--r--   0        0        0      396 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_ospf_interface_brief.textfsm
+-rw-r--r--   0        0        0      383 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_ospf_neighbor.textfsm
+-rw-r--r--   0        0        0      436 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_prefix-list.textfsm
+-rw-r--r--   0        0        0     2499 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_route.textfsm
+-rw-r--r--   0        0        0     1389 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_route_summary.textfsm
+-rw-r--r--   0        0        0      555 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_source_binding.textfsm
+-rw-r--r--   0        0        0      472 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_vrf_interfaces.textfsm
+-rw-r--r--   0        0        0      917 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ipv6_access-lists.textfsm
+-rw-r--r--   0        0        0      399 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ipv6_interface_brief.textfsm
+-rw-r--r--   0        0        0      371 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ipv6_neighbors.textfsm
+-rw-r--r--   0        0        0      523 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ipv6_route.textfsm
+-rw-r--r--   0        0        0      956 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_isdn_status.textfsm
+-rw-r--r--   0        0        0      412 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_isis_neighbors.textfsm
+-rw-r--r--   0        0        0      547 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_license.textfsm
+-rw-r--r--   0        0        0      479 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_lldp_neighbors.textfsm
+-rw-r--r--   0        0        0     2655 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_lldp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0     5593 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_logging.textfsm
+-rw-r--r--   0        0        0     4086 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_mac-address-table.textfsm
+-rw-r--r--   0        0        0     1017 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_module.textfsm
+-rw-r--r--   0        0        0      585 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_module_online_diag.textfsm
+-rw-r--r--   0        0        0     1062 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_module_status.textfsm
+-rw-r--r--   0        0        0      760 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_module_submodule.textfsm
+-rw-r--r--   0        0        0      350 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_mpls_interfaces.textfsm
+-rw-r--r--   0        0        0      377 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_nve_peers.textfsm
+-rw-r--r--   0        0        0      346 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_nve_vni.textfsm
+-rw-r--r--   0        0        0     1215 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_object-group.textfsm
+-rw-r--r--   0        0        0     1072 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_platform_diag.textfsm
+-rw-r--r--   0        0        0      974 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_port-security_interface_interface.textfsm
+-rw-r--r--   0        0        0      922 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_power_available.textfsm
+-rw-r--r--   0        0        0      684 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_power_status.textfsm
+-rw-r--r--   0        0        0      314 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_power_supplies.textfsm
+-rw-r--r--   0        0        0      344 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_processes_cpu.textfsm
+-rw-r--r--   0        0        0      640 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_processes_memory_sorted.textfsm
+-rw-r--r--   0        0        0     3950 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_redundancy.textfsm
+-rw-r--r--   0        0        0      784 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_route-map.textfsm
+-rw-r--r--   0        0        0     3318 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_running-config_partition_access-list.textfsm
+-rw-r--r--   0        0        0     1034 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_running-config_partition_route-map.textfsm
+-rw-r--r--   0        0        0      359 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_snmp_community.textfsm
+-rw-r--r--   0        0        0      802 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_snmp_group.textfsm
+-rw-r--r--   0        0        0      668 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_snmp_user.textfsm
+-rw-r--r--   0        0        0      413 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_spanning-tree.textfsm
+-rw-r--r--   0        0        0     2018 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_standby.textfsm
+-rw-r--r--   0        0        0      621 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_standby_brief.textfsm
+-rw-r--r--   0        0        0      495 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_switch_detail.textfsm
+-rw-r--r--   0        0        0      357 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_switch_detail_stack_ports.textfsm
+-rw-r--r--   0        0        0     1009 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_tacacs.textfsm
+-rw-r--r--   0        0        0     1735 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_version.textfsm
+-rw-r--r--   0        0        0     6327 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_vlan.textfsm
+-rw-r--r--   0        0        0      534 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_vrf.textfsm
+-rw-r--r--   0        0        0     1047 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_vrf_detail.textfsm
+-rw-r--r--   0        0        0     1596 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_vrrp_all.textfsm
+-rw-r--r--   0        0        0     1655 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_vrrp_brief.textfsm
+-rw-r--r--   0        0        0     1109 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_vtp_status.textfsm
+-rw-r--r--   0        0        0     1660 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_traceroute.textfsm
+-rw-r--r--   0        0        0     1781 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_access-lists.textfsm
+-rw-r--r--   0        0        0      461 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_cdp_neighbors.textfsm
+-rw-r--r--   0        0        0      689 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_cdp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0      203 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_clock.textfsm
+-rw-r--r--   0        0        0      210 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_configuration_session_summary.textfsm
+-rw-r--r--   0        0        0      954 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_cts_interface_all.textfsm
+-rw-r--r--   0        0        0      233 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_cts_interface_brief.textfsm
+-rw-r--r--   0        0        0     2143 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_environment.textfsm
+-rw-r--r--   0        0        0      384 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_environment_temperature.textfsm
+-rw-r--r--   0        0        0      147 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_feature.textfsm
+-rw-r--r--   0        0        0      178 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_fex.textfsm
+-rw-r--r--   0        0        0     1002 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_fex_id.textfsm
+-rw-r--r--   0        0        0      491 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_flogi_database.textfsm
+-rw-r--r--   0        0        0     1083 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_forwarding_adjacency.textfsm
+-rw-r--r--   0        0        0      979 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_forwarding_ipv4_route.textfsm
+-rw-r--r--   0        0        0       57 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_hostname.textfsm
+-rw-r--r--   0        0        0     2323 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_hsrp_all.textfsm
+-rw-r--r--   0        0        0     1491 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_interface.textfsm
+-rw-r--r--   0        0        0     1718 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_interface_brief.textfsm
+-rw-r--r--   0        0        0      358 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_interface_description.textfsm
+-rw-r--r--   0        0        0      364 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_interface_status.textfsm
+-rw-r--r--   0        0        0      518 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver.textfsm
+-rw-r--r--   0        0        0     2240 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver_details.textfsm
+-rw-r--r--   0        0        0      800 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_interfaces_switchport.textfsm
+-rw-r--r--   0        0        0      500 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_inventory.textfsm
+-rw-r--r--   0        0        0      698 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_adjacency.textfsm
+-rw-r--r--   0        0        0      300 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_arp.textfsm
+-rw-r--r--   0        0        0      426 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_arp_detail.textfsm
+-rw-r--r--   0        0        0     2011 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_bgp.textfsm
+-rw-r--r--   0        0        0     4318 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_neighbors.textfsm
+-rw-r--r--   0        0        0      974 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary.textfsm
+-rw-r--r--   0        0        0     1014 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary_vrf.textfsm
+-rw-r--r--   0        0        0      714 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_community-list.textfsm
+-rw-r--r--   0        0        0      283 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_dhcp_relay_address.textfsm
+-rw-r--r--   0        0        0     3956 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_dhcp_snooping_statistics.textfsm
+-rw-r--r--   0        0        0     5936 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_interface.textfsm
+-rw-r--r--   0        0        0      356 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_interface_brief.textfsm
+-rw-r--r--   0        0        0     2403 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_interface_vrf_all.textfsm
+-rw-r--r--   0        0        0      665 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_msdp_summary_vrf_all.textfsm
+-rw-r--r--   0        0        0      680 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_database.textfsm
+-rw-r--r--   0        0        0      526 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_interface_brief.textfsm
+-rw-r--r--   0        0        0      387 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_neighbor.textfsm
+-rw-r--r--   0        0        0      453 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_pim_group-range_vrf_all.textfsm
+-rw-r--r--   0        0        0      480 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_pim_interface_brief_vrf_all.textfsm
+-rw-r--r--   0        0        0      599 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_pim_neighbor_vrf_all.textfsm
+-rw-r--r--   0        0        0      546 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_pim_rp_vrf_all.textfsm
+-rw-r--r--   0        0        0     2072 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_route.textfsm
+-rw-r--r--   0        0        0      222 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ipv6_interface_brief.textfsm
+-rw-r--r--   0        0        0      244 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_l2rib_internal_permanently-frozen-list.textfsm
+-rw-r--r--   0        0        0      411 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_license_usage.textfsm
+-rw-r--r--   0        0        0      297 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_lldp_neighbors.textfsm
+-rw-r--r--   0        0        0      727 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_lldp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0      290 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_mac_address-table.textfsm
+-rw-r--r--   0        0        0      351 2023-06-27 15:17:15.900029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_module.textfsm
+-rw-r--r--   0        0        0      288 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_nve_peers.textfsm
+-rw-r--r--   0        0        0      495 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_nve_vni.textfsm
+-rw-r--r--   0        0        0     2346 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_port-channel_summary.textfsm
+-rw-r--r--   0        0        0      234 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_processes_cpu.textfsm
+-rw-r--r--   0        0        0      698 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_route-map.textfsm
+-rw-r--r--   0        0        0      489 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_spanning-tree_root.textfsm
+-rw-r--r--   0        0        0      296 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_vdc.textfsm
+-rwxr-xr-x   0        0        0      697 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_version.textfsm
+-rw-r--r--   0        0        0     6310 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_vlan.textfsm
+-rw-r--r--   0        0        0       99 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_vpc.textfsm
+-rw-r--r--   0        0        0      279 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_vrf.textfsm
+-rw-r--r--   0        0        0      239 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_vrf_interface.textfsm
+-rw-r--r--   0        0        0      594 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_s300_show_interfaces_status.textfsm
+-rw-r--r--   0        0        0      411 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_s300_show_lldp_neighbors.textfsm
+-rw-r--r--   0        0        0      330 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_s300_show_mac_address-table.textfsm
+-rw-r--r--   0        0        0      442 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_s300_show_version.textfsm
+-rw-r--r--   0        0        0     3155 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a.textfsm
+-rw-r--r--   0        0        0     4795 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a_cleanair_config.textfsm
+-rw-r--r--   0        0        0     1683 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_advanced_802.11a_channel.textfsm
+-rw-r--r--   0        0        0     2697 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_config_general.textfsm
+-rw-r--r--   0        0        0      643 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_image_all.textfsm
+-rw-r--r--   0        0        0      492 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_summary.textfsm
+-rw-r--r--   0        0        0      780 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_band-select.textfsm
+-rw-r--r--   0        0        0      661 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_cdp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0     1429 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_client_detail.textfsm
+-rw-r--r--   0        0        0      276 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_exclusionlist.textfsm
+-rw-r--r--   0        0        0      355 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_flexconnect_group_summary.textfsm
+-rw-r--r--   0        0        0     1437 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_detailed_id.textfsm
+-rw-r--r--   0        0        0      347 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_group_summary.textfsm
+-rw-r--r--   0        0        0      480 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_summary.textfsm
+-rw-r--r--   0        0        0      436 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_inventory.textfsm
+-rw-r--r--   0        0        0      463 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_mobility_anchor.textfsm
+-rw-r--r--   0        0        0      737 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_mobility_sum.textfsm
+-rw-r--r--   0        0        0      655 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_port_summary.textfsm
+-rw-r--r--   0        0        0     2799 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_radius_summary.textfsm
+-rw-r--r--   0        0        0      842 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_detail.textfsm
+-rw-r--r--   0        0        0      970 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_summary.textfsm
+-rw-r--r--   0        0        0      417 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_rf-profile_summary.textfsm
+-rw-r--r--   0        0        0      997 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_stats_port_summary.textfsm
+-rw-r--r--   0        0        0     1238 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_sysinfo.textfsm
+-rw-r--r--   0        0        0     1450 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_tacacs_summary.textfsm
+-rw-r--r--   0        0        0      906 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_time.textfsm
+-rw-r--r--   0        0        0      420 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_wlan_sum.textfsm
+-rw-r--r--   0        0        0     6223 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_admin_show_controller_fabric_health.textfsm
+-rw-r--r--   0        0        0     1379 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_admin_show_environment_fan.textfsm
+-rw-r--r--   0        0        0      309 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_admin_show_environment_power.textfsm
+-rw-r--r--   0        0        0      398 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_admin_show_inventory.textfsm
+-rw-r--r--   0        0        0      179 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_admin_show_platform.textfsm
+-rw-r--r--   0        0        0      419 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_admin_show_vm.textfsm
+-rw-r--r--   0        0        0      515 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_arp.textfsm
+-rw-r--r--   0        0        0      838 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_asic-errors_all_location.textfsm
+-rw-r--r--   0        0        0      179 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_bfd_sessions.textfsm
+-rw-r--r--   0        0        0     1905 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_bgp.textfsm
+-rw-r--r--   0        0        0      725 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_bgp_instance_all_summary.textfsm
+-rw-r--r--   0        0        0     5397 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_bgp_neighbors.textfsm
+-rw-r--r--   0        0        0      156 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_bgp_vrf_all_ipv4_unicast_summary.textfsm
+-rw-r--r--   0        0        0      513 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_cdp_neighbors_detail.textfsm
+-rw-r--r--   0        0        0     1544 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_cef_drops_location.textfsm
+-rw-r--r--   0        0        0      337 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_configuration_commit_list.textfsm
+-rw-r--r--   0        0        0      347 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_controller_fabric_plane_all.textfsm
+-rw-r--r--   0        0        0     2208 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_controllers_HundredGigabitEthernet.textfsm
+-rw-r--r--   0        0        0     2281 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_controllers_all_phy.textfsm
+-rw-r--r--   0        0        0     2823 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_egress_location.textfsm
+-rw-r--r--   0        0        0     1961 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_ingress_location.textfsm
+-rw-r--r--   0        0        0      426 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_errors_egress_location.textfsm
+-rw-r--r--   0        0        0     1406 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_errors_ingress_location.textfsm
+-rw-r--r--   0        0        0     4953 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_controllers_hundredgige_all.textfsm
+-rw-r--r--   0        0        0      266 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_dhcp_ipv4_proxy_binding.textfsm
+-rw-r--r--   0        0        0     7430 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_drops_np_all.textfsm
+-rw-r--r--   0        0        0      518 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_hsrp.textfsm
+-rw-r--r--   0        0        0      665 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_install_active.textfsm
+-rw-r--r--   0        0        0      268 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_interface_brief.textfsm
+-rw-r--r--   0        0        0      835 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_interfaces.textfsm
+-rw-r--r--   0        0        0      353 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_interfaces_summary.textfsm
+-rw-r--r--   0        0        0      571 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_ip_bgp_summary.textfsm
+-rw-r--r--   0        0        0      178 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_ip_interface_brief.textfsm
+-rw-r--r--   0        0        0     1094 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_ip_route.textfsm
+-rw-r--r--   0        0        0      769 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_ipv4_interface.textfsm
+-rw-r--r--   0        0        0      270 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_ipv4_vrf_all_interface_brief.textfsm
+-rw-r--r--   0        0        0      405 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_ipv6_neighbors.textfsm
+-rw-r--r--   0        0        0      288 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_isis_neighbors.textfsm
+-rw-r--r--   0        0        0      380 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_lldp_neighbors.textfsm
+-rw-r--r--   0        0        0      694 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_lpts_pifib_hardware_police_location.textfsm
+-rw-r--r--   0        0        0      398 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_mpls_ldp_neighbor_brief.textfsm
+-rw-r--r--   0        0        0      356 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_ospf_neighbor.textfsm
+-rw-r--r--   0        0        0      440 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_ospf_vrf_all_interface_brief.textfsm
+-rw-r--r--   0        0        0      474 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_ospf_vrf_all_neighbor.textfsm
+-rw-r--r--   0        0        0      359 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_pim_ipv4_group-map.textfsm
+-rw-r--r--   0        0        0      481 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_pim_ipv4_interface.textfsm
+-rw-r--r--   0        0        0      447 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_pim_ipv4_neighbor.textfsm
+-rw-r--r--   0        0        0      262 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_pim_neighbor.textfsm
+-rw-r--r--   0        0        0     1074 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_platform_summary_location_all.textfsm
+-rw-r--r--   0        0        0      205 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_processes_cpu.textfsm
+-rw-r--r--   0        0        0      187 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_redundancy_summary.textfsm
+-rw-r--r--   0        0        0      226 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_rsvp_neighbors.textfsm
+-rw-r--r--   0        0        0      856 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_version.textfsm
+-rw-r--r--   0        0        0      339 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_version_brief.textfsm
+-rw-r--r--   0        0        0      422 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_vrf_all_detail.textfsm
+-rw-r--r--   0        0        0      290 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/dell_force10_show_arp.textfsm
+-rw-r--r--   0        0        0      213 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/dell_force10_show_ip_interface_brief.textfsm
+-rw-r--r--   0        0        0      211 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/dell_force10_show_version.textfsm
+-rw-r--r--   0        0        0      815 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/dell_force10_show_vlan.textfsm
+-rw-r--r--   0        0        0      248 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/dell_force10_show_vlan_brief.textfsm
+-rw-r--r--   0        0        0      289 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/dell_powerconnect_show_bridge_address_table.textfsm
+-rw-r--r--   0        0        0      193 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/dell_powerconnect_show_interfaces_description.textfsm
+-rw-r--r--   0        0        0      592 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/dell_powerconnect_show_interfaces_status.textfsm
+-rw-r--r--   0        0        0      301 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/dlink_ds_show_arpentry.textfsm
+-rw-r--r--   0        0        0      647 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/ericsson_ipos_show_arp.textfsm
+-rw-r--r--   0        0        0      433 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/ericsson_ipos_show_isis_adjacency.textfsm
+-rw-r--r--   0        0        0      168 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/ericsson_ipos_show_version.textfsm
+-rw-r--r--   0        0        0      574 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/fortinet_get_router_info_bgp_summary.textfsm
+-rw-r--r--   0        0        0      230 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/fortinet_get_system_arp.textfsm
+-rw-r--r--   0        0        0     2048 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/fortinet_get_system_ha_status.textfsm
+-rw-r--r--   0        0        0     8998 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/fortinet_get_system_interface.textfsm
+-rw-r--r--   0        0        0      657 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/fortinet_get_system_interface_physical.textfsm
+-rw-r--r--   0        0        0     2528 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/fortinet_get_system_status.textfsm
+-rw-r--r--   0        0        0      238 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_arp.textfsm
+-rw-r--r--   0        0        0      200 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_clock.textfsm
+-rw-r--r--   0        0        0      519 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_counters_bound_interface.textfsm
+-rw-r--r--   0        0        0      666 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_device_manuinfo.textfsm
+-rw-r--r--   0        0        0     8519 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_interface.textfsm
+-rw-r--r--   0        0        0     1573 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_ip_interface.textfsm
+-rw-r--r--   0        0        0      616 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_ip_routing-table.textfsm
+-rw-r--r--   0        0        0      195 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_ip_vpn-instance.textfsm
+-rw-r--r--   0        0        0     5480 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_ip_vpn-instance_instance-name.textfsm
+-rw-r--r--   0        0        0      777 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_link-aggregation_verbose.textfsm
+-rw-r--r--   0        0        0      647 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_list.textfsm
+-rw-r--r--   0        0        0      926 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_verbose.textfsm
+-rw-r--r--   0        0        0      187 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_mac-address.textfsm
+-rw-r--r--   0        0        0      632 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_vlan_all.textfsm
+-rw-r--r--   0        0        0      106 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_vlan_brief.textfsm
+-rw-r--r--   0        0        0      179 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_procurve_show_arp.textfsm
+-rw-r--r--   0        0        0      710 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_procurve_show_interfaces.textfsm
+-rw-r--r--   0        0        0      917 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_procurve_show_interfaces_brief.textfsm
+-rw-r--r--   0        0        0      706 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device.textfsm
+-rw-r--r--   0        0        0     1699 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device_detail.textfsm
+-rw-r--r--   0        0        0      222 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_procurve_show_mac-address.textfsm
+-rw-r--r--   0        0        0      453 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_procurve_show_port-security.textfsm
+-rw-r--r--   0        0        0     1329 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_procurve_show_system.textfsm
+-rw-r--r--   0        0        0      385 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_procurve_show_tech_buffers.textfsm
+-rw-r--r--   0        0        0      407 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_procurve_show_trunks.textfsm
+-rw-r--r--   0        0        0      290 2023-06-27 15:17:15.904029 ntc_templates-3.5.0/ntc_templates/templates/hp_procurve_show_vlans.textfsm
+-rw-r--r--   0        0        0     1392 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_acl_all.textfsm
+-rw-r--r--   0        0        0      551 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_arp_all.textfsm
+-rw-r--r--   0        0        0      491 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_arp_brief.textfsm
+-rw-r--r--   0        0        0     3608 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_interface.textfsm
+-rw-r--r--   0        0        0      498 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_interface_brief.textfsm
+-rw-r--r--   0        0        0      376 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_interface_description.textfsm
+-rw-r--r--   0        0        0     2059 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_ip_routing-table_verbose.textfsm
+-rw-r--r--   0        0        0      843 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_ipv6_neighbors.textfsm
+-rw-r--r--   0        0        0      435 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_isis_peer.textfsm
+-rw-r--r--   0        0        0     1811 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_lldp_neighbor.textfsm
+-rw-r--r--   0        0        0      713 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_nat_server.textfsm
+-rw-r--r--   0        0        0     7310 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_port_vlan.textfsm
+-rw-r--r--   0        0        0      193 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_service-set_all.textfsm
+-rw-r--r--   0        0        0     1084 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_service-set_id_id.textfsm
+-rw-r--r--   0        0        0       96 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_sn_license.textfsm
+-rw-r--r--   0        0        0      424 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_snmp-agent_community_read.textfsm
+-rw-r--r--   0        0        0     1346 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_startup.textfsm
+-rw-r--r--   0        0        0      390 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_temperature.textfsm
+-rw-r--r--   0        0        0      522 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_traffic-filter_applied-record.textfsm
+-rw-r--r--   0        0        0      505 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_version.textfsm
+-rw-r--r--   0        0        0    52721 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/index
+-rw-r--r--   0        0        0      536 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/ipinfusion_ocnos_show_lldp_table.textfsm
+-rw-r--r--   0        0        0      303 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_arp_no-resolve.textfsm
+-rw-r--r--   0        0        0     3195 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_interfaces.textfsm
+-rw-r--r--   0        0        0      803 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_status.textfsm
+-rw-r--r--   0        0        0      341 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_chassis_firmware.textfsm
+-rw-r--r--   0        0        0      855 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_chassis_hardware.textfsm
+-rw-r--r--   0        0        0      729 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_ethernet-switching_table.textfsm
+-rw-r--r--   0        0        0      553 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_interfaces.textfsm
+-rw-r--r--   0        0        0      267 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_isis_adjacency.textfsm
+-rw-r--r--   0        0        0      630 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_lacp_interfaces.textfsm
+-rw-r--r--   0        0        0      389 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_lldp_neighbors.textfsm
+-rw-r--r--   0        0        0      292 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_ospf_neighbor.textfsm
+-rw-r--r--   0        0        0     1374 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_system_uptime.textfsm
+-rw-r--r--   0        0        0     4359 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_version.textfsm
+-rw-r--r--   0        0        0      318 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_vlans.textfsm
+-rw-r--r--   0        0        0      768 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/juniper_screenos_get_route.textfsm
+-rw-r--r--   0        0        0      338 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/linux_arp_-a.textfsm
+-rw-r--r--   0        0        0      915 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/linux_ip_address_show.textfsm
+-rw-r--r--   0        0        0     1092 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/linux_ip_link_show.textfsm
+-rw-r--r--   0        0        0      618 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/linux_ip_route_show.textfsm
+-rw-r--r--   0        0        0      134 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/linux_ip_vrf_show.textfsm
+-rw-r--r--   0        0        0      660 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/mikrotik_routeros_interface_ethernet_monitor_name_once.textfsm
+-rw-r--r--   0        0        0      364 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/mikrotik_routeros_ip_arp_print_without-paging.textfsm
+-rw-r--r--   0        0        0      899 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/mikrotik_routeros_ip_dhcp-server_lease_print_without-paging.textfsm
+-rw-r--r--   0        0        0      331 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_address-list_print_terse.textfsm
+-rw-r--r--   0        0        0     2499 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_filter_print_all_without-paging.textfsm
+-rw-r--r--   0        0        0     2229 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_nat_print_all_without-paging.textfsm
+-rw-r--r--   0        0        0      546 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/mikrotik_routeros_ip_route_print_terse.textfsm
+-rw-r--r--   0        0        0      400 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/mikrotik_routeros_ipv6_neighbor_print_without-paging.textfsm
+-rw-r--r--   0        0        0      483 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/mikrotik_routeros_snmp_community_print_without-paging.textfsm
+-rw-r--r--   0        0        0      673 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/mikrotik_routeros_system_routerboard_print.textfsm
+-rw-r--r--   0        0        0      169 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/paloalto_panos_debug_swm_status.textfsm
+-rw-r--r--   0        0        0      337 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/paloalto_panos_show_arp_all.textfsm
+-rw-r--r--   0        0        0      249 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/paloalto_panos_show_counter_global.textfsm
+-rw-r--r--   0        0        0     1943 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/paloalto_panos_show_high-availability_all.textfsm
+-rw-r--r--   0        0        0      293 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/paloalto_panos_show_interface_hardware.textfsm
+-rw-r--r--   0        0        0      256 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/paloalto_panos_show_interface_logical.textfsm
+-rw-r--r--   0        0        0      962 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/paloalto_panos_show_interface_management.textfsm
+-rw-r--r--   0        0        0      415 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/paloalto_panos_show_jobs_all.textfsm
+-rw-r--r--   0        0        0      236 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/paloalto_panos_show_mac_all.textfsm
+-rw-r--r--   0        0        0      729 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/paloalto_panos_show_running_nat-policy.textfsm
+-rw-r--r--   0        0        0      794 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/paloalto_panos_show_running_security-policy.textfsm
+-rw-r--r--   0        0        0      840 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/paloalto_panos_show_system_info.textfsm
+-rw-r--r--   0        0        0      975 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/paloalto_panos_test_security-policy-match.textfsm
+-rw-r--r--   0        0        0      908 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/ruckus_fastiron_show_arp.textfsm
+-rw-r--r--   0        0        0      693 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/ruckus_fastiron_show_interfaces.textfsm
+-rw-r--r--   0        0        0      602 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/ruckus_fastiron_show_interfaces_brief.textfsm
+-rw-r--r--   0        0        0      279 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/ruckus_fastiron_show_mac-address.textfsm
+-rw-r--r--   0        0        0      263 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/ruckus_fastiron_show_media_validation.textfsm
+-rw-r--r--   0        0        0     1049 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/ruckus_fastiron_show_version.textfsm
+-rw-r--r--   0        0        0     2669 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/ruckus_fastiron_show_vlan.textfsm
+-rw-r--r--   0        0        0      401 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/ubiquiti_edgerouter_show_arp.textfsm
+-rw-r--r--   0        0        0      372 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/ubiquiti_edgerouter_show_dhcp_leases.textfsm
+-rw-r--r--   0        0        0      270 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/ubiquiti_edgerouter_show_dhcpv6_server_leases.textfsm
+-rw-r--r--   0        0        0      300 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/ubiquiti_edgerouter_show_interfaces.textfsm
+-rw-r--r--   0        0        0      307 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/ubiquiti_edgerouter_show_interfaces_ethernet_physical.textfsm
+-rw-r--r--   0        0        0      662 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/ubiquiti_edgerouter_show_ip_route.textfsm
+-rw-r--r--   0        0        0      233 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/ubiquiti_edgerouter_show_ipv6_neighbors.textfsm
+-rw-r--r--   0        0        0      471 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/ubiquiti_edgerouter_show_ipv6_route.textfsm
+-rw-r--r--   0        0        0      723 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/ubiquiti_edgerouter_show_nat_rules.textfsm
+-rw-r--r--   0        0        0      380 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/ubiquiti_edgerouter_show_version.textfsm
+-rw-r--r--   0        0        0      314 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/ubiquiti_edgeswitch_show_arp.textfsm
+-rw-r--r--   0        0        0      553 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/ubiquiti_edgeswitch_show_version.textfsm
+-rw-r--r--   0        0        0      209 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/ubiquiti_edgeswitch_show_vlan.textfsm
+-rw-r--r--   0        0        0      470 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/vmware_nsxv_show_ip_bgp_neighbors.textfsm
+-rw-r--r--   0        0        0      259 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/vmware_nsxv_show_ip_route.textfsm
+-rw-r--r--   0        0        0      281 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/vyatta_vyos_show_arp.textfsm
+-rw-r--r--   0        0        0      374 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/vyatta_vyos_show_interfaces.textfsm
+-rw-r--r--   0        0        0      859 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/vyatta_vyos_show_ip_bgp_summary.textfsm
+-rw-r--r--   0        0        0      231 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/watchguard_firebox_show_arp.textfsm
+-rw-r--r--   0        0        0     1181 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/yamaha_show_environment.textfsm
+-rw-r--r--   0        0        0      472 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/yamaha_show_ip_route.textfsm
+-rw-r--r--   0        0        0      626 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_cfg_firewall_acl_get.textfsm
+-rw-r--r--   0        0        0      402 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_cfg_intf_group_get.textfsm
+-rw-r--r--   0        0        0      563 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_cfg_ipalias_get.textfsm
+-rw-r--r--   0        0        0      409 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_cfg_lan_get.textfsm
+-rw-r--r--   0        0        0      662 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_cfg_lan_get_--Name_name.textfsm
+-rw-r--r--   0        0        0      411 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_cfg_lanhosts_get.textfsm
+-rw-r--r--   0        0        0      664 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_cfg_nat_addr_map_get.textfsm
+-rw-r--r--   0        0        0      751 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_cfg_nat_get.textfsm
+-rw-r--r--   0        0        0      629 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_cfg_snmp_get.textfsm
+-rw-r--r--   0        0        0      339 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_cfg_static_dhcp_get.textfsm
+-rw-r--r--   0        0        0      625 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_cfg_static_route_get.textfsm
+-rw-r--r--   0        0        0      539 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_cfg_wlan_get.textfsm
+-rw-r--r--   0        0        0      857 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_sys_atsh.textfsm
+-rw-r--r--   0        0        0      337 2023-06-27 15:17:15.908029 ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_zycli_Ethctl_media-type.textfsm
+-rw-r--r--   0        0        0     3098 2023-06-27 15:17:26.300059 ntc_templates-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3871 1970-01-01 00:00:00.000000 ntc_templates-3.5.0/PKG-INFO
```

### Comparing `ntc_templates-3.4.0/LICENSE` & `ntc_templates-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/README.md` & `ntc_templates-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/parse.py` & `ntc_templates-3.5.0/ntc_templates/parse.py`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/alcatel_aos_show_vlan.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/alcatel_aos_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_port.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_port.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_bgp_summary_family.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_router_bgp_summary_family.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_interface.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_router_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_ldp_interface.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_router_ldp_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_mpls_interface.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_router_mpls_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_mpls_lsp.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_router_mpls_lsp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_ospf_interface.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_router_ospf_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_router_rsvp_interface.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_router_rsvp_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_service_id_base.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_service_id_base.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_service_sap-using.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_service_sap-using.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_service_sdp-using.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_service_sdp-using.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_service_sdp.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_service_sdp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/alcatel_sros_show_system_cpu.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/alcatel_sros_show_system_cpu.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_environment_cooling.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_environment_cooling.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_environment_temperature.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_environment_temperature.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_interfaces.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_interfaces_transceiver_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_interfaces_transceiver_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_inventory.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_inventory.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_access-lists.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_ip_access-lists.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_bgp.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_ip_bgp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_bgp_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_ip_bgp_summary.textfsm`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Value Filldown ROUTER_ID (\d+\.\d+\.\d+\.\d+)
 Value Filldown LOCAL_AS (\d+)
 Value Filldown VRF (\S+)
 Value DESCRIPTION (\S+)
 Value Required BGP_NEIGH (\d+\.\d+\.\d+\.\d+)
-Value NEIGH_AS (\d+)
+Value NEIGH_AS (\d+|\d+\.\d+)
 Value MSG_RCVD (\d+)
 Value MSG_SENT (\d+)
 Value IN_QUEUE (\d+)
 Value OUT_QUEUE (\d+)
 Value UP_DOWN (\S+)
 Value STATE (\S+)
 Value STATE_PFXRCD (\d+)
```

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_ospf_database.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_ip_ospf_database.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_ospf_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_ip_ospf_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ip_route.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_ip_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_ipv6_bgp_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_ipv6_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_lldp_neighbors_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_lldp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_mac_address-table.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_mac_address-table.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_mac_security_participants_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_mac_security_participants_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_module.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_module.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_pim_ipv4_interface.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_pim_ipv4_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_port-channel_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_port-channel_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_processes_top_once.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_processes_top_once.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_reload_cause.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_reload_cause.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_vlan.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/arista_eos_show_vrf.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/arista_eos_show_vrf.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_aaa_authentication_port-access_interface_all_client-status.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/aruba_aoscx_show_aaa_authentication_port-access_interface_all_client-status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_bfd_all-vrfs.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/aruba_aoscx_show_bfd_all-vrfs.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_bgp_all-vrfs_all_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/aruba_aoscx_show_bgp_all-vrfs_all_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_bgp_all_all-vrfs_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/aruba_aoscx_show_bgp_all_all-vrfs_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_interface.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/aruba_aoscx_show_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_interface_dom_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/aruba_aoscx_show_interface_dom_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_lldp_neighbors-info_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/aruba_aoscx_show_lldp_neighbors-info_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/aruba_aoscx_show_vsf_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/aruba_aoscx_show_vsf_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_ap_bss-table_details.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/aruba_os_show_ap_bss-table_details.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_ap_database.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/aruba_os_show_ap_database.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_ap_database_long.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/aruba_os_show_ap_database_long.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_ap_radio-database.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/aruba_os_show_ap_radio-database.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/aruba_os_show_arp.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/aruba_os_show_arp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_logging_config.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/avaya_ers_show_logging_config.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_mlt.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/avaya_ers_show_mlt.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_mlt_all-members.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/avaya_ers_show_mlt_all-members.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/avaya_ers_show_sys-info.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/avaya_ers_show_sys-info.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/broadcom_icos_show_isdp_neighbors.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/broadcom_icos_show_isdp_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/broadcom_icos_show_lldp_remote-device_all.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/broadcom_icos_show_lldp_remote-device_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/broadcom_icos_show_version.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/broadcom_icos_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_interfaces.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_interfaces_brief.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_interfaces_brief.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_lldp_neighbors_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_lldp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_metro.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_metro.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_running-config_vlan.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_running-config_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_span.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_span.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_trunk.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_trunk.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/brocade_fastiron_show_version.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/brocade_fastiron_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_interfaces.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/brocade_netiron_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_lldp_neighbors_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/brocade_netiron_show_lldp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_metro.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/brocade_netiron_show_metro.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_running-config_interface.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/brocade_netiron_show_running-config_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_running-config_vlan.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/brocade_netiron_show_running-config_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_span.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/brocade_netiron_show_span.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/brocade_netiron_show_topo.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/brocade_netiron_show_topo.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_interfaces_all.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/checkpoint_gaia_show_interfaces_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/checkpoint_gaia_show_route.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/checkpoint_gaia_show_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_port_show.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/ciena_saos_port_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_rstp_show.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/ciena_saos_rstp_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_software_show.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/ciena_saos_software_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_traffic-profiling_standard-profile_show.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/ciena_saos_traffic-profiling_standard-profile_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/ciena_saos_vlan_show.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/ciena_saos_vlan_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_apic_fabric_show_vlan_extended.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_apic_fabric_show_vlan_extended.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_dir.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_dir.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_ping.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_ping.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_access-list.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_access-list.textfsm`

 * *Files 18% similar despite different names*

```diff
@@ -7,65 +7,85 @@
 Value ACTION (permit|deny)
 Value PROTOCOL ([a-z]+)
 Value SVC_OBJECT_GRP (\S+)
 Value SVC_OBJECT (\S+)
 Value SRC_INTFC (\S+)
 Value SRC_OBJECT_GRP (\S+)
 Value SRC_OBJECT (\S+)
-Value SRC_HOST (\S+)
+Value SRC_HOST (\d+\.\d+\.\d+\.\d+)
+Value SRC_V6HOST ([0-9a-f:]+)
 Value SRC_NETWORK (\d+\.\d+\.\d+\.\d+)
+Value SRC_V6NETWORK ([0-9a-f:]+)
 Value SRC_MASK (\d+\.\d+\.\d+\.\d+)
+Value SRC_V6MASK (\d{1,3})
 Value SRC_ANY (any[46]{0,1})
 Value DST_INTFC (\S+)
 Value DST_OBJECT_GRP (\S+)
 Value DST_OBJECT (\S+)
-Value DST_HOST (\S+)
+Value DST_HOST (\d+\.\d+\.\d+\.\d+)
+Value DST_V6HOST ([0-9a-f:]+)
 Value DST_NETWORK (\d+\.\d+\.\d+\.\d+)
+Value DST_V6NETWORK ([0-9a-f:]+)
 Value DST_MASK (\d+\.\d+\.\d+\.\d+)
+Value DST_V6MASK (\d{1,3})
 Value DST_ANY (any[46]{0,1})
 Value DST_PORT (\S+)
+Value DST_PORT_LESS_THAN (\S+)
+Value DST_PORT_GREATER_THAN (\S+)
+Value DST_PORT_RANGE_START (\S+)
+Value DST_PORT_RANGE_END (\S+)
 Value DST_PORT_GRP (\S+)
 Value DST_PORT_OBJECT (\S+)
+Value DST_ICMP_TYPE ((?!log|time|inactive)\S+)
 Value LOG_LEVEL ([a-z0-9]+)
 Value LOG_INTERVAL (\d+)
+Value TIME_RANGE (\S+)
 Value STATE (inactive)
 Value HIT_COUNT (\d+)
 Value LINE_HASH (0x\w+)
 Value ENTRY_PROTOCOL_ICMP (icmp)
 Value ENTRY_PROTOCOL ([a-z\-]+)
 Value ENTRY_SRC_FQDN (\S+)
 Value ENTRY_SRC_RANGE_START (\d+\.\d+\.\d+\.\d+)
 Value ENTRY_SRC_RANGE_END (\d+\.\d+\.\d+\.\d+)
 Value ENTRY_SRC_HOST (\d+\.\d+\.\d+\.\d+)
+Value ENTRY_SRC_V6HOST ([0-9a-f:]+)
 Value ENTRY_SRC_NETWORK (\d+\.\d+\.\d+\.\d+)
+Value ENTRY_SRC_V6NETWORK ([0-9a-f:]+)
 Value ENTRY_SRC_MASK (\d+\.\d+\.\d+\.\d+)
+Value ENTRY_SRC_V6MASK (\d{1,3})
 Value ENTRY_SRC_ANY (any[46]{0,1})
 Value ENTRY_SRC_FQDN_STATE (unresolved)
 Value ENTRY_DST_FQDN (\S+)
 Value ENTRY_DST_RANGE_START (\d+\.\d+\.\d+\.\d+)
 Value ENTRY_DST_RANGE_END (\d+\.\d+\.\d+\.\d+)
 Value ENTRY_DST_HOST (\S+)
+Value ENTRY_DST_V6HOST ([0-9a-f:]+)
 Value ENTRY_DST_NETWORK (\d+\.\d+\.\d+\.\d+)
+Value ENTRY_DST_V6NETWORK ([0-9a-f:]+)
 Value ENTRY_DST_MASK (\d+\.\d+\.\d+\.\d+)
+Value ENTRY_DST_V6MASK (\d{1,3})
 Value ENTRY_DST_ANY (any[46]{0,1})
 Value ENTRY_DST_FQDN_STATE (unresolved)
-Value ENTRY_ICMP_TYPE (echo-reply|unreachable|echo|time-exceeded)
+Value ENTRY_ICMP_TYPE (alternate-address|conversion-error|echo|echo-reply|information-reply|information-request|mask-reply|mask-request|mobile-redirect|parameter-problem|redirect|router-advertisement|router-solicitation|source-quench|time-exceeded|timestamp-reply|timestamp-request|traceroute|unreachable|\d{1,3})
 Value ENTRY_ICMP_CODE (\d+)
 Value ENTRY_PORT ([a-z\-]+\s+\d+|[\w\-]+)
-Value ENTRY_PORT_LESS_THAN ([a-z\-]+\s+\d+|\w+)
-Value ENTRY_PORT_GREATER_THAN ([a-z\-]+\s+\d+|\w+)
-Value ENTRY_PORT_RANGE_START ([a-z\-]+\s+\d+|\w+)
-Value ENTRY_PORT_RANGE_END ([a-z\-]+\s+\d+|\w+)
+Value ENTRY_PORT_LESS_THAN ([a-z\-]+\s+\d+|\S+)
+Value ENTRY_PORT_GREATER_THAN ([a-z\-]+\s+\d+|\S+)
+Value ENTRY_PORT_RANGE_START ([a-z\-]+\s+\d+|\S+)
+Value ENTRY_PORT_RANGE_END ([a-z\-]+\s+\d+|\S+)
 Value ENTRY_HIT_COUNT (\d+)
 Value ENTRY_STATE (inactive)
 Value ENTRY_HASH (0x\w+)
 
+
 Start
   ^access\-list\s+${ACL_NAME};\s+${ACL_TOT_ELEM}\s+elements;\s+name\s+hash:\s+${ACL_NAME_HASH}\s* -> Record
-  ^access-list\s+${ACL_NAME}\s+line\s+${LINE_NUM}\s+remark\s+${REMARK}\s*$$ -> Record
-  ^access\-list\s+${ACL_NAME}\s+line\s+${LINE_NUM}\s+${TYPE}\s+${ACTION}\s+(object\-group\s+${SVC_OBJECT_GRP}|object\s+${SVC_OBJECT}|${PROTOCOL})\s+(interface\s+${SRC_INTFC}|object\-group\s+${SRC_OBJECT_GRP}|object\s+${SRC_OBJECT}|host\s+${SRC_HOST}|${SRC_NETWORK}\s+${SRC_MASK}|${SRC_ANY})\s+(interface\s+${DST_INTFC}|object\-group\s+${DST_OBJECT_GRP}|object\s+${DST_OBJECT}|host\s+${DST_HOST}|${DST_NETWORK}\s+${DST_MASK}|${DST_ANY})\s+((eq\s+${DST_PORT}|object\-group\s+${DST_PORT_GRP}|object\s+${DST_PORT_OBJECT})\s+){0,1}(${ENTRY_ICMP_TYPE}(\s+${ENTRY_ICMP_CODE}){0,1}\s+){0,1}((log\s+(${LOG_LEVEL}\s+interval\s+${LOG_INTERVAL}|disable|default))\s+){0,1}(${STATE}\s+){0,1}\(hitcnt=${HIT_COUNT}\)\s+(\(inactive\)\s+){0,1}${LINE_HASH}\s* -> Record
-  ^\s+access\-list\s+${ACL_NAME}\s+line\s+${LINE_NUM}\s+(standard|extended)\s+(permit|deny)\s+${ENTRY_PROTOCOL_ICMP}\s+(fqdn\s+${ENTRY_SRC_FQDN}|range\s+${ENTRY_SRC_RANGE_START}\s+${ENTRY_SRC_RANGE_END}|host\s+${ENTRY_SRC_HOST}|${ENTRY_SRC_NETWORK}\s+${ENTRY_SRC_MASK}|${ENTRY_SRC_ANY})\s+(\(${ENTRY_SRC_FQDN_STATE}\)\s+){0,1}(fqdn\s+${ENTRY_DST_FQDN}|range\s+${ENTRY_DST_RANGE_START}\s+${ENTRY_DST_RANGE_END}|host\s+${ENTRY_DST_HOST}|${ENTRY_DST_NETWORK}\s+${ENTRY_DST_MASK}|${ENTRY_DST_ANY})\s+(\(${ENTRY_DST_FQDN_STATE}\)\s+){0,1}(${ENTRY_ICMP_TYPE}(\s+${ENTRY_ICMP_CODE}){0,1}\s+){0,1}(log\s+(${LOG_LEVEL}\s+interval\s+${LOG_INTERVAL}|disable|default)\s+){0,1}(inactive){0,1}\s*(\(hitcnt=${ENTRY_HIT_COUNT}\)){0,1}\s*(\(${ENTRY_STATE}\)){0,1}\s+${ENTRY_HASH}\s* -> Record
-  ^\s+access\-list\s+${ACL_NAME}\s+line\s+${LINE_NUM}\s+(standard|extended)\s+(permit|deny)\s+(${ENTRY_PROTOCOL}\s+){0,1}(fqdn\s+${ENTRY_SRC_FQDN}|range\s+${ENTRY_SRC_RANGE_START}\s+${ENTRY_SRC_RANGE_END}|host\s+${ENTRY_SRC_HOST}|${ENTRY_SRC_NETWORK}\s+${ENTRY_SRC_MASK}|${ENTRY_SRC_ANY})\s+(\(${ENTRY_SRC_FQDN_STATE}\)\s+){0,1}((fqdn\s+${ENTRY_DST_FQDN}|range\s+${ENTRY_DST_RANGE_START}\s+${ENTRY_DST_RANGE_END}|host\s+${ENTRY_DST_HOST}|${ENTRY_DST_NETWORK}\s+${ENTRY_DST_MASK}|${ENTRY_DST_ANY})\s+){0,1}(\(${ENTRY_DST_FQDN_STATE}\)\s+){0,1}((eq\s+${ENTRY_PORT}|lt\s+${ENTRY_PORT_LESS_THAN}|gt\s+${ENTRY_PORT_GREATER_THAN}|range\s+${ENTRY_PORT_RANGE_START}\s+${ENTRY_PORT_RANGE_END})\s+){0,1}(log\s+([a-z0-9]+\s+interval\s+\d+|disable|default)\s+){0,1}(inactive){0,1}\s*(\(hitcnt=${ENTRY_HIT_COUNT}\)){0,1}\s*(\(${ENTRY_STATE}\)){0,1}\s+${ENTRY_HASH}\s* -> Record
-  ^access\-list\s+${ACL_NAME}\s+line\s+${LINE_NUM}\s+(standard|extended)\s+(permit|deny)\s+(fqdn\s+${ENTRY_SRC_FQDN}|range\s+${ENTRY_SRC_RANGE_START}\s+${ENTRY_SRC_RANGE_END}|host\s+${ENTRY_SRC_HOST}|${ENTRY_SRC_NETWORK}\s+${ENTRY_SRC_MASK}|${ENTRY_SRC_ANY})\s+\((hitcnt=${ENTRY_HIT_COUNT})\)\s+${ENTRY_HASH}\s* -> Record
+  ^access\-list\s+cached\s+ACL\s+log\s+flows.* -> NoRecord
+  ^\s+alert-interval\s+\d+ -> NoRecord
+  ^access\-list\s+${ACL_NAME}\s+line\s+${LINE_NUM}\s+remark\s+${REMARK}\s*$$ -> Record
+  ^access\-list\s+${ACL_NAME}\s+line\s+${LINE_NUM}\s+${TYPE}\s+${ACTION}\s+(object\-group\s+${SVC_OBJECT_GRP}|object\s+${SVC_OBJECT}|${PROTOCOL})\s+(interface\s+${SRC_INTFC}|object\-group\s+${SRC_OBJECT_GRP}|object\s+${SRC_OBJECT}|host\s+(${SRC_HOST}|${SRC_V6HOST})|${SRC_NETWORK}\s+${SRC_MASK}|${SRC_V6NETWORK}\/${SRC_V6MASK}|${SRC_ANY})\s+(interface\s+${DST_INTFC}|object\-group\s+${DST_OBJECT_GRP}|object\s+${DST_OBJECT}|host\s+(${DST_HOST}|${DST_V6HOST})|${DST_NETWORK}\s+${DST_MASK}|${DST_V6NETWORK}\/${DST_V6MASK}|${DST_ANY})\s+((eq\s+${DST_PORT}|lt\s+${DST_PORT_LESS_THAN}|gt\s+${DST_PORT_GREATER_THAN}|range\s+${DST_PORT_RANGE_START}\s+${DST_PORT_RANGE_END}|object\-group\s+${DST_PORT_GRP}|object\s+${DST_PORT_OBJECT})\s+){0,1}(${ENTRY_ICMP_TYPE}(\s+${ENTRY_ICMP_CODE}){0,1}\s+){0,1}((log\s+(${LOG_LEVEL}\s+interval\s+${LOG_INTERVAL}|disable|default))\s+){0,1}(time-range\s+${TIME_RANGE}\s+){0,1}(${STATE}\s+){0,1}\(hitcnt=${HIT_COUNT}\)\s+(\(inactive\)\s+){0,1}${LINE_HASH}\s* -> Record
+  ^\s+access\-list\s+${ACL_NAME}\s+line\s+${LINE_NUM}\s+${TYPE}\s+${ACTION}\s+${ENTRY_PROTOCOL_ICMP}\s+(fqdn\s+${ENTRY_SRC_FQDN}|range\s+${ENTRY_SRC_RANGE_START}\s+${ENTRY_SRC_RANGE_END}|host\s+(${ENTRY_SRC_HOST}|${ENTRY_SRC_V6HOST})|${ENTRY_SRC_NETWORK}\s+${ENTRY_SRC_MASK}|${ENTRY_SRC_V6NETWORK}\/${ENTRY_SRC_V6MASK}|${ENTRY_SRC_ANY})\s+(\(${ENTRY_SRC_FQDN_STATE}\)\s+){0,1}(fqdn\s+${ENTRY_DST_FQDN}|range\s+${ENTRY_DST_RANGE_START}\s+${ENTRY_DST_RANGE_END}|host\s+(${ENTRY_DST_HOST}|${ENTRY_DST_V6HOST})|${ENTRY_DST_NETWORK}\s+${ENTRY_DST_MASK}|${ENTRY_DST_V6NETWORK}\/${ENTRY_DST_V6MASK}|${ENTRY_DST_ANY})\s+(\(${ENTRY_DST_FQDN_STATE}\)\s+){0,1}(${ENTRY_ICMP_TYPE}(\s+${ENTRY_ICMP_CODE}){0,1}\s+){0,1}(log\s+(${LOG_LEVEL}\s+interval\s+${LOG_INTERVAL}|disable|default)\s+){0,1}(time-range\s+${TIME_RANGE}\s+){0,1}(inactive){0,1}\s*(\(hitcnt=${ENTRY_HIT_COUNT}\)){0,1}\s*(\(${ENTRY_STATE}\)){0,1}\s+${ENTRY_HASH}\s* -> Record
+  ^\s+access\-list\s+${ACL_NAME}\s+line\s+${LINE_NUM}\s+${TYPE}\s+${ACTION}\s+(${ENTRY_PROTOCOL}\s+){0,1}(fqdn\s+${ENTRY_SRC_FQDN}|range\s+${ENTRY_SRC_RANGE_START}\s+${ENTRY_SRC_RANGE_END}|host\s+(${ENTRY_SRC_HOST}|${ENTRY_SRC_V6HOST})|${ENTRY_SRC_NETWORK}\s+${ENTRY_SRC_MASK}|${ENTRY_SRC_V6NETWORK}\/${ENTRY_SRC_V6MASK}|${ENTRY_SRC_ANY})\s+(\(${ENTRY_SRC_FQDN_STATE}\)\s+){0,1}((fqdn\s+${ENTRY_DST_FQDN}|range\s+${ENTRY_DST_RANGE_START}\s+${ENTRY_DST_RANGE_END}|host\s+(${ENTRY_DST_HOST}|${ENTRY_DST_V6HOST})|${ENTRY_DST_NETWORK}\s+${ENTRY_DST_MASK}|${ENTRY_DST_V6NETWORK}\/${ENTRY_DST_V6MASK}|${ENTRY_DST_ANY})\s+){0,1}(\(${ENTRY_DST_FQDN_STATE}\)\s+){0,1}((eq\s+${ENTRY_PORT}|lt\s+${ENTRY_PORT_LESS_THAN}|gt\s+${ENTRY_PORT_GREATER_THAN}|range\s+${ENTRY_PORT_RANGE_START}\s+${ENTRY_PORT_RANGE_END})\s+){0,1}(log\s+([a-z0-9]+\s+interval\s+\d+|disable|default)\s+){0,1}(time-range\s+${TIME_RANGE}\s+){0,1}(inactive){0,1}\s*(\(hitcnt=${ENTRY_HIT_COUNT}\)){0,1}\s*(\(${ENTRY_STATE}\)){0,1}\s+${ENTRY_HASH}\s* -> Record
   ^.* -> Error "Did not match any rules"
 
 EOF
```

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_asp_drop.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_asp_drop.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_asp_table_vpn-context_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_asp_table_vpn-context_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_bgp_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_cpu_usage_detailed.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_cpu_usage_detailed.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_crypto_ipsec_sa.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_crypto_ipsec_sa.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_failover.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_failover.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_interface.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_interface_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_interface_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_license_all.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_license_all.textfsm`

 * *Files 24% similar despite different names*

```diff
@@ -20,27 +20,39 @@
 Value AUTH_DEADLINE (.+?)
 Value LICENSE (\S.*?)
 Value LICENSE_PID (\S+?)
 Value LICENSE_DESCRIPTION (.+?)
 Value LICENSE_COUNT (\d+)
 Value LICENSE_VERSION (\S+)
 Value LICENSE_STATUS (.+?)
+Value LICENSE_EXPORT_STATUS (.+?)
 Value PID (.+?)
 Value SN (.+?)
 Value SMART_AGENT_VERSION (.+?)
+Value UTILITY_STATUS (.+?)
+Value PRIVACY_SENDING_HOSTNAME (.+?)
+Value PRIVACY_CALLHOME_HOSTNAME_PRIVACY (.+?)
+Value PRIVACY_SMART_LICENSING_HOSTNAME_PRIVACY (.+?)
+Value PRIVACY_VERSION_PRIVACY (.+?)
+Value TRANSPORT_TYPE (.+?)
+Value LICENSE_RESERVATION (.+?)
 
 Start
   ^\s*$$
   ^Smart\s+Licensing\s+Status
   ^Smart\s+Licensing\s+is\s+${SMART_STATUS}\s*$$
   ^Registration:\s*$$ -> REGISTRATION
   ^License\s+Authorization:\s*$$ -> AUTHORIZATION
   ^License\s+Usage\s*$$ -> LICENSE_USAGE
   ^Product\s+Information\s*$$ -> PRODUCT_INFORMATION
   ^Agent\s+Version\s*$$ -> AGENT_VERSION
+  ^Utility:\s*$$ -> UTILITY
+  ^Data\s+Privacy:\s*$$ -> PRIVACY
+  ^Transport:\s*$$ -> TRANSPORT
+  ^No\s+licenses\s+in\s+use\s*$$
   ^=+\s*$$
   ^. -> Error
 
 REGISTRATION
   ^\s*$$
   ^\s+Status:\s+${REGISTRATION_STATUS}\s*$$
   ^\s+Smart\s+Account:\s+${SMART_ACCOUNT}\s*$$
@@ -70,30 +82,34 @@
   ^\s+Communication\s+Deadline:\s+${AUTH_DEADLINE}\s*$$
   ^License\s+Usage\s*$$ -> LICENSE_USAGE
   ^Product\s+Information\s*$$ -> PRODUCT_INFORMATION
   ^Agent\s+Version\s*$$ -> AGENT_VERSION
   ^Smart\s+Licensing\s+is\s+${SMART_STATUS}\s*$$
   ^Registration:\s*$$ -> REGISTRATION
   ^License\s+Authorization:\s*$$ -> AUTHORIZATION
+  ^Utility:\s*$$ -> UTILITY
+  ^Export\s+Authorization\s+Key:\s*$$ -> EXPORT_AUTHORIZATION_KEY
   ^=+\s*$$
   ^. -> Error
 
 LICENSE_USAGE
   ^\s*$$
   ^${LICENSE}?\s*\(${LICENSE_PID}\):\s*$$
   ^\s+Description:(?:\s+${LICENSE_DESCRIPTION})?\s*$$
   ^\s+Count:\s+${LICENSE_COUNT}\s*$$
   ^\s+Version:\s+${LICENSE_VERSION}\s*$$
   ^\s+Status:\s+${LICENSE_STATUS}\s*$$
+  ^\s+Export\s+status:\s+${LICENSE_EXPORT_STATUS}\s*$$
   ^Product\s+Information\s*$$ -> PRODUCT_INFORMATION
   ^Agent\s+Version\s*$$ -> AGENT_VERSION
   ^Smart\s+Licensing\s+is\s+${SMART_STATUS}\s*$$
   ^Registration:\s*$$ -> REGISTRATION
   ^License\s+Authorization:\s*$$ -> AUTHORIZATION
   ^License\s+Usage\s*$$ -> LICENSE_USAGE
+  ^No\s+licenses\s+in\s+use\s*$$
   ^=+\s*$$
   ^. -> Error
 
 PRODUCT_INFORMATION
   ^\s*$$
   ^UDI:.*PID:${PID},\s*SN:${SN}\s*$$ -> Start
   ^Agent\s+Version\s*$$ -> AGENT_VERSION
@@ -110,9 +126,54 @@
   ^Smart\s+Agent\s+for\s+Licensing:\s+${SMART_AGENT_VERSION}\s*$$
   ^Smart\s+Licensing\s+is\s+${SMART_STATUS}\s*$$
   ^Registration:\s*$$ -> REGISTRATION
   ^License\s+Authorization:\s*$$ -> AUTHORIZATION
   ^License\s+Usage\s*$$ -> LICENSE_USAGE
   ^Product\s+Information\s*$$ -> PRODUCT_INFORMATION
   ^Agent\s+Version\s*$$ -> AGENT_VERSION
+  ^Reservation\s+Info\s*$$ -> RESERVATION_INFO
+  ^=+\s*$$
+  ^. -> Error
+
+RESERVATION_INFO
+  ^\s*$$
+  ^\s*License\s+reservation:\s+${LICENSE_RESERVATION}\s*$$
+  ^=+\s*$$
+  ^. -> Error
+
+UTILITY
+  ^\s*$$
+  ^\s+Status:\s+${UTILITY_STATUS}\s*$$
+  ^Data\s+Privacy:\s*$$ -> PRIVACY
+  ^=+\s*$$
+  ^. -> Error
+
+PRIVACY
+  ^\s*$$
+  ^\s+Sending\s+Hostname:\s+${PRIVACY_SENDING_HOSTNAME}\s*$$
+  ^\s+Callhome\s+hostname\s+privacy:\s+${PRIVACY_CALLHOME_HOSTNAME_PRIVACY}\s*$$
+  ^\s+Smart\s+Licensing\s+hostname\s+privacy:\s+${PRIVACY_SMART_LICENSING_HOSTNAME_PRIVACY}\s*$$
+  ^\s+Version\s+privacy:\s+${PRIVACY_VERSION_PRIVACY}\s*$$
+  ^Transport:\s*$$ -> TRANSPORT
+  ^=+\s*$$
+  ^. -> Error
+
+TRANSPORT
+  ^\s*$$
+  ^\s+Type:\s+${TRANSPORT_TYPE}\s*$$
+  ^License\s+Usage\s*$$ -> LICENSE_USAGE
+  ^=+\s*$$
+  ^. -> Error
+
+EXPORT_AUTHORIZATION_KEY
+  ^\s*$$
+  ^\s+Features\s+Authorized:\s*$$
+  ^\s+<none>\s*$$
+  ^License\s+Usage\s*$$ -> LICENSE_USAGE
+  ^Product\s+Information\s*$$ -> PRODUCT_INFORMATION
+  ^Agent\s+Version\s*$$ -> AGENT_VERSION
+  ^Smart\s+Licensing\s+is\s+${SMART_STATUS}\s*$$
+  ^Registration:\s*$$ -> REGISTRATION
+  ^License\s+Authorization:\s*$$ -> AUTHORIZATION
+  ^Utility:\s*$$ -> UTILITY
   ^=+\s*$$
   ^. -> Error
```

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_logging.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_logging.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_nat.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_nat.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_object-group_network.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_object-group_network.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_port-channel_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_port-channel_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_route.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_running-config_all_crypto_map.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_running-config_all_crypto_map.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_running-config_crypto_map.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_running-config_crypto_map.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_running-config_ipsec.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_running-config_ipsec.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_running-config_tunnel-group.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_running-config_tunnel-group.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_version.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_anyconnect.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_anyconnect.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_detail_l2l.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_vpn-sessiondb_detail_l2l.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_asa_show_xlate.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_asa_show_xlate.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_ping.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_ping.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_access-list.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_access-list.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_adjacency.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_adjacency.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ap_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ap_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_archive.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_archive.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_bfd_neighbors_details.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_bfd_neighbors_details.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_boot.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_boot.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_cdp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_controller_t1.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_controller_t1.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_crypto_ipsec_sa_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_crypto_ipsec_sa_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_crypto_pki_certificates.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_crypto_pki_certificates.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_crypto_session_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_crypto_session_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_dhcp_lease.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_dhcp_lease.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_dot1x_all.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_dot1x_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_environment_temperature.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_environment_temperature.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_etherchannel_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_etherchannel_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_interface_link.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_interface_link.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_interfaces.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_interfaces_status.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_interfaces_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_interfaces_switchport.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_interfaces_switchport.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_inventory.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_inventory.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_access-lists.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_access-lists.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_arp.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_arp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_bgp.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_bgp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors_advertised-routes.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_bgp_neighbors_advertised-routes.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_bgp_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_bgp_vpnv4_all_neighbors.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_bgp_vpnv4_all_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_cef.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_cef.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_cef_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_cef_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_device_tracking_all.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_device_tracking_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_interfaces_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_interfaces_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_neighbors.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_topology.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_eigrp_topology.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_http_server_status.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_http_server_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_interface.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_mroute.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_mroute.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_nat_translations.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_nat_translations.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_network.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_network.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_router.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_ospf_database_router.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_route.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_route_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_route_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ip_source_binding.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ip_source_binding.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ipv6_access-lists.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ipv6_access-lists.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_ipv6_route.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_ipv6_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_isdn_status.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_isdn_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_license.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_license.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_lldp_neighbors_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_lldp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_logging.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_logging.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_mac-address-table.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_mac-address-table.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_module.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_module.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_module_online_diag.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_module_online_diag.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_module_status.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_module_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_module_submodule.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_module_submodule.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_object-group.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_object-group.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_platform_diag.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_platform_diag.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_port-security_interface_interface.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_port-security_interface_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_power_available.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_power_available.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_power_status.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_power_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_processes_memory_sorted.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_processes_memory_sorted.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_redundancy.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_redundancy.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_route-map.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_route-map.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_running-config_partition_access-list.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_running-config_partition_access-list.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_running-config_partition_route-map.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_running-config_partition_route-map.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_snmp_group.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_snmp_group.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_snmp_user.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_snmp_user.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_standby.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_standby.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_standby_brief.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_standby_brief.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_tacacs.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_tacacs.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_version.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vlan.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vrf.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_vrf.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vrf_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_vrf_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vrrp_all.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_vrrp_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vrrp_brief.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_vrrp_brief.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_show_vtp_status.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_show_vtp_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_ios_traceroute.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_ios_traceroute.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_access-lists.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_access-lists.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_cdp_neighbors_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_cdp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_cts_interface_all.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_cts_interface_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_environment.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_environment.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_fex_id.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_fex_id.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_forwarding_adjacency.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_forwarding_adjacency.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_forwarding_ipv4_route.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_forwarding_ipv4_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_hsrp_all.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_hsrp_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interface.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interface_brief.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_interface_brief.textfsm`

 * *Files 0% similar despite different names*

```diff
@@ -57,7 +57,8 @@
   ^. -> Error PORTCHANNEL
 
 TUNNEL
   ^${INTERFACE}\s+${STATUS}\s+${IP}\s+${TYPE}\s+${MTU} -> Record
   ^---+$$
   ^\s*$$ -> Start
   ^. -> Error TUNNEL
+
```

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver_details.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_interface_transceiver_details.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_interfaces_switchport.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_interfaces_switchport.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_adjacency.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_adjacency.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_bgp.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_bgp.textfsm`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Path type: i-internal, e-external, c-confed, l-local, a-aggregate, r-redist, I-injected
 Value ROUTE_SOURCE ([ieclarI])
 Value Filldown NETWORK ([A-Fa-f0-9:\.]+\/\d+)
 Value NEXT_HOP ([A-Fa-f0-9:\.]+)
 Value METRIC (\d+)
 Value LOCAL_PREF (\d+)
 Value WEIGHT (\d+)
-Value AS_PATH (\d+(\s\d+)*)
+Value AS_PATH (\d+(\s.*?)*)
 # Origin codes: i - IGP, e - EGP, ? - incomplete, | - multipath, & - backup
 Value ORIGIN ([ie\?\|&])
 
 
 Start
   ^BGP\s+(routing|table)\s 
   ^Status:
```

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_neighbors.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary_vrf.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_bgp_summary_vrf.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_community-list.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_community-list.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_dhcp_snooping_statistics.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_dhcp_snooping_statistics.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_interface.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_interface_vrf_all.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_interface_vrf_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_msdp_summary_vrf_all.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_msdp_summary_vrf_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_database.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_database.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_interface_brief.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_ospf_interface_brief.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_pim_neighbor_vrf_all.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_pim_neighbor_vrf_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_pim_rp_vrf_all.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_pim_rp_vrf_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_ip_route.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_ip_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_lldp_neighbors_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_lldp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_port-channel_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_port-channel_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_route-map.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_route-map.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_version.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_nxos_show_vlan.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_nxos_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_s300_show_interfaces_status.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_s300_show_interfaces_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a_cleanair_config.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_802.11a_cleanair_config.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_advanced_802.11a_channel.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_advanced_802.11a_channel.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_config_general.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_config_general.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_image_all.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_ap_image_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_band-select.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_band-select.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_cdp_neighbors_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_cdp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_client_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_client_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_detailed_id.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_interface_detailed_id.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_mobility_sum.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_mobility_sum.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_port_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_port_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_radius_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_radius_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_redundancy_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_stats_port_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_stats_port_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_sysinfo.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_sysinfo.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_tacacs_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_tacacs_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_wlc_ssh_show_time.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_wlc_ssh_show_time.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_admin_show_controller_fabric_health.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_admin_show_controller_fabric_health.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_admin_show_environment_fan.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_admin_show_environment_fan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_arp.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_arp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_asic-errors_all_location.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_asic-errors_all_location.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_bgp.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_bgp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_bgp_instance_all_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_bgp_instance_all_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_bgp_neighbors.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_bgp_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_cdp_neighbors_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_cdp_neighbors_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_cef_drops_location.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_cef_drops_location.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_HundredGigabitEthernet.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_controllers_HundredGigabitEthernet.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_all_phy.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_controllers_all_phy.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_egress_location.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_egress_location.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_ingress_location.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_drops_ingress_location.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_errors_ingress_location.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_controllers_fabric_fia_errors_ingress_location.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_controllers_hundredgige_all.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_controllers_hundredgige_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_drops_np_all.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_drops_np_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_hsrp.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_hsrp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_install_active.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_install_active.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_interfaces.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ip_bgp_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_ip_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ip_route.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_ip_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_ipv4_interface.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_ipv4_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_lpts_pifib_hardware_police_location.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_lpts_pifib_hardware_police_location.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_platform_summary_location_all.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_platform_summary_location_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/cisco_xr_show_version.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/cisco_xr_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/dell_force10_show_vlan.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/dell_force10_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/dell_powerconnect_show_interfaces_status.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/dell_powerconnect_show_interfaces_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/ericsson_ipos_show_arp.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/ericsson_ipos_show_arp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_router_info_bgp_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/fortinet_get_router_info_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_system_ha_status.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/fortinet_get_system_ha_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_system_interface.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/fortinet_get_system_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_system_interface_physical.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/fortinet_get_system_interface_physical.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/fortinet_get_system_status.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/fortinet_get_system_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_counters_bound_interface.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_counters_bound_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_device_manuinfo.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_device_manuinfo.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_interface.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_ip_interface.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_ip_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_ip_routing-table.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_ip_routing-table.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_ip_vpn-instance_instance-name.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_ip_vpn-instance_instance-name.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_link-aggregation_verbose.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_link-aggregation_verbose.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_list.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_list.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_verbose.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_lldp_neighbor-information_verbose.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/hp_comware_display_vlan_all.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/hp_comware_display_vlan_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_interfaces.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/hp_procurve_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_interfaces_brief.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/hp_procurve_show_interfaces_brief.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device_detail.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/hp_procurve_show_lldp_info_remote-device_detail.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/hp_procurve_show_system.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/hp_procurve_show_system.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_acl_all.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_acl_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_arp_all.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_arp_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_interface.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_interface.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_ip_routing-table_verbose.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_ip_routing-table_verbose.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_ipv6_neighbors.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_ipv6_neighbors.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_lldp_neighbor.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_lldp_neighbor.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_nat_server.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_nat_server.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_port_vlan.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_port_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_service-set_id_id.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_service-set_id_id.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_startup.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_startup.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/huawei_vrp_display_traffic-filter_applied-record.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/huawei_vrp_display_traffic-filter_applied-record.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/index` & `ntc_templates-3.5.0/ntc_templates/templates/index`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 aruba_aoscx_show_ip_route_all-vrfs.textfsm, .*, aruba_aoscx, sh[[ow]] ip r[[oute]] a[[ll-vrfs]]
 aruba_aoscx_show_mac-address-table.textfsm, .*, aruba_aoscx, sh[[ow]] ma[[c-address-table]]
 aruba_aoscx_show_ntp_associations.textfsm, .*, aruba_aoscx, sh[[ow]] ntp as[[sociations]]
 aruba_aoscx_show_arp_all-vrfs.textfsm, .*, aruba_aoscx, sh[[ow]] ar[[p]] a[[ll-vrfs]]
 aruba_aoscx_show_bfd_all-vrfs.textfsm, .*, aruba_aoscx, sh[[ow]] bf[[d]] a[[ll-vrfs]]
 aruba_aoscx_show_vsf_detail.textfsm , .*, aruba_aoscx, sh[[ow]] vsf d[[etail]]
 aruba_aoscx_show_interface.textfsm , .*, aruba_aoscx, sh[[ow]] int[[erface]]
+aruba_aoscx_show_system.textfsm , .*, aruba_aoscx, sh[[ow]] sys[[tem]]
 
 aruba_os_show_ap_bss-table_details.textfsm, .*, aruba_os, show ap bss-table details
 aruba_os_show_ipv6_interface_brief.textfsm, .*, aruba_os, sh[[ow]] ipv6 in[[terface]] b[[rief]]
 aruba_os_show_ip_interface_brief.textfsm, .*, aruba_os, sh[[ow]] ip in[[terface]] b[[rief]]
 aruba_os_show_ap_radio-database.textfsm, .*, aruba_os, show ap radio-database
 aruba_os_show_ap_database_long.textfsm, .*, aruba_os, show ap database long
 aruba_os_show_ap_database.textfsm, .*, aruba_os, show ap database
@@ -593,14 +594,15 @@
 
 ubiquiti_edgerouter_show_interfaces_ethernet_physical.textfsm, .*, ubiquiti_edgerouter, sh[[ow]] interfaces ethernet (\S+\s)?physical
 ubiquiti_edgerouter_show_dhcpv6_server_leases.textfsm, .*, ubiquiti_edgerouter, sh[[ow]] dhcpv6 server leases
 ubiquiti_edgerouter_show_ipv6_neighbors.textfsm, .*, ubiquiti_edgerouter, sh[[ow]] ipv6 neighbors
 ubiquiti_edgerouter_show_dhcp_leases.textfsm, .*, ubiquiti_edgerouter, sh[[ow]] dhcp leases
 ubiquiti_edgerouter_show_interfaces.textfsm, .*, ubiquiti_edgerouter, show interfaces
 ubiquiti_edgerouter_show_ipv6_route.textfsm, .*, ubiquiti_edgerouter, show ipv6 route
+ubiquiti_edgerouter_show_nat_rules.textfsm, .*, ubiquiti_edgerouter, sh[[ow]] nat rules
 ubiquiti_edgerouter_show_ip_route.textfsm, .*, ubiquiti_edgerouter, show ip route
 ubiquiti_edgerouter_show_version.textfsm, .*, ubiquiti_edgerouter, sh[[ow]] ve[[rsion]]
 ubiquiti_edgerouter_show_arp.textfsm, .*, ubiquiti_edgerouter, sh[[ow]] arp
 
 ubiquiti_edgeswitch_show_version.textfsm, .*, ubiquiti_edgeswitch, sh[[ow]] ve[[rsion]]
 ubiquiti_edgeswitch_show_vlan.textfsm, .*, ubiquiti_edgeswitch, sh[[ow]] vl[[an]]
 ubiquiti_edgeswitch_show_arp.textfsm, .*, ubiquiti_edgeswitch, sh[[ow]] ar[[p]]
```

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/ipinfusion_ocnos_show_lldp_table.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/ipinfusion_ocnos_show_lldp_table.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_interfaces.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_status.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_chassis_cluster_status.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_chassis_hardware.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_chassis_hardware.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_ethernet-switching_table.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_ethernet-switching_table.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_interfaces.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_lacp_interfaces.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_lacp_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_system_uptime.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_system_uptime.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/juniper_junos_show_version.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/juniper_junos_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/juniper_screenos_get_route.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/juniper_screenos_get_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/linux_ip_address_show.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/linux_ip_address_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/linux_ip_link_show.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/linux_ip_link_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/linux_ip_route_show.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/linux_ip_route_show.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_interface_ethernet_monitor_name_once.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/mikrotik_routeros_interface_ethernet_monitor_name_once.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ip_dhcp-server_lease_print_without-paging.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/mikrotik_routeros_ip_dhcp-server_lease_print_without-paging.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_filter_print_all_without-paging.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_filter_print_all_without-paging.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_nat_print_all_without-paging.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/mikrotik_routeros_ip_firewall_nat_print_all_without-paging.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_ip_route_print_terse.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/mikrotik_routeros_ip_route_print_terse.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/mikrotik_routeros_system_routerboard_print.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/mikrotik_routeros_system_routerboard_print.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_high-availability_all.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/paloalto_panos_show_high-availability_all.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_interface_management.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/paloalto_panos_show_interface_management.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_running_nat-policy.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/paloalto_panos_show_running_nat-policy.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_running_security-policy.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/paloalto_panos_show_running_security-policy.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_show_system_info.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/paloalto_panos_show_system_info.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/paloalto_panos_test_security-policy-match.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/paloalto_panos_test_security-policy-match.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_arp.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/ruckus_fastiron_show_arp.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_interfaces.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/ruckus_fastiron_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_interfaces_brief.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/ruckus_fastiron_show_interfaces_brief.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_version.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/ruckus_fastiron_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/ruckus_fastiron_show_vlan.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/ruckus_fastiron_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgerouter_show_ip_route.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/ubiquiti_edgerouter_show_ip_route.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/ubiquiti_edgeswitch_show_version.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/ubiquiti_edgeswitch_show_version.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/vyatta_vyos_show_ip_bgp_summary.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/vyatta_vyos_show_ip_bgp_summary.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/yamaha_show_environment.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/yamaha_show_environment.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_firewall_acl_get.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_cfg_firewall_acl_get.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_ipalias_get.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_cfg_ipalias_get.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_lan_get_--Name_name.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_cfg_lan_get_--Name_name.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_nat_addr_map_get.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_cfg_nat_addr_map_get.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_nat_get.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_cfg_nat_get.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_snmp_get.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_cfg_snmp_get.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_static_route_get.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_cfg_static_route_get.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_cfg_wlan_get.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_cfg_wlan_get.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/ntc_templates/templates/zyxel_os_sys_atsh.textfsm` & `ntc_templates-3.5.0/ntc_templates/templates/zyxel_os_sys_atsh.textfsm`

 * *Files identical despite different names*

### Comparing `ntc_templates-3.4.0/pyproject.toml` & `ntc_templates-3.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ntc_templates"
-version = "v3.4.0"
+version = "v3.5.0"
 description = "TextFSM Templates for Network Devices, and Python wrapper for TextFSM's CliTable."
 authors = ["Network to Code <info@networktocode.com>"]
 license = "Apache-2.0"
 homepage = "https://ntc-templates.readthedocs.io"
 repository = "https://github.com/networktocode/ntc-templates"
 documentation = "https://ntc-templates.readthedocs.io"
 readme = "README.md"
```

### Comparing `ntc_templates-3.4.0/PKG-INFO` & `ntc_templates-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntc-templates
-Version: 3.4.0
+Version: 3.5.0
 Summary: TextFSM Templates for Network Devices, and Python wrapper for TextFSM's CliTable.
 Home-page: https://ntc-templates.readthedocs.io
 License: Apache-2.0
 Keywords: textfsm,network parsers
 Author: Network to Code
 Author-email: info@networktocode.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ntc-templates Version: 3.4.0 Summary: TextFSM
+Metadata-Version: 2.1 Name: ntc-templates Version: 3.5.0 Summary: TextFSM
 Templates for Network Devices, and Python wrapper for TextFSM's CliTable. Home-
 page: https://ntc-templates.readthedocs.io License: Apache-2.0 Keywords:
 textfsm,network parsers Author: Network to Code Author-email:
 info@networktocode.com Requires-Python: >=3.7,<4.0 Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
```

