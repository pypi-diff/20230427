# Comparing `tmp/netdoc-0.9.56.tar.gz` & `tmp/netdoc-0.9.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netdoc-0.9.56.tar", last modified: Tue Apr 25 14:22:47 2023, max compression
+gzip compressed data, was "netdoc-0.9.57.tar", last modified: Wed Apr 26 16:55:03 2023, max compression
```

## Comparing `netdoc-0.9.56.tar` & `netdoc-0.9.57.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.935201 netdoc-0.9.56/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.56/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      241 2023-04-05 08:40:22.000000 netdoc-0.9.56/MANIFEST.in
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      469 2023-04-25 14:22:47.935201 netdoc-0.9.56/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     9982 2023-04-24 17:00:01.000000 netdoc-0.9.56/README.md
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.839199 netdoc-0.9.56/netdoc/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2218 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/__init__.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.847200 netdoc-0.9.56/netdoc/api/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/api/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2812 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/api/serializers.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      597 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/api/urls.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1207 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/api/views.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.851199 netdoc-0.9.56/netdoc/discoverers/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/discoverers/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6978 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/discoverers/netmiko_cisco_ios.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5160 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/discoverers/netmiko_cisco_nxos.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6514 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/discoverers/netmiko_cisco_xr.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6406 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/discoverers/netmiko_hp_comware.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4511 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/discoverers/netmiko_linux.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3613 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/filtersets.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6587 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/forms.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.887200 netdoc-0.9.56/netdoc/ingestors/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1205 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3710 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2014 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2457 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1705 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      822 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1544 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1951 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2602 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3959 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1660 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      886 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1010 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1238 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3677 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2349 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1986 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      824 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1539 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2000 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2668 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3936 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1509 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2020 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      888 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      909 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1204 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1529 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_arp.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3673 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2347 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1802 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2921 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2709 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_route.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      980 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1562 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_arp.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      894 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2980 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1385 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2626 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1038 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1687 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2035 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2962 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3964 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1514 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      895 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      899 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1202 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1539 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_linux_arp__an.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1008 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_linux_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1412 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_linux_ip_address_show.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1933 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_linux_ip_link_show.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2450 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_linux_ip_route_show.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      711 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_linux_ip_vrf_show.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.891200 netdoc-0.9.56/netdoc/migrations/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    13632 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/migrations/0001_initial.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1800 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3399 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3022 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      577 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      453 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/migrations/0006_alter_routetableentry_metric.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      419 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/migrations/0007_discoverylog_supported.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/migrations/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    15079 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/models.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2436 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/navigation.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2988 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/nornir_inventory.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.891200 netdoc-0.9.56/netdoc/reports/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5880 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/reports/NetDoc.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.895200 netdoc-0.9.56/netdoc/schemas/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1937 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/arptableentry.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4549 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/cable.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1739 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/credential.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4374 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/device.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1508 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/devicerole.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1714 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/devicetype.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3905 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/discoverable.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3176 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/discoverylog.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8791 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1362 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/ipaddress.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1978 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/macaddresstableentry.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1453 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/manufacturer.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1986 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/prefix.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2904 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/routetableentry.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      884 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/site.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1623 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/vlan.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2476 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/vrf.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.895200 netdoc-0.9.56/netdoc/scripts/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    13085 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/scripts/NetDoc.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.831199 netdoc-0.9.56/netdoc/static/
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.831199 netdoc-0.9.56/netdoc/static/netdoc/
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.895200 netdoc-0.9.56/netdoc/static/netdoc/css/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/css/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/css/README.md
--rw-rw-r--   0 andrea    (1000) andrea    (1000)   220164 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/css/vis-network.min.css
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.907201 netdoc-0.9.56/netdoc/static/netdoc/img/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      305 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/README.md
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7415 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/access-switch.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5648 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/backup.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    28633 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/circuit.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8387 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/core-switch.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     9522 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/distribution-switch.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    15596 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/firewall.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1614 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/internal-switch.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5537 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/isp-cpe-material.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5079 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/non-racked-devices.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    15857 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/power-feed.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    18685 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/power-panel.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4710 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/power-units.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    34335 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/provider-networks.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    13504 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/router.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4484 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/server.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5648 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/storage.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8308 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/unknown.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7415 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/wan-network.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6975 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/wireless-ap.png
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.911201 netdoc-0.9.56/netdoc/static/netdoc/js/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/js/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/js/README.md
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4198 2023-04-05 14:32:29.000000 netdoc-0.9.56/netdoc/static/netdoc/js/diagram.js
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1739 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/js/netdoc.js
--rw-rw-r--   0 andrea    (1000) andrea    (1000)   702066 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/js/vis-network.min.js
--rw-rw-r--   0 andrea    (1000) andrea    (1000)  1930592 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/js/vis-network.min.js.map
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8198 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/tables.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3912 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/tasks.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.831199 netdoc-0.9.56/netdoc/templates/
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.927201 netdoc-0.9.56/netdoc/templates/netdoc/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3038 2023-04-10 16:21:20.000000 netdoc-0.9.56/netdoc/templates/netdoc/arptableentry.html
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.931201 netdoc-0.9.56/netdoc/templates/netdoc/buttons/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      451 2023-04-10 16:17:25.000000 netdoc-0.9.56/netdoc/templates/netdoc/buttons/discover.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      337 2023-04-10 16:17:25.000000 netdoc-0.9.56/netdoc/templates/netdoc/buttons/export.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1669 2023-04-10 16:21:17.000000 netdoc-0.9.56/netdoc/templates/netdoc/credential.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1439 2023-04-10 16:29:06.000000 netdoc-0.9.56/netdoc/templates/netdoc/diagram.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2654 2023-04-10 16:23:32.000000 netdoc-0.9.56/netdoc/templates/netdoc/discoverable.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1217 2023-04-10 16:26:08.000000 netdoc-0.9.56/netdoc/templates/netdoc/discoverable_bulk_discover.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      638 2023-04-10 16:26:30.000000 netdoc-0.9.56/netdoc/templates/netdoc/discoverable_discover.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1006 2023-04-10 16:23:40.000000 netdoc-0.9.56/netdoc/templates/netdoc/discoverable_list.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5123 2023-04-10 16:23:17.000000 netdoc-0.9.56/netdoc/templates/netdoc/discoverylog.html
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.931201 netdoc-0.9.56/netdoc/templates/netdoc/htmx/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1005 2023-04-10 16:17:25.000000 netdoc-0.9.56/netdoc/templates/netdoc/htmx/discover_form.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1025 2023-04-10 16:17:25.000000 netdoc-0.9.56/netdoc/templates/netdoc/htmx/logexport_form.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3046 2023-04-10 16:20:47.000000 netdoc-0.9.56/netdoc/templates/netdoc/macaddresstableentry.html
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.931201 netdoc-0.9.56/netdoc/templatetags/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/templatetags/__init__.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.931201 netdoc-0.9.56/netdoc/templatetags/__pycache__/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      148 2023-04-16 15:43:43.000000 netdoc-0.9.56/netdoc/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1048 2023-04-16 15:43:43.000000 netdoc-0.9.56/netdoc/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      890 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/templatetags/netdoc_buttons.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.935201 netdoc-0.9.56/netdoc/tests/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/tests/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    16779 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/tests/test.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    11155 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/topologies.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5128 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/urls.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    27006 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/utils.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    18389 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/views.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.843199 netdoc-0.9.56/netdoc.egg-info/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      469 2023-04-25 14:22:47.000000 netdoc-0.9.56/netdoc.egg-info/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6905 2023-04-25 14:22:47.000000 netdoc-0.9.56/netdoc.egg-info/SOURCES.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-04-25 14:22:47.000000 netdoc-0.9.56/netdoc.egg-info/dependency_links.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-04-05 14:49:45.000000 netdoc-0.9.56/netdoc.egg-info/not-zip-safe
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      132 2023-04-25 14:22:47.000000 netdoc-0.9.56/netdoc.egg-info/requires.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        7 2023-04-25 14:22:47.000000 netdoc-0.9.56/netdoc.egg-info/top_level.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      103 2023-04-25 14:22:47.935201 netdoc-0.9.56/setup.cfg
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1272 2023-04-25 14:22:45.000000 netdoc-0.9.56/setup.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.389942 netdoc-0.9.57/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.57/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      241 2023-04-05 08:40:22.000000 netdoc-0.9.57/MANIFEST.in
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      469 2023-04-26 16:55:03.401942 netdoc-0.9.57/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     9982 2023-04-24 17:00:01.000000 netdoc-0.9.57/README.md
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.197938 netdoc-0.9.57/netdoc/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2218 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/__init__.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.221939 netdoc-0.9.57/netdoc/api/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/api/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2812 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/api/serializers.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      597 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/api/urls.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1207 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/api/views.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.221939 netdoc-0.9.57/netdoc/discoverers/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/discoverers/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6978 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/discoverers/netmiko_cisco_ios.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5160 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/discoverers/netmiko_cisco_nxos.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6514 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/discoverers/netmiko_cisco_xr.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6406 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/discoverers/netmiko_hp_comware.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4511 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/discoverers/netmiko_linux.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3613 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/filtersets.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6587 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/forms.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.277940 netdoc-0.9.57/netdoc/ingestors/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1205 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3710 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2014 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2457 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1705 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      822 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1544 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1951 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2678 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3959 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1660 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      886 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1010 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1238 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3677 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2349 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1986 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      824 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1539 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2000 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2851 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3936 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1509 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2020 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      888 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      909 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1204 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_xr_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1529 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_xr_show_arp.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3673 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2347 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1802 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2921 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2785 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_xr_show_route.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      980 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1562 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_arp.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      894 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2980 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1385 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2702 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1038 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1687 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2035 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2962 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3964 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1514 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      895 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      899 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1202 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1539 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_linux_arp__an.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1008 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_linux_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1412 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_linux_ip_address_show.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1933 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_linux_ip_link_show.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2526 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_linux_ip_route_show.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      711 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/ingestors/netmiko_linux_ip_vrf_show.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.277940 netdoc-0.9.57/netdoc/migrations/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    13632 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/migrations/0001_initial.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1800 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3399 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3022 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      577 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      453 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/migrations/0006_alter_routetableentry_metric.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      419 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/migrations/0007_discoverylog_supported.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/migrations/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    15079 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/models.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2436 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/navigation.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2988 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/nornir_inventory.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.277940 netdoc-0.9.57/netdoc/reports/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5880 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/reports/NetDoc.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.281940 netdoc-0.9.57/netdoc/schemas/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/schemas/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1937 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/schemas/arptableentry.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4532 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/schemas/cable.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1739 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/schemas/credential.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4374 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/schemas/device.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1508 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/schemas/devicerole.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1714 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/schemas/devicetype.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3905 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/schemas/discoverable.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3176 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/schemas/discoverylog.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8843 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/schemas/interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1362 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/schemas/ipaddress.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1978 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/schemas/macaddresstableentry.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1453 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/schemas/manufacturer.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2015 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/schemas/prefix.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3018 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/schemas/routetableentry.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      884 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/schemas/site.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1623 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/schemas/vlan.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2476 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/schemas/vrf.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.281940 netdoc-0.9.57/netdoc/scripts/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    13085 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/scripts/NetDoc.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.177938 netdoc-0.9.57/netdoc/static/
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.177938 netdoc-0.9.57/netdoc/static/netdoc/
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.281940 netdoc-0.9.57/netdoc/static/netdoc/css/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/css/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/css/README.md
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)   220164 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/css/vis-network.min.css
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.373942 netdoc-0.9.57/netdoc/static/netdoc/img/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/img/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      305 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/img/README.md
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7415 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/img/access-switch.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5648 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/img/backup.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    28633 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/img/circuit.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8387 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/img/core-switch.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     9522 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/img/distribution-switch.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    15596 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/img/firewall.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1614 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/img/internal-switch.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5537 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/img/isp-cpe-material.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5079 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/img/non-racked-devices.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    15857 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/img/power-feed.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    18685 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/img/power-panel.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4710 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/img/power-units.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    34335 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/img/provider-networks.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    13504 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/img/router.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4484 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/img/server.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5648 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/img/storage.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8308 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/img/unknown.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7415 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/img/wan-network.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6975 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/img/wireless-ap.png
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.373942 netdoc-0.9.57/netdoc/static/netdoc/js/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/js/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/js/README.md
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4198 2023-04-05 14:32:29.000000 netdoc-0.9.57/netdoc/static/netdoc/js/diagram.js
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1739 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/js/netdoc.js
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)   702066 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/js/vis-network.min.js
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)  1930592 2023-04-05 08:40:22.000000 netdoc-0.9.57/netdoc/static/netdoc/js/vis-network.min.js.map
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8272 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/tables.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3912 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/tasks.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.177938 netdoc-0.9.57/netdoc/templates/
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.389942 netdoc-0.9.57/netdoc/templates/netdoc/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3038 2023-04-10 16:21:20.000000 netdoc-0.9.57/netdoc/templates/netdoc/arptableentry.html
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.389942 netdoc-0.9.57/netdoc/templates/netdoc/buttons/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      451 2023-04-10 16:17:25.000000 netdoc-0.9.57/netdoc/templates/netdoc/buttons/discover.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      337 2023-04-10 16:17:25.000000 netdoc-0.9.57/netdoc/templates/netdoc/buttons/export.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1669 2023-04-10 16:21:17.000000 netdoc-0.9.57/netdoc/templates/netdoc/credential.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1439 2023-04-10 16:29:06.000000 netdoc-0.9.57/netdoc/templates/netdoc/diagram.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2654 2023-04-10 16:23:32.000000 netdoc-0.9.57/netdoc/templates/netdoc/discoverable.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1217 2023-04-10 16:26:08.000000 netdoc-0.9.57/netdoc/templates/netdoc/discoverable_bulk_discover.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      638 2023-04-10 16:26:30.000000 netdoc-0.9.57/netdoc/templates/netdoc/discoverable_discover.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1006 2023-04-10 16:23:40.000000 netdoc-0.9.57/netdoc/templates/netdoc/discoverable_list.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5123 2023-04-10 16:23:17.000000 netdoc-0.9.57/netdoc/templates/netdoc/discoverylog.html
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.389942 netdoc-0.9.57/netdoc/templates/netdoc/htmx/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1005 2023-04-10 16:17:25.000000 netdoc-0.9.57/netdoc/templates/netdoc/htmx/discover_form.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1025 2023-04-10 16:17:25.000000 netdoc-0.9.57/netdoc/templates/netdoc/htmx/logexport_form.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3046 2023-04-10 16:20:47.000000 netdoc-0.9.57/netdoc/templates/netdoc/macaddresstableentry.html
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.389942 netdoc-0.9.57/netdoc/templatetags/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/templatetags/__init__.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.389942 netdoc-0.9.57/netdoc/templatetags/__pycache__/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      148 2023-04-25 14:22:52.000000 netdoc-0.9.57/netdoc/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1048 2023-04-25 14:22:52.000000 netdoc-0.9.57/netdoc/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      890 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/templatetags/netdoc_buttons.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.389942 netdoc-0.9.57/netdoc/tests/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/tests/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    17018 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/tests/test.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    11155 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/topologies.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5128 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/urls.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    28063 2023-04-26 16:55:00.000000 netdoc-0.9.57/netdoc/utils.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    18389 2023-04-26 16:54:59.000000 netdoc-0.9.57/netdoc/views.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-26 16:55:03.217939 netdoc-0.9.57/netdoc.egg-info/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      469 2023-04-26 16:55:02.000000 netdoc-0.9.57/netdoc.egg-info/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6905 2023-04-26 16:55:02.000000 netdoc-0.9.57/netdoc.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-04-26 16:55:02.000000 netdoc-0.9.57/netdoc.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-04-05 14:49:45.000000 netdoc-0.9.57/netdoc.egg-info/not-zip-safe
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      132 2023-04-26 16:55:02.000000 netdoc-0.9.57/netdoc.egg-info/requires.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        7 2023-04-26 16:55:02.000000 netdoc-0.9.57/netdoc.egg-info/top_level.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      103 2023-04-26 16:55:03.405942 netdoc-0.9.57/setup.cfg
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1272 2023-04-26 16:55:00.000000 netdoc-0.9.57/setup.py
```

### Comparing `netdoc-0.9.56/LICENSE` & `netdoc-0.9.57/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/README.md` & `netdoc-0.9.57/README.md`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/__init__.py` & `netdoc-0.9.57/netdoc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Main class."""
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
-__version__ = "0.9.56"
+__version__ = "0.9.57"
 
 import os
 import pkgutil
 import shutil
 
 from django.conf import settings
```

### Comparing `netdoc-0.9.56/netdoc/api/serializers.py` & `netdoc-0.9.57/netdoc/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/api/urls.py` & `netdoc-0.9.57/netdoc/api/urls.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/api/views.py` & `netdoc-0.9.57/netdoc/api/views.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/discoverers/netmiko_cisco_ios.py` & `netdoc-0.9.57/netdoc/discoverers/netmiko_cisco_ios.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/discoverers/netmiko_cisco_nxos.py` & `netdoc-0.9.57/netdoc/discoverers/netmiko_cisco_nxos.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/discoverers/netmiko_cisco_xr.py` & `netdoc-0.9.57/netdoc/discoverers/netmiko_cisco_xr.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/discoverers/netmiko_hp_comware.py` & `netdoc-0.9.57/netdoc/discoverers/netmiko_hp_comware.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/discoverers/netmiko_linux.py` & `netdoc-0.9.57/netdoc/discoverers/netmiko_linux.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/filtersets.py` & `netdoc-0.9.57/netdoc/filtersets.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/forms.py` & `netdoc-0.9.57/netdoc/forms.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_hostname.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,16 @@
         # Get or create route table entry
         routetableentry_o = routetableentry.get(
             device_id=device_o.id,
             destination=destination,
             distance=distance,
             metric=metric,
             protocol=protocol,
+            nexthop_if_id=nexthop_if_id,
+            nexthop_ip=nexthop_ip,
         )
         if not routetableentry_o:
             data = {
                 "device_id": device_o.id,
                 "destination": destination,
                 "distance": distance,
                 "metric": metric,
```

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_hostname.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,41 @@
-"""Ingestor for netmiko_cisco_ios_show_ip_arp."""
+"""Ingestor for netmiko_hp_comware_display_ip_routing_table."""
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
 
 from netdoc.schemas import interface, vrf, routetableentry
 from netdoc import utils
 
 
 def ingest(log):
     """Processing parsed output."""
     device_o = log.discoverable.device
+    vrf_name = log.details.get("vrf")
+
+    # Get or create VRF
+    vrf_o = None
+    if vrf_name:
+        vrf_o = vrf.get(name=vrf_name)
+        if not vrf_o:
+            data = {
+                "name": vrf_name,
+            }
+            vrf_o = vrf.create(**data)
 
     for item in log.parsed_output:
-        # See https://github.com/networktocode/ntc-templates/tree/master/tests/cisco_nxos/show_ip_route # pylint: disable=line-too-long
+        # See https://github.com/networktocode/ntc-templates/tree/master/tests/hp_comware/display_ip_routing-table # pylint: disable=line-too-long
         nexthop_if_name = item.get("nexthop_if")
-        vrf_name = log.details.get("vrf")
-
         distance = int(item.get("distance")) if item.get("distance") else None
         metric = int(item.get("metric")) if item.get("metric") else None
         destination = (
             f"{item.get('network')}/{item.get('mask')}" if item.get("network") else None
         )
-        protocol = utils.normalize_route_type(item.get("protocol"))
+        protocol = utils.normalize_route_type(item.get("protocal"))
         nexthop_ip = item.get("nexthop_ip") if item.get("nexthop_ip") else None
 
         # Get or create interface
         nexthop_if_id = None
         if nexthop_if_name:
             nexthop_if_label = utils.normalize_interface_label(nexthop_if_name)
             nexthop_if_o = interface.get(device_id=device_o.id, label=nexthop_if_label)
@@ -34,31 +43,23 @@
                 interface_data = {
                     "name": nexthop_if_label,
                     "device_id": device_o.id,
                 }
                 nexthop_if_o = interface.create(**interface_data)
             nexthop_if_id = nexthop_if_o.id
 
-        # Get or create VRF
-        vrf_o = None
-        if vrf_name and vrf_name != "default":
-            vrf_o = vrf.get(name=vrf_name)
-            if not vrf_o:
-                data = {
-                    "name": vrf_name,
-                }
-                vrf_o = vrf.create(**data)
-
         # Get or create route table entry
         routetableentry_o = routetableentry.get(
             device_id=device_o.id,
             destination=destination,
             distance=distance,
             metric=metric,
             protocol=protocol,
+            nexthop_if_id=nexthop_if_id,
+            nexthop_ip=nexthop_ip,
         )
         if not routetableentry_o:
             data = {
                 "device_id": device_o.id,
                 "destination": destination,
                 "distance": distance,
                 "metric": metric,
```

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_hostname.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_xr_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_arp.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_xr_show_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_route.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_xr_show_route.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,14 +54,16 @@
         # Get or create route table entry
         routetableentry_o = routetableentry.get(
             device_id=device_o.id,
             destination=destination,
             distance=distance,
             metric=metric,
             protocol=protocol,
+            nexthop_if_id=nexthop_if_id,
+            nexthop_ip=nexthop_ip,
         )
         if not routetableentry_o:
             data = {
                 "device_id": device_o.id,
                 "destination": destination,
                 "distance": distance,
                 "metric": metric,
```

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_arp.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_interface.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,69 @@
-"""Ingestor for netmiko_hp_comware_display_ip_routing_table."""
+"""Ingestor for netmiko_cisco_ios_show_ip_arp."""
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
 
 from netdoc.schemas import interface, vrf, routetableentry
 from netdoc import utils
 
 
 def ingest(log):
     """Processing parsed output."""
     device_o = log.discoverable.device
-    vrf_name = log.details.get("vrf")
-
-    # Get or create VRF
-    vrf_o = None
-    if vrf_name:
-        vrf_o = vrf.get(name=vrf_name)
-        if not vrf_o:
-            data = {
-                "name": vrf_name,
-            }
-            vrf_o = vrf.create(**data)
 
     for item in log.parsed_output:
-        # See https://github.com/networktocode/ntc-templates/tree/master/tests/hp_comware/display_ip_routing-table # pylint: disable=line-too-long
+        # See https://github.com/networktocode/ntc-templates/tree/master/tests/cisco_nxos/show_ip_route # pylint: disable=line-too-long
         nexthop_if_name = item.get("nexthop_if")
+        vrf_name = item.get("vrf")
+
         distance = int(item.get("distance")) if item.get("distance") else None
         metric = int(item.get("metric")) if item.get("metric") else None
         destination = (
             f"{item.get('network')}/{item.get('mask')}" if item.get("network") else None
         )
-        protocol = utils.normalize_route_type(item.get("protocal"))
+        protocol = item.get("protocol")
+        if item.get("type"):
+            protocol = protocol + " " + item.get("type")
         nexthop_ip = item.get("nexthop_ip") if item.get("nexthop_ip") else None
+        protocol = utils.normalize_route_type(protocol)
 
         # Get or create interface
         nexthop_if_id = None
         if nexthop_if_name:
             nexthop_if_label = utils.normalize_interface_label(nexthop_if_name)
             nexthop_if_o = interface.get(device_id=device_o.id, label=nexthop_if_label)
             if not nexthop_if_o:
                 interface_data = {
                     "name": nexthop_if_label,
                     "device_id": device_o.id,
                 }
                 nexthop_if_o = interface.create(**interface_data)
             nexthop_if_id = nexthop_if_o.id
 
+        # Get or create VRF
+        vrf_o = None
+        if vrf_name and vrf_name != "default":
+            vrf_o = vrf.get(name=vrf_name)
+            if not vrf_o:
+                data = {
+                    "name": vrf_name,
+                }
+                vrf_o = vrf.create(**data)
+
         # Get or create route table entry
         routetableentry_o = routetableentry.get(
             device_id=device_o.id,
             destination=destination,
             distance=distance,
             metric=metric,
             protocol=protocol,
+            nexthop_if_id=nexthop_if_id,
+            nexthop_ip=nexthop_ip,
         )
         if not routetableentry_o:
             data = {
                 "device_id": device_o.id,
                 "destination": destination,
                 "distance": distance,
                 "metric": metric,
```

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_hostname.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_hp_comware_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_linux_arp__an.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_linux_arp__an.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_linux_hostname.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_linux_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_linux_ip_address_show.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_linux_ip_address_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_linux_ip_link_show.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_linux_ip_link_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_linux_ip_route_show.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_linux_ip_route_show.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 
         # Get or create route table entry
         routetableentry_o = routetableentry.get(
             device_id=device_o.id,
             destination=destination,
             metric=metric,
             protocol=protocol,
+            nexthop_if_id=nexthop_if_id,
+            nexthop_ip=nexthop_ip,
         )
         if not routetableentry_o:
             data = {
                 "device_id": device_o.id,
                 "destination": destination,
                 "metric": metric,
                 "protocol": protocol,
```

### Comparing `netdoc-0.9.56/netdoc/ingestors/netmiko_linux_ip_vrf_show.py` & `netdoc-0.9.57/netdoc/ingestors/netmiko_linux_ip_vrf_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/migrations/0001_initial.py` & `netdoc-0.9.57/netdoc/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py` & `netdoc-0.9.57/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py` & `netdoc-0.9.57/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py` & `netdoc-0.9.57/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py` & `netdoc-0.9.57/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/models.py` & `netdoc-0.9.57/netdoc/models.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/navigation.py` & `netdoc-0.9.57/netdoc/navigation.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/nornir_inventory.py` & `netdoc-0.9.57/netdoc/nornir_inventory.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/reports/NetDoc.py` & `netdoc-0.9.57/netdoc/reports/NetDoc.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/schemas/arptableentry.py` & `netdoc-0.9.57/netdoc/schemas/arptableentry.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/schemas/cable.py` & `netdoc-0.9.57/netdoc/schemas/cable.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,14 @@
             # L2 connections with multiple devices (do we have a hub or a CDP/LLDP
             # forwarding device?)
             if PLUGIN_SETTINGS.get(f"RAISE_ON_{protocol}_FAIL"):
                 raise IntegrityError(
                     f"Multiple neighbors on {left_interface_o.device}:{left_interface_o}"
                     + f" or {right_interface_o.device}:{right_interface_o}"
                 ) from exc
-            pass
 
 
 def unlink(**kwargs):
     """Unlink two Interface objects."""
     validate(kwargs, get_schema_create(), format_checker=FormatChecker())
 
     # Sort interfaces
```

### Comparing `netdoc-0.9.56/netdoc/schemas/credential.py` & `netdoc-0.9.57/netdoc/schemas/credential.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/schemas/device.py` & `netdoc-0.9.57/netdoc/schemas/device.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/schemas/devicerole.py` & `netdoc-0.9.57/netdoc/schemas/devicerole.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/schemas/devicetype.py` & `netdoc-0.9.57/netdoc/schemas/devicetype.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/schemas/discoverable.py` & `netdoc-0.9.57/netdoc/schemas/discoverable.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/schemas/discoverylog.py` & `netdoc-0.9.57/netdoc/schemas/discoverylog.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/schemas/interface.py` & `netdoc-0.9.57/netdoc/schemas/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         "name",
         "type",
         "device_id",
     ]
     return schema
 
 
-def create(type="other", **kwargs):
+def create(type="other", **kwargs):  # pylint: disable=redefined-builtin
     """Create an Interface."""
     # The following are updated in update_mode
     if "mode" in kwargs:
         del kwargs["mode"]
     if "untagged_vlan_id" in kwargs:
         del kwargs["untagged_vlan_id"]
     if "tagged_vlan_ids" in kwargs:
@@ -246,15 +246,15 @@
     vrf_id = obj.vrf.id if obj.vrf else None
 
     for ip_address in ip_addresses:
         if not ip_address:
             # Skip empty IP addresses
             continue
         # Get or create Prefix
-        prefix_o = prefix.get(prefix=ip_address)
+        prefix_o = prefix.get(prefix=ip_address, vrf_id=vrf_id)
         if not prefix_o:
             prefix.create(prefix=ip_address, vrf_id=vrf_id, site_id=site_id)
 
         if ip_address not in previous_ip_addresses:
             # Get or create IPAddress
             ip_address_list = ipaddress.get_list(address=ip_address, vrf_id=vrf_id)
             if ip_address_list:
```

### Comparing `netdoc-0.9.56/netdoc/schemas/ipaddress.py` & `netdoc-0.9.57/netdoc/schemas/ipaddress.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/schemas/macaddresstableentry.py` & `netdoc-0.9.57/netdoc/schemas/macaddresstableentry.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/schemas/manufacturer.py` & `netdoc-0.9.57/netdoc/schemas/manufacturer.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/schemas/prefix.py` & `netdoc-0.9.57/netdoc/schemas/prefix.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,12 +64,12 @@
     }
     data = utils.delete_empty_keys(data)
     validate(data, get_schema_create(), format_checker=FormatChecker())
     obj = utils.object_create(Prefix, **data)
     return obj
 
 
-def get(prefix):
+def get(prefix, vrf_id=None):
     """Return an Prefix."""
     prefix = address_to_network(prefix)
-    obj = utils.object_get_or_none(Prefix, prefix=prefix)
+    obj = utils.object_get_or_none(Prefix, prefix=prefix, vrf__id=vrf_id)
     return obj
```

### Comparing `netdoc-0.9.56/netdoc/schemas/routetableentry.py` & `netdoc-0.9.57/netdoc/schemas/routetableentry.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,23 +76,27 @@
 def get(
     device_id=None,
     destination=None,
     distance=None,
     metric=None,
     protocol=None,
     discovered=True,
+    nexthop_if_id=None,
+    nexthop_ip=None,
 ):
     """Return an RouteTableEntry."""
     obj = utils.object_get_or_none(
         RouteTableEntry,
         device_id=device_id,
         destination=destination,
         distance=distance,
         metric=metric,
         protocol=protocol,
+        nexthop_if__id=nexthop_if_id,
+        nexthop_ip=nexthop_ip,
     )
     if obj and discovered:
         # Update updated_at
         obj.save()
     return obj
```

### Comparing `netdoc-0.9.56/netdoc/schemas/site.py` & `netdoc-0.9.57/netdoc/schemas/site.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/schemas/vlan.py` & `netdoc-0.9.57/netdoc/schemas/vlan.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/schemas/vrf.py` & `netdoc-0.9.57/netdoc/schemas/vrf.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/scripts/NetDoc.py` & `netdoc-0.9.57/netdoc/scripts/NetDoc.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/css/LICENSE` & `netdoc-0.9.57/netdoc/static/netdoc/css/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/css/vis-network.min.css` & `netdoc-0.9.57/netdoc/static/netdoc/css/vis-network.min.css`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/img/LICENSE` & `netdoc-0.9.57/netdoc/static/netdoc/img/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/img/access-switch.png` & `netdoc-0.9.57/netdoc/static/netdoc/img/access-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/img/backup.png` & `netdoc-0.9.57/netdoc/static/netdoc/img/backup.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/img/circuit.png` & `netdoc-0.9.57/netdoc/static/netdoc/img/circuit.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/img/core-switch.png` & `netdoc-0.9.57/netdoc/static/netdoc/img/core-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/img/distribution-switch.png` & `netdoc-0.9.57/netdoc/static/netdoc/img/distribution-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/img/firewall.png` & `netdoc-0.9.57/netdoc/static/netdoc/img/firewall.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/img/internal-switch.png` & `netdoc-0.9.57/netdoc/static/netdoc/img/internal-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/img/isp-cpe-material.png` & `netdoc-0.9.57/netdoc/static/netdoc/img/isp-cpe-material.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/img/non-racked-devices.png` & `netdoc-0.9.57/netdoc/static/netdoc/img/non-racked-devices.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/img/power-feed.png` & `netdoc-0.9.57/netdoc/static/netdoc/img/power-feed.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/img/power-panel.png` & `netdoc-0.9.57/netdoc/static/netdoc/img/power-panel.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/img/power-units.png` & `netdoc-0.9.57/netdoc/static/netdoc/img/power-units.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/img/provider-networks.png` & `netdoc-0.9.57/netdoc/static/netdoc/img/provider-networks.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/img/router.png` & `netdoc-0.9.57/netdoc/static/netdoc/img/router.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/img/server.png` & `netdoc-0.9.57/netdoc/static/netdoc/img/server.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/img/storage.png` & `netdoc-0.9.57/netdoc/static/netdoc/img/storage.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/img/unknown.png` & `netdoc-0.9.57/netdoc/static/netdoc/img/unknown.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/img/wan-network.png` & `netdoc-0.9.57/netdoc/static/netdoc/img/wan-network.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/img/wireless-ap.png` & `netdoc-0.9.57/netdoc/static/netdoc/img/wireless-ap.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/js/LICENSE` & `netdoc-0.9.57/netdoc/static/netdoc/js/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/js/diagram.js` & `netdoc-0.9.57/netdoc/static/netdoc/js/diagram.js`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/js/netdoc.js` & `netdoc-0.9.57/netdoc/static/netdoc/js/netdoc.js`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/js/vis-network.min.js` & `netdoc-0.9.57/netdoc/static/netdoc/js/vis-network.min.js`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/static/netdoc/js/vis-network.min.js.map` & `netdoc-0.9.57/netdoc/static/netdoc/js/vis-network.min.js.map`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/tables.py` & `netdoc-0.9.57/netdoc/tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,14 +298,15 @@
     device = tables.LinkColumn(
         "dcim:device",
         args=[tables.utils.A("device__pk")],
     )
     nexthop_if = tables.LinkColumn(
         "dcim:interface", args=[tables.utils.A("nexthop_if__pk")]
     )
+    vrf = tables.LinkColumn("ipam:vrf", args=[tables.utils.A("vrf__pk")])
     device_role = tables.Column(accessor="device.device_role")
     actions = []  # Read only table
 
     class Meta(NetBoxTable.Meta):
         """Table metadata."""
 
         model = models.RouteTableEntry
```

### Comparing `netdoc-0.9.56/netdoc/tasks.py` & `netdoc-0.9.57/netdoc/tasks.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/templates/netdoc/arptableentry.html` & `netdoc-0.9.57/netdoc/templates/netdoc/arptableentry.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/templates/netdoc/credential.html` & `netdoc-0.9.57/netdoc/templates/netdoc/credential.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/templates/netdoc/diagram.html` & `netdoc-0.9.57/netdoc/templates/netdoc/diagram.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/templates/netdoc/discoverable.html` & `netdoc-0.9.57/netdoc/templates/netdoc/discoverable.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/templates/netdoc/discoverable_bulk_discover.html` & `netdoc-0.9.57/netdoc/templates/netdoc/discoverable_bulk_discover.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/templates/netdoc/discoverable_discover.html` & `netdoc-0.9.57/netdoc/templates/netdoc/discoverable_discover.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/templates/netdoc/discoverable_list.html` & `netdoc-0.9.57/netdoc/templates/netdoc/discoverable_list.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/templates/netdoc/discoverylog.html` & `netdoc-0.9.57/netdoc/templates/netdoc/discoverylog.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/templates/netdoc/htmx/discover_form.html` & `netdoc-0.9.57/netdoc/templates/netdoc/htmx/discover_form.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/templates/netdoc/htmx/logexport_form.html` & `netdoc-0.9.57/netdoc/templates/netdoc/htmx/logexport_form.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/templates/netdoc/macaddresstableentry.html` & `netdoc-0.9.57/netdoc/templates/netdoc/macaddresstableentry.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc` & `netdoc-0.9.57/netdoc/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 18:43:34 2023 UTC, .py size: 890 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 564d 3864 7a03 0000  o.......VM8dz...
+00000000: 6f0d 0d0a 0000 0000 34e2 4764 7a03 0000  o.......4.Gdz...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 6406 6c05 6d06 5a06 0100 6405  Z.d.d.l.m.Z...d.
 00000050: 6407 6c07 6d08 5a08 0100 6405 6408 6c09  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0a 0100 6506 a00b a100 5a0c 650c  m.Z...e.....Z.e.
 00000070: a00d 6409 a101 640a 640b 8400 8301 5a0e  ..d...d.d.....Z.
```

### Comparing `netdoc-0.9.56/netdoc/templatetags/netdoc_buttons.py` & `netdoc-0.9.57/netdoc/templatetags/netdoc_buttons.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/tests/test.py` & `netdoc-0.9.57/netdoc/tests/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,30 +206,39 @@
     """Test IPAddress given an expected_results dict."""
     # Test total IPAddress objects
     ipaddress_qs = IPAddress.objects.all()
     test_o.assertEquals(len(ipaddress_qs), len(expected_results))
 
     # Test each item
     for expected_result in expected_results:
-        ipaddress_o = IPAddress.objects.get(address=expected_result.get("address"))
-        if ipaddress_o.vrf:
-            test_o.assertEquals(ipaddress_o.vrf.name, expected_result.get("vrf"))
+        if expected_result.get("vrf"):
+            IPAddress.objects.get(
+                address=expected_result.get("address"),
+                vrf__name=expected_result.get("vrf"),
+            )
         else:
-            test_o.assertIs(expected_result.get("vrf"), None)
+            IPAddress.objects.get(address=expected_result.get("address"))
 
 
 def test_prefixes(test_o, expected_results):
     """Test Prefix given an expected_results dict."""
     # Test total Prefix objects
     prefix_qs = Prefix.objects.all()
     test_o.assertEquals(len(prefix_qs), len(expected_results))
 
     # Test each item
     for expected_result in expected_results:
-        prefix_o = Prefix.objects.get(prefix=expected_result.get("prefix"))
+        if expected_result.get("vrf"):
+            prefix_o = Prefix.objects.get(
+                prefix=expected_result.get("prefix"),
+                vrf__name=expected_result.get("vrf"),
+            )
+        else:
+            prefix_o = Prefix.objects.get(prefix=expected_result.get("prefix"))
+
         if prefix_o.vrf:
             test_o.assertEquals(prefix_o.vrf.name, expected_result.get("vrf"))
         else:
             test_o.assertIs(expected_result.get("vrf"), None)
 
         if prefix_o.site:
             test_o.assertEquals(prefix_o.site.name, expected_result.get("site"))
```

### Comparing `netdoc-0.9.56/netdoc/topologies.py` & `netdoc-0.9.57/netdoc/topologies.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/urls.py` & `netdoc-0.9.57/netdoc/urls.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc/utils.py` & `netdoc-0.9.57/netdoc/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """Useful functions."""
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
 
+from os import path
 import re
 import random
 import importlib
 import ipaddress
 import string
 import json
 import uuid
+from difflib import get_close_matches
 import macaddress
+import yaml
+from yaml.loader import SafeLoader
 
 from nornir_netmiko.tasks import netmiko_send_command
 from netmiko.utilities import get_structured_data
 from textfsm.parser import TextFSMError
 
 from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
@@ -295,14 +299,40 @@
         # Give prevedence to port_id
         return normalize_interface_label(port_id)
 
     # Use port_description as last resort
     return normalize_interface_label(port_description)
 
 
+def find_model(manufacturer=None, keyword=None):
+    """
+    Get most similar DeviceType (model) using Netbox devicetype-library.
+
+    See: https://github.com/netbox-community/devicetype-library
+    """
+    netdoc_directory = path.dirname(path.realpath(__file__))
+    library_file = f"{netdoc_directory}/library/{manufacturer}.yml"
+
+    with open(library_file, "r", encoding="utf-8") as vendor_fh:
+        # Load library file based on manufacturer
+        data = yaml.load(vendor_fh, Loader=SafeLoader)
+
+    # Find closest words (part number/model)
+    closests = get_close_matches(keyword, possibilities=data.get("keywords"), n=1)
+    if closests:
+        # Found something
+        closest = closests.pop()
+        for item in data.get("models"):
+            # Looking for the model based on closest word
+            if item.get("model") == closest or item.get("part_number") == closest:
+                return item
+
+    return None
+
+
 def incomplete_mac(mac):
     """Return True if the MAC address is incomplete (from ARP table)."""
     if not mac:
         return True
     if "incomplete" in mac.lower():
         return True
     return False
@@ -599,15 +629,15 @@
         return "b"
     if route_type in ["d"]:
         # EIGRP
         return "e"
     if route_type in ["ex"]:
         # EIGRP External
         return "ex"
-    if route_type in ["o", "ospf", "o_intra", "o ia"]:
+    if route_type in ["o", "ospf", "o_intra", "o ia", "ospf-1 intra"]:
         # OSPF Inter Area
         return "oia"
     if route_type in ["n1", "o n1"]:
         # OSPF NSSA Type 1
         return "on1"
     if route_type in ["n2", "o n2"]:
         # OSPF NSSA Type 2
```

### Comparing `netdoc-0.9.56/netdoc/views.py` & `netdoc-0.9.57/netdoc/views.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/netdoc.egg-info/SOURCES.txt` & `netdoc-0.9.57/netdoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.56/setup.py` & `netdoc-0.9.57/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     twine upload dist/*
 """
 
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
-__version__ = "0.9.56"
+__version__ = "0.9.57"
 
 from setuptools import find_packages, setup
 
 setup(
     name="netdoc",
     version=__version__,
     description="Network Documentation plugin for NetBox",
```

