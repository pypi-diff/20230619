# Comparing `tmp/textfsm_aos-1.1.2.tar.gz` & `tmp/textfsm_aos-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textfsm_aos-1.1.2.tar", max compression
+gzip compressed data, was "textfsm_aos-1.1.3.tar", max compression
```

## Comparing `textfsm_aos-1.1.2.tar` & `textfsm_aos-1.1.3.tar`

### file list

```diff
@@ -1,60 +1,62 @@
--rw-r--r--   0        0        0    11357 2022-09-18 14:42:27.660191 textfsm_aos-1.1.2/LICENSE
--rw-r--r--   0        0        0    11430 2022-12-20 09:27:55.846485 textfsm_aos-1.1.2/README.md
--rw-r--r--   0        0        0      723 2022-12-20 08:56:47.360408 textfsm_aos-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      160 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/__init__.py
--rw-r--r--   0        0        0     1881 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/parser.py
--rw-r--r--   0        0        0       44 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/__init__.py
--rw-r--r--   0        0        0      210 2022-11-09 09:48:22.496491 textfsm_aos-1.1.2/textfsm_aos/templates/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      636 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_802.1x_non-supplicant.textfsm
--rw-r--r--   0        0        0      538 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_802.1x_non-supplicant_unp.textfsm
--rw-r--r--   0        0        0      918 2022-12-20 08:28:31.045280 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_802.1x_users.textfsm
--rw-r--r--   0        0        0      518 2022-12-20 08:28:31.045280 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_802.1x_users_unp.textfsm
--rw-r--r--   0        0        0      896 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_chassis.textfsm
--rw-r--r--   0        0        0      345 2022-12-20 07:43:37.271948 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_command-log.textfsm
--rw-r--r--   0        0        0     1743 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_health.textfsm
--rw-r--r--   0        0        0       88 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_history.textfsm
--rw-r--r--   0        0        0      922 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_interfaces_status.textfsm
--rw-r--r--   0        0        0      490 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_ip_interface.textfsm
--rw-r--r--   0        0        0      504 2022-12-19 09:52:02.077791 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_ip_route.textfsm
--rw-r--r--   0        0        0     2137 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_lldp_remote-system.textfsm
--rw-r--r--   0        0        0      533 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_mac-address-table.textfsm
--rw-r--r--   0        0        0      274 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_microcode.textfsm
--rw-r--r--   0        0        0     1759 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_ntp_server_status.textfsm
--rw-r--r--   0        0        0      368 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_snmp_community_map.textfsm
--rw-r--r--   0        0        0      396 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_snmp_station.textfsm
--rw-r--r--   0        0        0      660 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_system.textfsm
--rw-r--r--   0        0        0     1129 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_user.textfsm
--rw-r--r--   0        0        0      668 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_vlan.textfsm
--rw-r--r--   0        0        0      611 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_vlan_port_mobile.textfsm
--rw-r--r--   0        0        0      108 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_history.textfsm
--rw-r--r--   0        0        0      594 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_arp.textfsm
--rw-r--r--   0        0        0     1043 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_chassis.textfsm
--rw-r--r--   0        0        0     1281 2022-12-20 07:43:37.271948 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_cmm.textfsm
--rw-r--r--   0        0        0      337 2022-12-06 10:26:24.922126 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_command-log.textfsm
--rw-r--r--   0        0        0     1699 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_hardware-info.textfsm
--rw-r--r--   0        0        0      777 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_health.textfsm
--rw-r--r--   0        0        0     3182 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_interfaces.textfsm
--rw-r--r--   0        0        0     1147 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_interfaces_status.textfsm
--rw-r--r--   0        0        0      601 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_ip_interface.textfsm
--rw-r--r--   0        0        0      518 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_ip_routes.textfsm
--rw-r--r--   0        0        0      493 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_linkagg.textfsm
--rw-r--r--   0        0        0      512 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_linkagg_port.textfsm
--rw-r--r--   0        0        0      260 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_log_events.textfsm
--rw-r--r--   0        0        0      711 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_mac-learning.textfsm
--rw-r--r--   0        0        0      268 2022-12-20 07:43:37.271948 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_microcode.textfsm
--rw-r--r--   0        0        0     1759 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_ntp_server_status.textfsm
--rw-r--r--   0        0        0      647 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_port-security_brief.textfsm
--rw-r--r--   0        0        0      848 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_qos_port.textfsm
--rw-r--r--   0        0        0      754 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_running-directory.textfsm
--rw-r--r--   0        0        0      371 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_snmp_community-map.textfsm
--rw-r--r--   0        0        0      396 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_snmp_station.textfsm
--rw-r--r--   0        0        0      433 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_spantree_ports.textfsm
--rw-r--r--   0        0        0      660 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_system.textfsm
--rw-r--r--   0        0        0     1056 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_transceivers.textfsm
--rw-r--r--   0        0        0      579 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_unp_user.textfsm
--rw-r--r--   0        0        0     1162 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_user.textfsm
--rw-r--r--   0        0        0      499 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_vlan.textfsm
--rw-r--r--   0        0        0      318 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_vlan_members.textfsm
--rw-r--r--   0        0        0     2462 2022-09-18 14:42:27.668191 textfsm_aos-1.1.2/textfsm_aos/templates/templates_index.yml
--rw-r--r--   0        0        0    12552 1970-01-01 00:00:00.000000 textfsm_aos-1.1.2/setup.py
--rw-r--r--   0        0        0    12301 1970-01-01 00:00:00.000000 textfsm_aos-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-09-18 14:42:27.660191 textfsm_aos-1.1.3/LICENSE
+-rw-r--r--   0        0        0    12254 2023-06-19 14:00:00.371176 textfsm_aos-1.1.3/README.md
+-rw-r--r--   0        0        0      722 2023-06-19 14:07:11.127422 textfsm_aos-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      160 2023-02-15 14:50:20.314114 textfsm_aos-1.1.3/textfsm_aos/__init__.py
+-rw-r--r--   0        0        0     1882 2023-02-17 11:14:22.309672 textfsm_aos-1.1.3/textfsm_aos/parser.py
+-rw-r--r--   0        0        0       44 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/__init__.py
+-rw-r--r--   0        0        0      210 2022-11-09 09:48:22.496491 textfsm_aos-1.1.3/textfsm_aos/templates/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      636 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_802.1x_non-supplicant.textfsm
+-rw-r--r--   0        0        0      538 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_802.1x_non-supplicant_unp.textfsm
+-rw-r--r--   0        0        0      918 2023-02-15 14:50:20.314114 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_802.1x_users.textfsm
+-rw-r--r--   0        0        0      518 2023-02-15 14:50:20.314114 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_802.1x_users_unp.textfsm
+-rw-r--r--   0        0        0      896 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_chassis.textfsm
+-rw-r--r--   0        0        0      345 2023-02-15 14:50:20.314114 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_command-log.textfsm
+-rw-r--r--   0        0        0     1743 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_health.textfsm
+-rw-r--r--   0        0        0       88 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_history.textfsm
+-rw-r--r--   0        0        0      922 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_interfaces_status.textfsm
+-rw-r--r--   0        0        0      490 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_ip_interface.textfsm
+-rw-r--r--   0        0        0      504 2023-02-15 14:50:20.314114 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_ip_route.textfsm
+-rw-r--r--   0        0        0     2137 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_lldp_remote-system.textfsm
+-rw-r--r--   0        0        0      533 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_mac-address-table.textfsm
+-rw-r--r--   0        0        0      274 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_microcode.textfsm
+-rw-r--r--   0        0        0     1759 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_ntp_server_status.textfsm
+-rw-r--r--   0        0        0      368 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_snmp_community_map.textfsm
+-rw-r--r--   0        0        0      396 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_snmp_station.textfsm
+-rw-r--r--   0        0        0      660 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_system.textfsm
+-rw-r--r--   0        0        0     1129 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_user.textfsm
+-rw-r--r--   0        0        0      668 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_vlan.textfsm
+-rw-r--r--   0        0        0      611 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_vlan_port_mobile.textfsm
+-rw-r--r--   0        0        0      108 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_history.textfsm
+-rw-r--r--   0        0        0      594 2023-02-15 14:50:20.314114 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_arp.textfsm
+-rw-r--r--   0        0        0     1043 2022-12-20 13:02:09.609606 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_chassis.textfsm
+-rw-r--r--   0        0        0     1281 2023-02-15 14:50:20.314114 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_cmm.textfsm
+-rw-r--r--   0        0        0      337 2022-12-06 10:26:24.922126 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_command-log.textfsm
+-rw-r--r--   0        0        0     1699 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_hardware-info.textfsm
+-rw-r--r--   0        0        0      777 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_health.textfsm
+-rw-r--r--   0        0        0     3182 2023-02-15 14:50:20.314114 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_interfaces.textfsm
+-rw-r--r--   0        0        0     1147 2023-02-15 14:50:20.314114 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_interfaces_status.textfsm
+-rw-r--r--   0        0        0      601 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_ip_interface.textfsm
+-rw-r--r--   0        0        0     1037 2023-02-17 11:14:22.309672 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_ip_router_database.textfsm
+-rw-r--r--   0        0        0      518 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_ip_routes.textfsm
+-rw-r--r--   0        0        0      493 2023-02-15 14:50:20.314114 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_linkagg.textfsm
+-rw-r--r--   0        0        0      512 2023-02-15 14:50:20.314114 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_linkagg_port.textfsm
+-rw-r--r--   0        0        0      260 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_log_events.textfsm
+-rw-r--r--   0        0        0      711 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_mac-learning.textfsm
+-rw-r--r--   0        0        0      268 2023-02-15 14:50:20.314114 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_microcode.textfsm
+-rw-r--r--   0        0        0     1759 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_ntp_server_status.textfsm
+-rw-r--r--   0        0        0      647 2023-02-15 14:50:20.314114 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_port-security_brief.textfsm
+-rw-r--r--   0        0        0     1795 2023-02-15 14:52:52.824797 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_qos_log.textfsm
+-rw-r--r--   0        0        0      848 2023-02-15 14:50:20.314114 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_qos_port.textfsm
+-rw-r--r--   0        0        0      754 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_running-directory.textfsm
+-rw-r--r--   0        0        0      371 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_snmp_community-map.textfsm
+-rw-r--r--   0        0        0      396 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_snmp_station.textfsm
+-rw-r--r--   0        0        0      433 2023-02-15 14:50:20.314114 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_spantree_ports.textfsm
+-rw-r--r--   0        0        0      660 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_system.textfsm
+-rw-r--r--   0        0        0     1056 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_transceivers.textfsm
+-rw-r--r--   0        0        0      579 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_unp_user.textfsm
+-rw-r--r--   0        0        0     2796 2023-06-19 13:38:29.569872 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_unp_user_details.textfsm
+-rw-r--r--   0        0        0     1162 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_user.textfsm
+-rw-r--r--   0        0        0      499 2022-09-18 14:42:27.668191 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_vlan.textfsm
+-rw-r--r--   0        0        0      334 2023-06-19 13:52:06.855070 textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_vlan_members.textfsm
+-rw-r--r--   0        0        0     2617 2023-06-19 13:45:37.946286 textfsm_aos-1.1.3/textfsm_aos/templates/templates_index.yml
+-rw-r--r--   0        0        0    13125 1970-01-01 00:00:00.000000 textfsm_aos-1.1.3/PKG-INFO
```

### Comparing `textfsm_aos-1.1.2/LICENSE` & `textfsm_aos-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/README.md` & `textfsm_aos-1.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 > Alcatel-Lucent Enterprise AOS CLI parsing
 
 Python package for Alcatel-Lucent Enterprise aos6 and aos8 parsing based on TextFSM templates.
 
 ## Why TextFSM-AOS?
 
-Parse semi-structured cli data to structured data ready to be ingested by your network automation pipeline. Autmatically transform gathered output from screen-scraping tools like Netmiko, Scrapli and Paramiko. Receive uniform data accross Alcatel-Lucent Enterprise devices running aos6 or aos8.
+Parse semi-structured cli data to structured data ready to be ingested by your network automation pipeline. Automatically transform gathered output from screen-scraping tools like Netmiko, Scrapli and Paramiko. Receive uniform data across Alcatel-Lucent Enterprise devices running aos6 or aos8.
 
 ## Installation
 
 Textfsm-aos can be installed using Git + Poetry or PyPI.
-
+s
 ## Git
 
 ```bash
 git clone https://github.com/jefvantongerloo/textfsm-aos
 poetry install
 ```
 
@@ -75,18 +75,24 @@
       "description":"Alcatel-Lucent Enterprise Security M"
    }
 ]
 ```
 
 ## Integration tests
 
-| aos version                       |                    tests            | 
-|-----------------------------------|:--------------------------------:|
-| 6.7.2.122.R08                  |    :heavy_check_mark:    |
-| 8.8.56.R02                       |    :heavy_check_mark:    |
+Due to sensitive information the gathered live data for integration testing is stored in a private repository. Releases are tested against following aos versions:
+
+| aos version                       |                    tests            |
+|-----------------------------------|:-----------------------------------:|
+| 6.7.2.122.R08                     |         :heavy_check_mark:          |
+| 8.9.73.R01                        |         :heavy_check_mark:          |
+| 8.8.56.R02                        |         :heavy_check_mark:          |
+| 8.8.152.R01                       |         :heavy_check_mark:          |
+| 8.9.73.R01                        |         :heavy_check_mark:          |
+| 8.9.107.R02                       |         :heavy_check_mark:          |
 
 ## Supported commands
 
 | command                        |                 aos6                |                aos8               |
 |--------------------------------|:-----------------------------------:|:---------------------------------:|
 | history                        |        `alias: show history`        |         :heavy_check_mark:        |
 | show 802.1x users              |          :heavy_check_mark:         |       `alias: show unp user`      |
@@ -100,28 +106,31 @@
 | show hardware-info             |                 :x:                 |         :heavy_check_mark:        |
 | show health                    |          :heavy_check_mark:         |         :heavy_check_mark:        |
 | show history                   |          :heavy_check_mark:         |          `alias: history`         |
 | show interface status          |          :heavy_check_mark:         |         :heavy_check_mark:        |
 | show interfaces                |                 :x:                 |         :heavy_check_mark:        |
 | show ip interface              |          :heavy_check_mark:         |         :heavy_check_mark:        |
 | show ip route                  |          :heavy_check_mark:         |       `alias: show ip routes`     |
+| show ip router database        |                 :x:                 |         :heavy_check_mark:        |
 | show ip routes                 |        `alias: show ip route`       |         :heavy_check_mark:        |
 | show linkagg                   |                 :x:                 |         :heavy_check_mark:        |
 | show linkagg port              |                 :x:                 |         :heavy_check_mark:        |
 | show lld remote system         |          :heavy_check_mark:         |                :x:                |
 | show log events                |                 :x:                 |         :heavy_check_mark:        |
 | show mac-address-table         |          :heavy_check_mark:         |     `alias: show mac-learning`    |
 | show mac-learning              |   `alias: show mac-address-table`   |         :heavy_check_mark:        |
 | show microcode                 |          :heavy_check_mark:         |         :heavy_check_mark:        |
 | show ntp server status         |          :heavy_check_mark:         |         :heavy_check_mark:        |
 | show port-security brief       |                 :x:                 |         :heavy_check_mark:        |
 | show qos port                  |                 :x:                 |         :heavy_check_mark:        |
 | show unp user                  |     `alias: show 802.1x users`      |         :heavy_check_mark:        |
+| show unp user details          |                 :x:                 |         :heavy_check_mark:        |
 | show user                      |          :heavy_check_mark:         |         :heavy_check_mark:        |
 | show running-directory         |                 :x:                 |         :heavy_check_mark:        |
+| show qos log                   |                 :x:                 |         :heavy_check_mark:        |
 | show snmp station              |          :heavy_check_mark:         |         :heavy_check_mark:        |
 | show snmp community map        |          :heavy_check_mark:         |  `alias: show snmp community-map` |
 | show snmp community-map        |   `alias: show snmp community map`  |         :heavy_check_mark:        |
 | show spantree ports            |                 :x:                 |         :heavy_check_mark:        |
 | show system                    |          :heavy_check_mark:         |         :heavy_check_mark:        |
 | show transceivers              |                 :x:                 |         :heavy_check_mark:        |
 | show vlan                      |          :heavy_check_mark:         |         :heavy_check_mark:        |
```

### Comparing `textfsm_aos-1.1.2/pyproject.toml` & `textfsm_aos-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textfsm_aos"
-version = "1.1.2"
+version = "1.1.3"
 description = "Alcatel-Lucent Enterprise AOS CLI parsing (TextFSM)"
 authors = ["Jef Vantongerloo <jefvantongerloo@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/jefvantongerloo/textfsm-aos"
 homepage = "https://github.com/jefvantongerloo/textfsm-aos"
 keywords = ["network automation", "textfsm", "scraping", "Alcatel-Lucent Enterprise", "infrastructure"]
@@ -13,13 +13,13 @@
 python = ">=3.8"
 textfsm = "^1.1.0"
 PyYAML = "^6.0"
 
 [tool.poetry.dev-dependencies]
 textfsm = "^1.1.0"
 PyYAML = "^6.0"
-tox = "^3.28.0"
-pytest = "^7.1.3"
+tox = "^4.6.0"
+pytest = "^7.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `textfsm_aos-1.1.2/textfsm_aos/parser.py` & `textfsm_aos-1.1.3/textfsm_aos/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,12 +48,12 @@
     Returns:
         output: structured data (dict)
     """
     template_index = _search_template_index(platform, command)
     if template_index:
         structured_response = _parse_textfsm(template_index, data)
     else:
-        raise Exception(
+        raise ValueError(
             f"Unable to find platform:{platform} or command:{command} in supported values."
         )
 
     return structured_response
```

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_802.1x_non-supplicant.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_802.1x_non-supplicant.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_802.1x_non-supplicant_unp.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_802.1x_non-supplicant_unp.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_802.1x_users.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_802.1x_users.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_802.1x_users_unp.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_802.1x_users_unp.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_chassis.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_chassis.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_health.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_health.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_interfaces_status.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_interfaces_status.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_lldp_remote-system.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_lldp_remote-system.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_mac-address-table.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_mac-address-table.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_ntp_server_status.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_ntp_server_status.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_system.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_system.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_user.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_user.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_vlan.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_vlan.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos6_show_vlan_port_mobile.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos6_show_vlan_port_mobile.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_arp.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_arp.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_chassis.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_chassis.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_cmm.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_cmm.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_hardware-info.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_hardware-info.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_health.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_health.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_interfaces.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_interfaces.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_interfaces_status.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_interfaces_status.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_ip_interface.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_ip_interface.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_ip_routes.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_ip_routes.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_linkagg_port.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_linkagg_port.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_mac-learning.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_mac-learning.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_ntp_server_status.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_ntp_server_status.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_port-security_brief.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_port-security_brief.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_qos_port.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_qos_port.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_running-directory.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_running-directory.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_system.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_system.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_transceivers.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_transceivers.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_unp_user.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_unp_user.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/ale_aos8_show_user.textfsm` & `textfsm_aos-1.1.3/textfsm_aos/templates/ale_aos8_show_user.textfsm`

 * *Files identical despite different names*

### Comparing `textfsm_aos-1.1.2/textfsm_aos/templates/templates_index.yml` & `textfsm_aos-1.1.3/textfsm_aos/templates/templates_index.yml`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,16 @@
   platform: ale_aos8  
 - command: show ip interface
   platform: ale_aos6
 - command: show ip interface
   platform: ale_aos8
 - command: show ip route
   platform: ale_aos6
+- command: show ip router database
+  platform: ale_aos8
 - command: show ip routes
   platform: ale_aos8
 - command: show linkagg
   platform: ale_aos8
 - command: show linkagg port
   platform: ale_aos8
 - command: show lldp remote-system
@@ -61,18 +63,22 @@
   platform: ale_aos8
 - command: show ntp server status
   platform: ale_aos6
 - command: show ntp server status
   platform: ale_aos8
 - command: show port-security brief
   platform: ale_aos8
+- command: show qos log
+  platform: ale_aos8
 - command: show qos port
   platform: ale_aos8
 - command: show unp user
   platform: ale_aos8
+- command: show unp user details
+  platform: ale_aos8
 - command: show user
   platform: ale_aos6
 - command: show user
   platform: ale_aos8
 - command: show running-directory
   platform: ale_aos8
 - command: show snmp station
```

### Comparing `textfsm_aos-1.1.2/setup.py` & `textfsm_aos-1.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,352 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: textfsm-aos
+Version: 1.1.3
+Summary: Alcatel-Lucent Enterprise AOS CLI parsing (TextFSM)
+Home-page: https://github.com/jefvantongerloo/textfsm-aos
+License: Apache-2.0
+Keywords: network automation,textfsm,scraping,Alcatel-Lucent Enterprise,infrastructure
+Author: Jef Vantongerloo
+Author-email: jefvantongerloo@gmail.com
+Requires-Python: >=3.8
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: textfsm (>=1.1.0,<2.0.0)
+Project-URL: Repository, https://github.com/jefvantongerloo/textfsm-aos
+Description-Content-Type: text/markdown
 
-packages = \
-['textfsm_aos', 'textfsm_aos.templates']
+[![Build Status](https://app.travis-ci.com/jefvantongerloo/textfsm-aos.svg?branch=main)](https://app.travis-ci.com/jefvantongerloo/textfsm-aos)
 
-package_data = \
-{'': ['*']}
+# TEXTFSM-AOS
 
-install_requires = \
-['PyYAML>=6.0,<7.0', 'textfsm>=1.1.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'textfsm-aos',
-    'version': '1.1.2',
-    'description': 'Alcatel-Lucent Enterprise AOS CLI parsing (TextFSM)',
-    'long_description': '[![Build Status](https://app.travis-ci.com/jefvantongerloo/textfsm-aos.svg?branch=main)](https://app.travis-ci.com/jefvantongerloo/textfsm-aos)\n\n# TEXTFSM-AOS\n\n> Alcatel-Lucent Enterprise AOS CLI parsing\n\nPython package for Alcatel-Lucent Enterprise aos6 and aos8 parsing based on TextFSM templates.\n\n## Why TextFSM-AOS?\n\nParse semi-structured cli data to structured data ready to be ingested by your network automation pipeline. Autmatically transform gathered output from screen-scraping tools like Netmiko, Scrapli and Paramiko. Receive uniform data accross Alcatel-Lucent Enterprise devices running aos6 or aos8.\n\n## Installation\n\nTextfsm-aos can be installed using Git + Poetry or PyPI.\n\n## Git\n\n```bash\ngit clone https://github.com/jefvantongerloo/textfsm-aos\npoetry install\n```\n\n## PyPI\n\n```bash\npip install textfsm-aos\n```\n\n## Getting started\n\nProvide screen-scraped data to parser\n\n```python\nfrom textfsm_aos.parser import parse\n\nsample_data = """\n   Package           Release       Size     Description\n-----------------+---------------+--------+-----------------------------------\nKFbase.img        6.7.2.89.R06    18059551 Alcatel-Lucent Enterprise Base Softw\nKFos.img          6.7.2.89.R06     3566798 Alcatel-Lucent Enterprise OS\nKFeni.img         6.7.2.89.R06     6123991 Alcatel-Lucent Enterprise NI softwar\nKFsecu.img        6.7.2.89.R06      649383 Alcatel-Lucent Enterprise Security M\n"""\n\nparse("ale_aos6", "show microcode", sample_data)\n```\n\nparsed result\n\n```python\n[\n   {\n      "package":"KFbase.img",\n      "release":"6.7.2.89.R06",\n      "size":"18059551",\n      "description":"Alcatel-Lucent Enterprise Base Softw"\n   },\n   {\n      "package":"KFos.img",\n      "release":"6.7.2.89.R06",\n      "size":"3566798",\n      "description":"Alcatel-Lucent Enterprise OS"\n   },\n   {\n      "package":"KFeni.img",\n      "release":"6.7.2.89.R06",\n      "size":"6123991",\n      "description":"Alcatel-Lucent Enterprise NI softwar"\n   },\n   {\n      "package":"KFsecu.img",\n      "release":"6.7.2.89.R06",\n      "size":"649383",\n      "description":"Alcatel-Lucent Enterprise Security M"\n   }\n]\n```\n\n## Integration tests\n\n| aos version                       |                    tests            | \n|-----------------------------------|:--------------------------------:|\n| 6.7.2.122.R08                  |    :heavy_check_mark:    |\n| 8.8.56.R02                       |    :heavy_check_mark:    |\n\n## Supported commands\n\n| command                        |                 aos6                |                aos8               |\n|--------------------------------|:-----------------------------------:|:---------------------------------:|\n| history                        |        `alias: show history`        |         :heavy_check_mark:        |\n| show 802.1x users              |          :heavy_check_mark:         |       `alias: show unp user`      |\n| show 802.1x users unp          |          :heavy_check_mark:         |                :x:                |\n| show 802.1x non-supplicant     |          :heavy_check_mark:         |                :x:                |\n| show 802.1x non-supplicant unp |          :heavy_check_mark:         |                :x:                |\n| show arp                       |                 :x:                 |         :heavy_check_mark:        |\n| show chassis                   |          :heavy_check_mark:         |         :heavy_check_mark:        |\n| show cmm                       |                 :x:                 |         :heavy_check_mark:        |\n| show command-log               |          :heavy_check_mark:         |         :heavy_check_mark:        |\n| show hardware-info             |                 :x:                 |         :heavy_check_mark:        |\n| show health                    |          :heavy_check_mark:         |         :heavy_check_mark:        |\n| show history                   |          :heavy_check_mark:         |          `alias: history`         |\n| show interface status          |          :heavy_check_mark:         |         :heavy_check_mark:        |\n| show interfaces                |                 :x:                 |         :heavy_check_mark:        |\n| show ip interface              |          :heavy_check_mark:         |         :heavy_check_mark:        |\n| show ip route                  |          :heavy_check_mark:         |       `alias: show ip routes`     |\n| show ip routes                 |        `alias: show ip route`       |         :heavy_check_mark:        |\n| show linkagg                   |                 :x:                 |         :heavy_check_mark:        |\n| show linkagg port              |                 :x:                 |         :heavy_check_mark:        |\n| show lld remote system         |          :heavy_check_mark:         |                :x:                |\n| show log events                |                 :x:                 |         :heavy_check_mark:        |\n| show mac-address-table         |          :heavy_check_mark:         |     `alias: show mac-learning`    |\n| show mac-learning              |   `alias: show mac-address-table`   |         :heavy_check_mark:        |\n| show microcode                 |          :heavy_check_mark:         |         :heavy_check_mark:        |\n| show ntp server status         |          :heavy_check_mark:         |         :heavy_check_mark:        |\n| show port-security brief       |                 :x:                 |         :heavy_check_mark:        |\n| show qos port                  |                 :x:                 |         :heavy_check_mark:        |\n| show unp user                  |     `alias: show 802.1x users`      |         :heavy_check_mark:        |\n| show user                      |          :heavy_check_mark:         |         :heavy_check_mark:        |\n| show running-directory         |                 :x:                 |         :heavy_check_mark:        |\n| show snmp station              |          :heavy_check_mark:         |         :heavy_check_mark:        |\n| show snmp community map        |          :heavy_check_mark:         |  `alias: show snmp community-map` |\n| show snmp community-map        |   `alias: show snmp community map`  |         :heavy_check_mark:        |\n| show spantree ports            |                 :x:                 |         :heavy_check_mark:        |\n| show system                    |          :heavy_check_mark:         |         :heavy_check_mark:        |\n| show transceivers              |                 :x:                 |         :heavy_check_mark:        |\n| show vlan                      |          :heavy_check_mark:         |         :heavy_check_mark:        |\n| show vlan members              |                 :x:                 |         :heavy_check_mark:        |\n| show vlan port mobile          |          :heavy_check_mark:         |                :x:                |\n\n## Direct TextFSM example usage\n\nBypass the build-in parser functionality and use the TextFSM templates directly in network cli scraping and orchestration tools like Netmiko, Scrapli and Ansible.\n\n### Scrapli\n\nPython script:\n\n```python\nfrom scrapli import Scrapli\nfrom scrapli.helper import textfsm_parse\n\ndevice = {\n    "host": "<host ip>",\n    "auth_username": "<username>",\n    "auth_password": "<password>",\n    "auth_strict_key": False,\n    "transport": "ssh2",\n    "platform": "alcatel_aos",\n}\n\nwith Scrapli(**device) as conn:\n    response = conn.send_command("show health").result\n    structured_response = textfsm_parse(\n        "templates/ale_aos6_show_health.textfsm", response\n    )\n```\n\nExample output:\n\n```python\n[\n   {\n      "resource":"Receive",\n      "limit":"80",\n      "current":"01",\n      "min_avg":"01",\n      "hr_avg":"01",\n      "hr_max":"01"\n   },\n   {\n      "resource":"Transmit/Receive",\n      "limit":"80",\n      "current":"01",\n      "min_avg":"01",\n      "hr_avg":"01",\n      "hr_max":"01"\n   },\n   {\n      "resource":"Memory",\n      "limit":"80",\n      "current":"76",\n      "min_avg":"76",\n      "hr_avg":"76",\n      "hr_max":"76"\n   },\n   {\n      "resource":"Cpu",\n      "limit":"80",\n      "current":"32",\n      "min_avg":"33",\n      "hr_avg":"29",\n      "hr_max":"97"\n   }\n]\n```\n\n### Netmiko\n\nPython script:\n\n```python\nfrom netmiko import ConnectHandler\n\ndevice = {\n    \'device_type\': \'alcatel_aos\',\n    \'host\': \'<host ip>\',\n    \'username\': \'<username>\',\n    \'password\': \'<password>\'\n}\n\nwith ConnectHandler(**device) as conn:\n    output = conn.send_command("show health", use_textfsm=True, textfsm_template="textfsm-aos/templates/ale_aos6_show_health.textfsm")\n```\n\nExample Output:\n\n```python\n[\n   {\n      "resource":"Receive",\n      "limit":"80",\n      "current":"01",\n      "min_avg":"01",\n      "hr_avg":"01",\n      "hr_max":"01"\n   },\n   {\n      "resource":"Transmit/Receive",\n      "limit":"80",\n      "current":"01",\n      "min_avg":"01",\n      "hr_avg":"01",\n      "hr_max":"01"\n   },\n   {\n      "resource":"Memory",\n      "limit":"80",\n      "current":"76",\n      "min_avg":"76",\n      "hr_avg":"76",\n      "hr_max":"76"\n   },\n   {\n      "resource":"Cpu",\n      "limit":"80",\n      "current":"32",\n      "min_avg":"33",\n      "hr_avg":"29",\n      "hr_max":"97"\n   }\n]\n```\n\n### Ansible\n\nAnsible task:\n\n```yaml\n- name: AOS6 >> parsed with textfsm\n  set_fact:\n    health: "{{ health-aos6 | ansible.netcommon.parse_cli_textfsm(\'textfsm/templates/ale_aos6_show_health.textfsm\') }}"\n```\n\nExample Output:\n\n```yaml\n    health:\n    - healthModuleCpu1HrAvg: \'29\'\n      healthModuleCpu1HrMax: \'98\'\n      healthModuleCpu1MinAvg: \'26\'\n      healthModuleCpuLatest: \'31\'\n      healthModuleCpuLimit: \'80\'\n      healthModuleMemory1HrAvg: \'76\'\n      healthModuleMemory1HrMax: \'76\'\n      healthModuleMemory1MinAvg: \'76\'\n      healthModuleMemoryLatest: \'76\'\n      healthModuleMemoryLimit: \'80\'\n      healthModuleRx1HrAvg: \'01\'\n      healthModuleRx1HrMax: \'01\'\n      healthModuleRx1MinAvg: \'01\'\n      healthModuleRxLatest: \'01\'\n      healthModuleRxLimit: \'80\'\n      healthModuleRxTxRx1HrAvg: \'01\'\n      healthModuleRxTxRx1HrMax: \'01\'\n      healthModuleRxTxRx1MinAvg: \'01\'\n      healthModuleRxTxRxLatest: \'01\'\n      healthModuleRxTxRxLimit: \'80\'\n      healthModuleSlot: \'1\'\n```\n\n## How to contribute\n\n1. Fork and create a branch with naming `<platform>_<command>` (for example: ale_aos8_show_system).\n\n2. Add TextFSM template file in templates folder with naming `<platform>_<command>.textfsm`.\n\n3. Add entry in templates_index with attribute command and platform.\n\n4. Add test folder in \'templates\' with naming `<platform>_<command>`.\n\n5. Add sample cli output file in newly created folder `<platform>_<command>.txt`.\n\n6. Add expected parsed data from sample cli output in `<platform>_<command>.yml`.\n\n7. Run linting `tox` and tests `pytest`.\n\n## How to setup development environment\n\n1. Install `Poetry` package manager via `pip install poetry`\n\n2. Install dev dependencies and textfsm-aos package in development mode with `poetry install`\n\n3. Open virtual environment `poetry shell`\n\n## Related projects\n\n- Google TextFSM: [https://github.com/google/textfsm](https://github.com/google/textfsm)\n- Scrapli: [https://github.com/carlmontanari/scrapli](https://github.com/carlmontanari/scrapli)\n- Netmiko: [https://github.com/ktbyers/netmiko](https://github.com/ktbyers/netmiko)\n- Getting started with TextFSM: [https://pyneng.readthedocs.io](https://pyneng.readthedocs.io/en/latest/book/21_textfsm/index.html)\n',
-    'author': 'Jef Vantongerloo',
-    'author_email': 'jefvantongerloo@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/jefvantongerloo/textfsm-aos',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8',
+> Alcatel-Lucent Enterprise AOS CLI parsing
+
+Python package for Alcatel-Lucent Enterprise aos6 and aos8 parsing based on TextFSM templates.
+
+## Why TextFSM-AOS?
+
+Parse semi-structured cli data to structured data ready to be ingested by your network automation pipeline. Automatically transform gathered output from screen-scraping tools like Netmiko, Scrapli and Paramiko. Receive uniform data across Alcatel-Lucent Enterprise devices running aos6 or aos8.
+
+## Installation
+
+Textfsm-aos can be installed using Git + Poetry or PyPI.
+s
+## Git
+
+```bash
+git clone https://github.com/jefvantongerloo/textfsm-aos
+poetry install
+```
+
+## PyPI
+
+```bash
+pip install textfsm-aos
+```
+
+## Getting started
+
+Provide screen-scraped data to parser
+
+```python
+from textfsm_aos.parser import parse
+
+sample_data = """
+   Package           Release       Size     Description
+-----------------+---------------+--------+-----------------------------------
+KFbase.img        6.7.2.89.R06    18059551 Alcatel-Lucent Enterprise Base Softw
+KFos.img          6.7.2.89.R06     3566798 Alcatel-Lucent Enterprise OS
+KFeni.img         6.7.2.89.R06     6123991 Alcatel-Lucent Enterprise NI softwar
+KFsecu.img        6.7.2.89.R06      649383 Alcatel-Lucent Enterprise Security M
+"""
+
+parse("ale_aos6", "show microcode", sample_data)
+```
+
+parsed result
+
+```python
+[
+   {
+      "package":"KFbase.img",
+      "release":"6.7.2.89.R06",
+      "size":"18059551",
+      "description":"Alcatel-Lucent Enterprise Base Softw"
+   },
+   {
+      "package":"KFos.img",
+      "release":"6.7.2.89.R06",
+      "size":"3566798",
+      "description":"Alcatel-Lucent Enterprise OS"
+   },
+   {
+      "package":"KFeni.img",
+      "release":"6.7.2.89.R06",
+      "size":"6123991",
+      "description":"Alcatel-Lucent Enterprise NI softwar"
+   },
+   {
+      "package":"KFsecu.img",
+      "release":"6.7.2.89.R06",
+      "size":"649383",
+      "description":"Alcatel-Lucent Enterprise Security M"
+   }
+]
+```
+
+## Integration tests
+
+Due to sensitive information the gathered live data for integration testing is stored in a private repository. Releases are tested against following aos versions:
+
+| aos version                       |                    tests            |
+|-----------------------------------|:-----------------------------------:|
+| 6.7.2.122.R08                     |         :heavy_check_mark:          |
+| 8.9.73.R01                        |         :heavy_check_mark:          |
+| 8.8.56.R02                        |         :heavy_check_mark:          |
+| 8.8.152.R01                       |         :heavy_check_mark:          |
+| 8.9.73.R01                        |         :heavy_check_mark:          |
+| 8.9.107.R02                       |         :heavy_check_mark:          |
+
+## Supported commands
+
+| command                        |                 aos6                |                aos8               |
+|--------------------------------|:-----------------------------------:|:---------------------------------:|
+| history                        |        `alias: show history`        |         :heavy_check_mark:        |
+| show 802.1x users              |          :heavy_check_mark:         |       `alias: show unp user`      |
+| show 802.1x users unp          |          :heavy_check_mark:         |                :x:                |
+| show 802.1x non-supplicant     |          :heavy_check_mark:         |                :x:                |
+| show 802.1x non-supplicant unp |          :heavy_check_mark:         |                :x:                |
+| show arp                       |                 :x:                 |         :heavy_check_mark:        |
+| show chassis                   |          :heavy_check_mark:         |         :heavy_check_mark:        |
+| show cmm                       |                 :x:                 |         :heavy_check_mark:        |
+| show command-log               |          :heavy_check_mark:         |         :heavy_check_mark:        |
+| show hardware-info             |                 :x:                 |         :heavy_check_mark:        |
+| show health                    |          :heavy_check_mark:         |         :heavy_check_mark:        |
+| show history                   |          :heavy_check_mark:         |          `alias: history`         |
+| show interface status          |          :heavy_check_mark:         |         :heavy_check_mark:        |
+| show interfaces                |                 :x:                 |         :heavy_check_mark:        |
+| show ip interface              |          :heavy_check_mark:         |         :heavy_check_mark:        |
+| show ip route                  |          :heavy_check_mark:         |       `alias: show ip routes`     |
+| show ip router database        |                 :x:                 |         :heavy_check_mark:        |
+| show ip routes                 |        `alias: show ip route`       |         :heavy_check_mark:        |
+| show linkagg                   |                 :x:                 |         :heavy_check_mark:        |
+| show linkagg port              |                 :x:                 |         :heavy_check_mark:        |
+| show lld remote system         |          :heavy_check_mark:         |                :x:                |
+| show log events                |                 :x:                 |         :heavy_check_mark:        |
+| show mac-address-table         |          :heavy_check_mark:         |     `alias: show mac-learning`    |
+| show mac-learning              |   `alias: show mac-address-table`   |         :heavy_check_mark:        |
+| show microcode                 |          :heavy_check_mark:         |         :heavy_check_mark:        |
+| show ntp server status         |          :heavy_check_mark:         |         :heavy_check_mark:        |
+| show port-security brief       |                 :x:                 |         :heavy_check_mark:        |
+| show qos port                  |                 :x:                 |         :heavy_check_mark:        |
+| show unp user                  |     `alias: show 802.1x users`      |         :heavy_check_mark:        |
+| show unp user details          |                 :x:                 |         :heavy_check_mark:        |
+| show user                      |          :heavy_check_mark:         |         :heavy_check_mark:        |
+| show running-directory         |                 :x:                 |         :heavy_check_mark:        |
+| show qos log                   |                 :x:                 |         :heavy_check_mark:        |
+| show snmp station              |          :heavy_check_mark:         |         :heavy_check_mark:        |
+| show snmp community map        |          :heavy_check_mark:         |  `alias: show snmp community-map` |
+| show snmp community-map        |   `alias: show snmp community map`  |         :heavy_check_mark:        |
+| show spantree ports            |                 :x:                 |         :heavy_check_mark:        |
+| show system                    |          :heavy_check_mark:         |         :heavy_check_mark:        |
+| show transceivers              |                 :x:                 |         :heavy_check_mark:        |
+| show vlan                      |          :heavy_check_mark:         |         :heavy_check_mark:        |
+| show vlan members              |                 :x:                 |         :heavy_check_mark:        |
+| show vlan port mobile          |          :heavy_check_mark:         |                :x:                |
+
+## Direct TextFSM example usage
+
+Bypass the build-in parser functionality and use the TextFSM templates directly in network cli scraping and orchestration tools like Netmiko, Scrapli and Ansible.
+
+### Scrapli
+
+Python script:
+
+```python
+from scrapli import Scrapli
+from scrapli.helper import textfsm_parse
+
+device = {
+    "host": "<host ip>",
+    "auth_username": "<username>",
+    "auth_password": "<password>",
+    "auth_strict_key": False,
+    "transport": "ssh2",
+    "platform": "alcatel_aos",
 }
 
+with Scrapli(**device) as conn:
+    response = conn.send_command("show health").result
+    structured_response = textfsm_parse(
+        "templates/ale_aos6_show_health.textfsm", response
+    )
+```
+
+Example output:
+
+```python
+[
+   {
+      "resource":"Receive",
+      "limit":"80",
+      "current":"01",
+      "min_avg":"01",
+      "hr_avg":"01",
+      "hr_max":"01"
+   },
+   {
+      "resource":"Transmit/Receive",
+      "limit":"80",
+      "current":"01",
+      "min_avg":"01",
+      "hr_avg":"01",
+      "hr_max":"01"
+   },
+   {
+      "resource":"Memory",
+      "limit":"80",
+      "current":"76",
+      "min_avg":"76",
+      "hr_avg":"76",
+      "hr_max":"76"
+   },
+   {
+      "resource":"Cpu",
+      "limit":"80",
+      "current":"32",
+      "min_avg":"33",
+      "hr_avg":"29",
+      "hr_max":"97"
+   }
+]
+```
+
+### Netmiko
+
+Python script:
+
+```python
+from netmiko import ConnectHandler
+
+device = {
+    'device_type': 'alcatel_aos',
+    'host': '<host ip>',
+    'username': '<username>',
+    'password': '<password>'
+}
+
+with ConnectHandler(**device) as conn:
+    output = conn.send_command("show health", use_textfsm=True, textfsm_template="textfsm-aos/templates/ale_aos6_show_health.textfsm")
+```
+
+Example Output:
+
+```python
+[
+   {
+      "resource":"Receive",
+      "limit":"80",
+      "current":"01",
+      "min_avg":"01",
+      "hr_avg":"01",
+      "hr_max":"01"
+   },
+   {
+      "resource":"Transmit/Receive",
+      "limit":"80",
+      "current":"01",
+      "min_avg":"01",
+      "hr_avg":"01",
+      "hr_max":"01"
+   },
+   {
+      "resource":"Memory",
+      "limit":"80",
+      "current":"76",
+      "min_avg":"76",
+      "hr_avg":"76",
+      "hr_max":"76"
+   },
+   {
+      "resource":"Cpu",
+      "limit":"80",
+      "current":"32",
+      "min_avg":"33",
+      "hr_avg":"29",
+      "hr_max":"97"
+   }
+]
+```
+
+### Ansible
+
+Ansible task:
+
+```yaml
+- name: AOS6 >> parsed with textfsm
+  set_fact:
+    health: "{{ health-aos6 | ansible.netcommon.parse_cli_textfsm('textfsm/templates/ale_aos6_show_health.textfsm') }}"
+```
+
+Example Output:
+
+```yaml
+    health:
+    - healthModuleCpu1HrAvg: '29'
+      healthModuleCpu1HrMax: '98'
+      healthModuleCpu1MinAvg: '26'
+      healthModuleCpuLatest: '31'
+      healthModuleCpuLimit: '80'
+      healthModuleMemory1HrAvg: '76'
+      healthModuleMemory1HrMax: '76'
+      healthModuleMemory1MinAvg: '76'
+      healthModuleMemoryLatest: '76'
+      healthModuleMemoryLimit: '80'
+      healthModuleRx1HrAvg: '01'
+      healthModuleRx1HrMax: '01'
+      healthModuleRx1MinAvg: '01'
+      healthModuleRxLatest: '01'
+      healthModuleRxLimit: '80'
+      healthModuleRxTxRx1HrAvg: '01'
+      healthModuleRxTxRx1HrMax: '01'
+      healthModuleRxTxRx1MinAvg: '01'
+      healthModuleRxTxRxLatest: '01'
+      healthModuleRxTxRxLimit: '80'
+      healthModuleSlot: '1'
+```
+
+## How to contribute
+
+1. Fork and create a branch with naming `<platform>_<command>` (for example: ale_aos8_show_system).
+
+2. Add TextFSM template file in templates folder with naming `<platform>_<command>.textfsm`.
+
+3. Add entry in templates_index with attribute command and platform.
+
+4. Add test folder in 'templates' with naming `<platform>_<command>`.
+
+5. Add sample cli output file in newly created folder `<platform>_<command>.txt`.
+
+6. Add expected parsed data from sample cli output in `<platform>_<command>.yml`.
+
+7. Run linting `tox` and tests `pytest`.
+
+## How to setup development environment
+
+1. Install `Poetry` package manager via `pip install poetry`
+
+2. Install dev dependencies and textfsm-aos package in development mode with `poetry install`
+
+3. Open virtual environment `poetry shell`
+
+## Related projects
+
+- Google TextFSM: [https://github.com/google/textfsm](https://github.com/google/textfsm)
+- Scrapli: [https://github.com/carlmontanari/scrapli](https://github.com/carlmontanari/scrapli)
+- Netmiko: [https://github.com/ktbyers/netmiko](https://github.com/ktbyers/netmiko)
+- Getting started with TextFSM: [https://pyneng.readthedocs.io](https://pyneng.readthedocs.io/en/latest/book/21_textfsm/index.html)
 
-setup(**setup_kwargs)
```

