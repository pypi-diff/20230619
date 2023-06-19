# Comparing `tmp/mistapi-0.40.1.tar.gz` & `tmp/mistapi-0.40.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistapi-0.40.1.tar", last modified: Tue Jun 13 20:28:16 2023, max compression
+gzip compressed data, was "mistapi-0.40.2.tar", last modified: Mon Jun 19 15:17:39 2023, max compression
```

## Comparing `mistapi-0.40.1.tar` & `mistapi-0.40.2.tar`

### file list

```diff
@@ -1,237 +1,237 @@
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.480102 mistapi-0.40.1/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-01-13 07:55:51.000000 mistapi-0.40.1/LICENSE
--rw-r--r--   0 tmunzer    (502) staff       (20)    11281 2023-06-13 20:28:16.480228 mistapi-0.40.1/PKG-INFO
--rw-r--r--   0 tmunzer    (502) staff       (20)    10505 2023-06-13 20:27:38.000000 mistapi-0.40.1/README.md
--rw-r--r--   0 tmunzer    (502) staff       (20)      976 2023-06-13 20:28:05.000000 mistapi-0.40.1/pyproject.toml
--rw-r--r--   0 tmunzer    (502) staff       (20)      125 2023-06-13 20:28:16.480650 mistapi-0.40.1/setup.cfg
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.309313 mistapi-0.40.1/src/
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.324350 mistapi-0.40.1/src/mistapi/
--rw-r--r--   0 tmunzer    (502) staff       (20)     7909 2023-04-20 13:57:39.000000 mistapi-0.40.1/src/mistapi/__api_request.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2962 2023-02-21 11:06:36.000000 mistapi-0.40.1/src/mistapi/__api_response.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    21804 2023-06-01 19:27:20.000000 mistapi-0.40.1/src/mistapi/__api_session.py
--rw-r--r--   0 tmunzer    (502) staff       (20)      635 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2229 2023-02-13 15:54:52.000000 mistapi-0.40.1/src/mistapi/__logger.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.327114 mistapi-0.40.1/src/mistapi/__models/
--rw-r--r--   0 tmunzer    (502) staff       (20)        0 2023-02-21 08:35:01.000000 mistapi-0.40.1/src/mistapi/__models/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1530 2023-05-30 09:43:55.000000 mistapi-0.40.1/src/mistapi/__models/privilege.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2029 2023-02-09 11:01:08.000000 mistapi-0.40.1/src/mistapi/__pagination.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.327677 mistapi-0.40.1/src/mistapi/api/
--rw-r--r--   0 tmunzer    (502) staff       (20)      446 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.328071 mistapi-0.40.1/src/mistapi/api/v1/
--rw-r--r--   0 tmunzer    (502) staff       (20)      869 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.335713 mistapi-0.40.1/src/mistapi/api/v1/const/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1235 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1729 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/alarm_defs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2027 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/ap_channels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1730 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/ap_led_status.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1713 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/applications.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1756 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/call_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1770 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/client_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1707 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/countries.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1402 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/default_gateway_config.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1770 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/device_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1715 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/device_models.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1729 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/insight_metrics.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1712 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/languages.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1055 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/license_types.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1770 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/mxedge_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1715 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/mxedge_models.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1807 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/other_device_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1715 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/const/traffic_types.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.339406 mistapi-0.40.1/src/mistapi/api/v1/installer/
--rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.355910 mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/
--rw-r--r--   0 tmunzer    (502) staff       (20)      798 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1968 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/alarmtemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1968 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7123 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1972 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/rftemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1947 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/secpolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1940 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/sitegroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7487 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/sites.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.356976 mistapi-0.40.1/src/mistapi/api/v1/installer/sites/
--rw-r--r--   0 tmunzer    (502) staff       (20)      471 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/sites/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1168 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/installer/sites/optimize.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.357876 mistapi-0.40.1/src/mistapi/api/v1/invite/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/invite/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1099 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/invite/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.361064 mistapi-0.40.1/src/mistapi/api/v1/login/
--rw-r--r--   0 tmunzer    (502) staff       (20)      584 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/login/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1136 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/login/login.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1145 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/login/lookup.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2628 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/login/oauth.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1155 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/login/two_factor.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.362065 mistapi-0.40.1/src/mistapi/api/v1/logout/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/logout/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)      984 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/logout/logout.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.364218 mistapi-0.40.1/src/mistapi/api/v1/mobile/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/mobile/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1257 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/mobile/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.372494 mistapi-0.40.1/src/mistapi/api/v1/msps/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1104 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3887 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/admins.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1250 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/claim.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1205 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/inventory.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2667 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/invites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2620 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1828 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/logo.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4444 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2981 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/msps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/orggroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5244 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/orgs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1660 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/search.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4002 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/ssoroles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5981 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/ssos.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3637 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1476 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/suggestion.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3225 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/msps/tickets.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.425419 mistapi-0.40.1/src/mistapi/api/v1/orgs/
--rw-r--r--   0 tmunzer    (502) staff       (20)     3208 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3255 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/admins.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6440 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/alarms.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7576 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/alarmtemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/apitokens.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4730 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/aptemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4762 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/assetfilters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5989 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/assets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2344 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/call.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1709 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/cert.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1250 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/claim.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    11397 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1236 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/clone.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1846 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/crl.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7034 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    20091 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4812 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/evpn_topologies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4870 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/gatewaytemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6514 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/guests.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2978 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5034 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/inventory.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2667 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/invites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6927 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/jsi.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2503 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5217 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1434 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/maps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4754 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/mxclusters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    15280 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/mxedges.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/mxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/nacrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4618 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/nactags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/networks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4872 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/networktemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1407 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/ocdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2975 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/orgs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8802 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/otherdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1913 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/pma.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4702 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/pskportals.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8274 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/psks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4730 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/rftemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1316 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/sdkclients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6892 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/sdkinvites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4719 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/sdktemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4721 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/secpolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4825 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/servicepolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/services.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    16586 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/setting.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4702 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/sitegroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8619 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/sites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4788 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/sitetemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/ssoroles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8223 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/ssos.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4767 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/ssr.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    32140 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1747 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5449 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/templates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6846 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/tickets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1758 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/troubleshoot.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4541 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/vpns.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1344 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/wan_client.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4779 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/wan_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/webhooks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3540 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/wired_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7466 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/wlans.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5236 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/wxrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5887 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/wxtags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/orgs/wxtunnels.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.426516 mistapi-0.40.1/src/mistapi/api/v1/recover/
--rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/recover/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1158 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/recover/recover.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1110 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/recover/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.427648 mistapi-0.40.1/src/mistapi/api/v1/register/
--rw-r--r--   0 tmunzer    (502) staff       (20)      508 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/register/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1161 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/register/register.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1103 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/register/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.431521 mistapi-0.40.1/src/mistapi/api/v1/self/
--rw-r--r--   0 tmunzer    (502) staff       (20)      707 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/self/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2916 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/self/apitokens.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2596 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/self/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2015 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/self/oauth.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2109 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/self/self.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/self/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1837 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/self/two_factor.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1756 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/self/update.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.478405 mistapi-0.40.1/src/mistapi/api/v1/sites/
--rw-r--r--   0 tmunzer    (502) staff       (20)     2588 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8657 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/alarms.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2655 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/anomaly.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1861 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/apps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4797 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/assetfilters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6038 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/assets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4659 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/beacons.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2356 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/call.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    17283 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2327 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/count.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2336 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    58343 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5037 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4073 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/evpn_topologies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7034 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/guests.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     9142 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1157 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8539 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/location.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    14930 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/maps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5297 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/mxedges.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1184 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/mxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2294 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/networks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6008 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/otherdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5810 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/pcaps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7530 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/psks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5752 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/rfdiags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5737 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/rogues.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3809 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/rrm.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4711 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/rssizones.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2343 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/servicepolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2294 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/services.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6042 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/setting.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2404 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/sites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3837 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/skyatp.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    20771 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/sle.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1970 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/ssr.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    61323 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1707 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1905 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/synthetic_test.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4633 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/uisettings.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4683 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/vbeacons.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2239 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/visits.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2266 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/vpns.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1350 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/wan_client.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4797 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/wan_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5300 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/webhooks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3839 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/wired_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6811 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/wlans.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5279 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/wxrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5936 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/wxtags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4711 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/wxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4599 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/sites/zones.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.479811 mistapi-0.40.1/src/mistapi/api/v1/utils/
--rw-r--r--   0 tmunzer    (502) staff       (20)      511 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/utils/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1072 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/utils/test_telstra.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1184 2023-06-13 20:28:05.000000 mistapi-0.40.1/src/mistapi/api/v1/utils/test_twilio.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    11557 2023-06-07 14:42:24.000000 mistapi-0.40.1/src/mistapi/cli.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-13 20:28:16.326381 mistapi-0.40.1/src/mistapi.egg-info/
--rw-r--r--   0 tmunzer    (502) staff       (20)    11281 2023-06-13 20:28:16.000000 mistapi-0.40.1/src/mistapi.egg-info/PKG-INFO
--rw-r--r--   0 tmunzer    (502) staff       (20)     7781 2023-06-13 20:28:16.000000 mistapi-0.40.1/src/mistapi.egg-info/SOURCES.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)        1 2023-06-13 20:28:16.000000 mistapi-0.40.1/src/mistapi.egg-info/dependency_links.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)       66 2023-06-13 20:28:16.000000 mistapi-0.40.1/src/mistapi.egg-info/requires.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)        8 2023-06-13 20:28:16.000000 mistapi-0.40.1/src/mistapi.egg-info/top_level.txt
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.452839 mistapi-0.40.2/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-01-13 07:55:51.000000 mistapi-0.40.2/LICENSE
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11281 2023-06-19 15:17:39.452971 mistapi-0.40.2/PKG-INFO
+-rw-r--r--   0 tmunzer    (502) staff       (20)    10505 2023-06-13 20:27:38.000000 mistapi-0.40.2/README.md
+-rw-r--r--   0 tmunzer    (502) staff       (20)      976 2023-06-19 15:17:23.000000 mistapi-0.40.2/pyproject.toml
+-rw-r--r--   0 tmunzer    (502) staff       (20)      125 2023-06-19 15:17:39.453633 mistapi-0.40.2/setup.cfg
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.362108 mistapi-0.40.2/src/
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.372845 mistapi-0.40.2/src/mistapi/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7909 2023-04-20 13:57:39.000000 mistapi-0.40.2/src/mistapi/__api_request.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2962 2023-02-21 11:06:36.000000 mistapi-0.40.2/src/mistapi/__api_response.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    21501 2023-06-19 15:16:16.000000 mistapi-0.40.2/src/mistapi/__api_session.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)      635 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2229 2023-02-13 15:54:52.000000 mistapi-0.40.2/src/mistapi/__logger.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.375880 mistapi-0.40.2/src/mistapi/__models/
+-rw-r--r--   0 tmunzer    (502) staff       (20)        0 2023-02-21 08:35:01.000000 mistapi-0.40.2/src/mistapi/__models/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1530 2023-05-30 09:43:55.000000 mistapi-0.40.2/src/mistapi/__models/privilege.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2029 2023-02-09 11:01:08.000000 mistapi-0.40.2/src/mistapi/__pagination.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.376338 mistapi-0.40.2/src/mistapi/api/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      446 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.376655 mistapi-0.40.2/src/mistapi/api/v1/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      869 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.384389 mistapi-0.40.2/src/mistapi/api/v1/const/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1235 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/const/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1729 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/const/alarm_defs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2027 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/const/ap_channels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1730 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/const/ap_led_status.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1713 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/const/applications.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1756 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/const/call_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1770 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/const/client_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1707 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/const/countries.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1402 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/const/default_gateway_config.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1770 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/const/device_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1715 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/const/device_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1729 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/const/insight_metrics.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1712 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/const/languages.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1055 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/const/license_types.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1770 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/const/mxedge_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1715 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/const/mxedge_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1807 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/const/other_device_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1715 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/const/traffic_types.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.384805 mistapi-0.40.2/src/mistapi/api/v1/installer/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/installer/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.388621 mistapi-0.40.2/src/mistapi/api/v1/installer/orgs/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      798 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/installer/orgs/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1968 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/installer/orgs/alarmtemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1968 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/installer/orgs/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7123 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/installer/orgs/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1972 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/installer/orgs/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1947 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/installer/orgs/secpolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1940 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/installer/orgs/sitegroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7487 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/installer/orgs/sites.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.389370 mistapi-0.40.2/src/mistapi/api/v1/installer/sites/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      471 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/installer/sites/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1168 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/installer/sites/optimize.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.390139 mistapi-0.40.2/src/mistapi/api/v1/invite/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/invite/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1099 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/invite/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.392374 mistapi-0.40.2/src/mistapi/api/v1/login/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      584 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/login/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1136 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/login/login.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1145 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/login/lookup.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2628 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/login/oauth.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1155 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/login/two_factor.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.393070 mistapi-0.40.2/src/mistapi/api/v1/logout/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/logout/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)      984 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/logout/logout.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.393830 mistapi-0.40.2/src/mistapi/api/v1/mobile/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/mobile/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1257 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/mobile/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.400606 mistapi-0.40.2/src/mistapi/api/v1/msps/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1104 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/msps/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3887 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/msps/admins.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1250 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/msps/claim.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/msps/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1205 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/msps/inventory.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2667 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/msps/invites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2620 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/msps/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1828 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/msps/logo.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4444 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/msps/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2981 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/msps/msps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/msps/orggroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5244 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/msps/orgs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1660 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/msps/search.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4002 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/msps/ssoroles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5981 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/msps/ssos.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3637 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/msps/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1476 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/msps/suggestion.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3225 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/msps/tickets.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.425587 mistapi-0.40.2/src/mistapi/api/v1/orgs/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3208 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3255 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/admins.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6440 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/alarms.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7576 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/alarmtemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/apitokens.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4730 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/aptemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4762 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/assetfilters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5989 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/assets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2344 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/call.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1709 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/cert.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1250 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/claim.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11397 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1236 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/clone.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1846 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/crl.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7034 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    20091 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4812 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/evpn_topologies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4870 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/gatewaytemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6514 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/guests.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2978 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5034 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/inventory.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2667 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/invites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6927 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/jsi.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2503 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5217 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1434 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/maps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4754 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/mxclusters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    15280 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/mxedges.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/mxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/nacrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4618 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/nactags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/networks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4872 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/networktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1407 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/ocdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2975 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/orgs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8802 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/otherdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1913 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/pma.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4702 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/pskportals.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8274 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/psks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4730 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1316 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/sdkclients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6892 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/sdkinvites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4719 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/sdktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4721 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/secpolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4825 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/servicepolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/services.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    16586 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/setting.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4702 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/sitegroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8619 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/sites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4788 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/sitetemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/ssoroles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8223 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/ssos.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4767 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/ssr.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    32140 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1747 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5449 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/templates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6846 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/tickets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1758 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/troubleshoot.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4541 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/vpns.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1344 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/wan_client.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4779 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/wan_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4646 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/webhooks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3540 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/wired_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7466 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/wlans.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5236 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/wxrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5887 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/wxtags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4674 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/orgs/wxtunnels.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.426705 mistapi-0.40.2/src/mistapi/api/v1/recover/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/recover/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1158 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/recover/recover.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1110 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/recover/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.427858 mistapi-0.40.2/src/mistapi/api/v1/register/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      508 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/register/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1161 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/register/register.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1103 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/register/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.430617 mistapi-0.40.2/src/mistapi/api/v1/self/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      707 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/self/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2916 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/self/apitokens.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2596 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/self/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2015 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/self/oauth.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2109 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/self/self.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/self/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1837 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/self/two_factor.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1756 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/self/update.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.451274 mistapi-0.40.2/src/mistapi/api/v1/sites/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2588 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8657 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/alarms.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2655 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/anomaly.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1861 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/apps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4797 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/assetfilters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6038 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/assets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4659 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/beacons.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2356 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/call.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    17283 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2327 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/count.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2336 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    58343 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5037 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4073 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/evpn_topologies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7034 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/guests.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     9142 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1157 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8539 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/location.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    14930 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/maps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5297 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/mxedges.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1184 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/mxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2294 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/networks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6008 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/otherdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5810 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/pcaps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7530 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/psks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5752 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/rfdiags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5737 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/rogues.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3809 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/rrm.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4711 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/rssizones.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2343 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/servicepolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2294 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/services.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6042 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/setting.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2404 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/sites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3837 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/skyatp.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    20771 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/sle.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1970 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/ssr.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    61323 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1707 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1905 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/synthetic_test.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4633 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/uisettings.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4683 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/vbeacons.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2239 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/visits.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2266 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/vpns.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1350 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/wan_client.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4797 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/wan_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5300 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/webhooks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3839 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/wired_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6811 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/wlans.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5279 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/wxrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5936 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/wxtags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4711 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/wxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4599 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/sites/zones.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.452557 mistapi-0.40.2/src/mistapi/api/v1/utils/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      511 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/utils/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1072 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/utils/test_telstra.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1184 2023-06-19 15:17:23.000000 mistapi-0.40.2/src/mistapi/api/v1/utils/test_twilio.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11952 2023-06-19 15:14:23.000000 mistapi-0.40.2/src/mistapi/cli.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-19 15:17:39.375170 mistapi-0.40.2/src/mistapi.egg-info/
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11281 2023-06-19 15:17:39.000000 mistapi-0.40.2/src/mistapi.egg-info/PKG-INFO
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7781 2023-06-19 15:17:39.000000 mistapi-0.40.2/src/mistapi.egg-info/SOURCES.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)        1 2023-06-19 15:17:39.000000 mistapi-0.40.2/src/mistapi.egg-info/dependency_links.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)       66 2023-06-19 15:17:39.000000 mistapi-0.40.2/src/mistapi.egg-info/requires.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)        8 2023-06-19 15:17:39.000000 mistapi-0.40.2/src/mistapi.egg-info/top_level.txt
```

### Comparing `mistapi-0.40.1/LICENSE` & `mistapi-0.40.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/PKG-INFO` & `mistapi-0.40.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistapi
-Version: 0.40.1
+Version: 0.40.2
 Summary: Python package to simplify the Mist System APIs usage
 Author-email: Thomas Munzer <tmunzer@juniper.net>
 License: MIT
 Project-URL: Source, https://github.com/tmunzer/mistapi_python
 Project-URL: Bug Tracker, https://github.com/tmunzer/mistapi_python/issues
 Keywords: Mist,Juniper,API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mistapi-0.40.1/README.md` & `mistapi-0.40.2/README.md`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/pyproject.toml` & `mistapi-0.40.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mistapi"
-version = "0.40.1"
+version = "0.40.2"
 authors = [{name="Thomas Munzer", email="tmunzer@juniper.net"}]
 description = "Python package to simplify the Mist System APIs usage"
 keywords = ["Mist", "Juniper", "API"]
 license = {text =  "MIT"}
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mistapi-0.40.1/src/mistapi/__api_request.py` & `mistapi-0.40.2/src/mistapi/__api_request.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/__api_response.py` & `mistapi-0.40.2/src/mistapi/__api_response.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/__api_session.py` & `mistapi-0.40.2/src/mistapi/__api_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,24 +160,19 @@
 
         PARAMS
         -----------
         :param str cloud_uri - Mist FQDN to reach ("api.mist.com", "api.eu.mist.com", ...)
         """
         logger.debug(f"apisession:in  > set_cloud")
         self._cloud_uri = None
-        if cloud_uri == "api.mistsys.com":
+        for cloud in clouds:
+            if cloud["host"] == cloud_uri:
                 self._cloud_uri = cloud_uri
                 logger.debug(f"apisession:Mist Cloud configured to {self._cloud_uri}")
                 console.debug(f"Mist Cloud configured to {self._cloud_uri}")
-        else:
-            for cloud in clouds:
-                if cloud["host"] == cloud_uri:
-                    self._cloud_uri = cloud_uri
-                    logger.debug(f"apisession:Mist Cloud configured to {self._cloud_uri}")
-                    console.debug(f"Mist Cloud configured to {self._cloud_uri}")
         if not self._cloud_uri:
             logger.error(f"apisession:{cloud_uri} is not valid")
             console.error(f"{cloud_uri} is not valid")
 
     def get_cloud(self):
         """
         Return the Mist Cloud currently configured
@@ -394,15 +389,15 @@
     def get_authentication_status(self) -> bool:
         """
         RETURN
         -----------
         Return the authentication status.
         """
         logger.debug(f"apisession:in  > get_authentication_status")
-        return self._authenticated or self._apitoken
+        return self._authenticated
 
     def get_api_token(self):
         """
         Retrieve and display the User/Org API Tokens
         """
         logger.debug(f"apisession:in  > list_api_token")
         logger.info(f'apisession:Sending GET request to "/api/v1/self/apitokens"')
```

### Comparing `mistapi-0.40.1/src/mistapi/__init__.py` & `mistapi-0.40.2/src/mistapi/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 '''
 
 from mistapi.__api_session import APISession
 from mistapi import api
 from mistapi import cli
 from mistapi.__pagination import get_next, get_all
 
-__version__ = "0.40.1"
+__version__ = "0.40.2"
 __author__ = "Thomas Munzer <tmunzer@juniper.net>"
```

### Comparing `mistapi-0.40.1/src/mistapi/__logger.py` & `mistapi-0.40.2/src/mistapi/__logger.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/__models/privilege.py` & `mistapi-0.40.2/src/mistapi/__models/privilege.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/__pagination.py` & `mistapi-0.40.2/src/mistapi/__pagination.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/__init__.py` & `mistapi-0.40.2/src/mistapi/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/const/__init__.py` & `mistapi-0.40.2/src/mistapi/api/v1/const/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/const/alarm_defs.py` & `mistapi-0.40.2/src/mistapi/api/v1/const/alarm_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listAlarmDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listAlarmDefinitions")  
 def getAlarmDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listAlarmDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/const/ap_channels.py` & `mistapi-0.40.2/src/mistapi/api/v1/const/ap_channels.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listApChannels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listApChannels")  
 def getApChannels(mist_session:_APISession, country_code:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApChannels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/const/ap_led_status.py` & `mistapi-0.40.2/src/mistapi/api/v1/const/ap_led_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listApLedDefinition")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listApLedDefinition")  
 def getApLedDefinition(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApLedDefinition
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/const/applications.py` & `mistapi-0.40.2/src/mistapi/api/v1/const/applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listApplications")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listApplications")  
 def getApplications(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApplications
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/const/call_events.py` & `mistapi-0.40.2/src/mistapi/api/v1/const/call_events.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listCallEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listCallEventsDefinitions")  
 def getCallEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listCallEventsDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/const/client_events.py` & `mistapi-0.40.2/src/mistapi/api/v1/const/client_events.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listClientEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listClientEventsDefinitions")  
 def getClientEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listClientEventsDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/const/countries.py` & `mistapi-0.40.2/src/mistapi/api/v1/const/countries.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listCountryCodes")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listCountryCodes")  
 def getCountryCodes(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listCountryCodes
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/const/default_gateway_config.py` & `mistapi-0.40.2/src/mistapi/api/v1/const/default_gateway_config.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/const/device_events.py` & `mistapi-0.40.2/src/mistapi/api/v1/const/device_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listDeviceEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listDeviceEventsDefinitions")  
 def getDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listDeviceEventsDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/const/device_models.py` & `mistapi-0.40.2/src/mistapi/api/v1/const/device_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listDeviceModels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listDeviceModels")  
 def getDeviceModels(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listDeviceModels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/const/insight_metrics.py` & `mistapi-0.40.2/src/mistapi/api/v1/const/insight_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listInsightMetrics")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listInsightMetrics")  
 def getInsightMetrics(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInsightMetrics
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/const/languages.py` & `mistapi-0.40.2/src/mistapi/api/v1/const/languages.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteLanguages")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteLanguages")  
 def getSiteLanguages(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteLanguages
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/const/license_types.py` & `mistapi-0.40.2/src/mistapi/api/v1/const/license_types.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/const/mxedge_events.py` & `mistapi-0.40.2/src/mistapi/api/v1/const/mxedge_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMxEdgeEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listMxEdgeEventsDefinitions")  
 def getMxEdgeEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMxEdgeEventsDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/const/mxedge_models.py` & `mistapi-0.40.2/src/mistapi/api/v1/const/mxedge_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMxEdgeModels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listMxEdgeModels")  
 def getMxEdgeModels(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMxEdgeModels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/const/other_device_events.py` & `mistapi-0.40.2/src/mistapi/api/v1/const/other_device_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOtherDeviceEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOtherDeviceEventsDefinitions")  
 def getOtherDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOtherDeviceEventsDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/const/traffic_types.py` & `mistapi-0.40.2/src/mistapi/api/v1/const/traffic_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listTrafficTypes")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listTrafficTypes")  
 def getTrafficTypes(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listTrafficTypes
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/__init__.py` & `mistapi-0.40.2/src/mistapi/api/v1/installer/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/alarmtemplates.py` & `mistapi-0.40.2/src/mistapi/api/v1/installer/orgs/alarmtemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listInstallerAlarmTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listInstallerAlarmTemplates")  
 def getInstallerAlarmTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerAlarmTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/deviceprofiles.py` & `mistapi-0.40.2/src/mistapi/api/v1/installer/orgs/deviceprofiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listInstallerDeviceProfiles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listInstallerDeviceProfiles")  
 def getInstallerDeviceProfiles(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerDeviceProfiles
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/devices.py` & `mistapi-0.40.2/src/mistapi/api/v1/installer/orgs/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listInstallerListOfRenctlyClaimedDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listInstallerListOfRenctlyClaimedDevices")  
 def getInstallerListOfRenctlyClaimedDevices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerListOfRenctlyClaimedDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/rftemplates.py` & `mistapi-0.40.2/src/mistapi/api/v1/installer/orgs/rftemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listInstallerRfTemplatesNames")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listInstallerRfTemplatesNames")  
 def getInstallerRfTemplatesNames(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerRfTemplatesNames
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/secpolicies.py` & `mistapi-0.40.2/src/mistapi/api/v1/installer/orgs/secpolicies.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listInstallerSecPolicies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listInstallerSecPolicies")  
 def getInstallerSecPolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSecPolicies
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/sitegroups.py` & `mistapi-0.40.2/src/mistapi/api/v1/installer/orgs/sitegroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listInstallerSiteGroups")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listInstallerSiteGroups")  
 def getInstallerSiteGroups(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSiteGroups
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/installer/orgs/sites.py` & `mistapi-0.40.2/src/mistapi/api/v1/installer/orgs/sites.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listInstallerSites")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listInstallerSites")  
 def getInstallerSites(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSites
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -78,15 +78,15 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/installer/orgs/{org_id}/sites/{site_name}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listInstallerMaps")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listInstallerMaps")  
 def getInstallerMaps(mist_session:_APISession, org_id:str, site_name:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerMaps
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/installer/sites/optimize.py` & `mistapi-0.40.2/src/mistapi/api/v1/installer/sites/optimize.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/invite/verify.py` & `mistapi-0.40.2/src/mistapi/api/v1/invite/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/login/__init__.py` & `mistapi-0.40.2/src/mistapi/api/v1/login/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/login/login.py` & `mistapi-0.40.2/src/mistapi/api/v1/login/login.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/login/lookup.py` & `mistapi-0.40.2/src/mistapi/api/v1/login/lookup.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/login/oauth.py` & `mistapi-0.40.2/src/mistapi/api/v1/login/oauth.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/login/two_factor.py` & `mistapi-0.40.2/src/mistapi/api/v1/login/two_factor.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/logout/logout.py` & `mistapi-0.40.2/src/mistapi/api/v1/logout/logout.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/mobile/verify.py` & `mistapi-0.40.2/src/mistapi/api/v1/mobile/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/msps/__init__.py` & `mistapi-0.40.2/src/mistapi/api/v1/msps/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/msps/admins.py` & `mistapi-0.40.2/src/mistapi/api/v1/msps/admins.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMspAdmins")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listMspAdmins")  
 def getMspAdmins(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspAdmins
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/msps/claim.py` & `mistapi-0.40.2/src/mistapi/api/v1/msps/claim.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/msps/insights.py` & `mistapi-0.40.2/src/mistapi/api/v1/msps/insights.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/msps/inventory.py` & `mistapi-0.40.2/src/mistapi/api/v1/msps/inventory.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/msps/invites.py` & `mistapi-0.40.2/src/mistapi/api/v1/msps/invites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/msps/licenses.py` & `mistapi-0.40.2/src/mistapi/api/v1/msps/licenses.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMspLicenses")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listMspLicenses")  
 def getMspLicenses(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspLicenses
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/msps/logo.py` & `mistapi-0.40.2/src/mistapi/api/v1/msps/logo.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/msps/logs.py` & `mistapi-0.40.2/src/mistapi/api/v1/msps/logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMspLogs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listMspLogs")  
 def getMspLogs(mist_session:_APISession, msp_id:str, site_id:str=None, admin_name:str=None, message:str=None, sort:any=None, start:int=None, end:int=None, limit:int=100, page:int=1, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspLogs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/msps/msps.py` & `mistapi-0.40.2/src/mistapi/api/v1/msps/msps.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/msps/orggroups.py` & `mistapi-0.40.2/src/mistapi/api/v1/msps/orggroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMspOrgGroups")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listMspOrgGroups")  
 def getMspOrgGroups(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgGroups
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/msps/orgs.py` & `mistapi-0.40.2/src/mistapi/api/v1/msps/orgs.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMspOrgs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listMspOrgs")  
 def getMspOrgs(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/msps/search.py` & `mistapi-0.40.2/src/mistapi/api/v1/msps/search.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/msps/ssoroles.py` & `mistapi-0.40.2/src/mistapi/api/v1/msps/ssoroles.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMspSsoRoles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listMspSsoRoles")  
 def getMspSsoRoles(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspSsoRoles
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/msps/ssos.py` & `mistapi-0.40.2/src/mistapi/api/v1/msps/ssos.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/ssos/{sso_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMspSsoLatestFailures")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listMspSsoLatestFailures")  
 def getMspSsoLatestFailures(mist_session:_APISession, msp_id:str, sso_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspSsoLatestFailures
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/msps/stats.py` & `mistapi-0.40.2/src/mistapi/api/v1/msps/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMspOrgLicenses")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listMspOrgLicenses")  
 def getMspOrgLicenses(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgLicenses
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -53,15 +53,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/stats/licenses"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMspOrgStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listMspOrgStats")  
 def getMspOrgStats(mist_session:_APISession, msp_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/msps/suggestion.py` & `mistapi-0.40.2/src/mistapi/api/v1/msps/suggestion.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/msps/tickets.py` & `mistapi-0.40.2/src/mistapi/api/v1/msps/tickets.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listMspTickets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listMspTickets")  
 def getMspTickets(mist_session:_APISession, msp_id:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspTickets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/__init__.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/admins.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/admins.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgAdmins")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgAdmins")  
 def getOrgAdmins(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAdmins
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/alarms.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/alarms.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/alarmtemplates.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/alarmtemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgAlarmTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgAlarmTemplates")  
 def getOrgAlarmTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAlarmTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -77,15 +77,15 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/alarmtemplates"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgSuppressedAlarms")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgSuppressedAlarms")  
 def getOrgSuppressedAlarms(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSuppressedAlarms
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/apitokens.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/apitokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgApiTokens")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgApiTokens")  
 def getOrgApiTokens(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgApiTokens
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/aptemplates.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/aptemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgAptemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgAptemplates")  
 def getOrgAptemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAptemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/assetfilters.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/assetfilters.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgAssetFilters")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgAssetFilters")  
 def getOrgAssetFilters(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssetFilters
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/assets.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgAssets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgAssets")  
 def getOrgAssets(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/call.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/call.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/cert.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/cert.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/claim.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/claim.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/clients.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/clone.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/clone.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/crl.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/crl.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/deviceprofiles.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/deviceprofiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgDeviceProfiles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgDeviceProfiles")  
 def getOrgDeviceProfiles(mist_session:_APISession, org_id:str, type:str="ap", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDeviceProfiles
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/devices.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgDevices")  
 def getOrgDevices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -279,15 +279,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if limit: query_params["limit"]=limit
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgApsMacs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgApsMacs")  
 def getOrgApsMacs(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgApsMacs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -394,15 +394,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgMultiSitesDevicesUpgrades")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgMultiSitesDevicesUpgrades")  
 def getOrgMultiSitesDevicesUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMultiSitesDevicesUpgrades
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/evpn_topologies.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/evpn_topologies.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgEvpnTopologies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgEvpnTopologies")  
 def getOrgEvpnTopologies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgEvpnTopologies
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/gatewaytemplates.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/gatewaytemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgGatewayTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgGatewayTemplates")  
 def getOrgGatewayTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgGatewayTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/guests.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/guests.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgGuestAuthorizations")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgGuestAuthorizations")  
 def getOrgGuestAuthorizations(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgGuestAuthorizations
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/insights.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/insights.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/inventory.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/inventory.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/invites.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/invites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/jsi.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/jsi.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgJsiDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgJsiDevices")  
 def getOrgJsiDevices(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None, mac:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgJsiDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -146,15 +146,15 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/jsi/devices/{device_mac}/upgrade"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgJsiPastPurchases")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgJsiPastPurchases")  
 def getOrgJsiPastPurchases(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgJsiPastPurchases
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/licenses.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/licenses.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/logs.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgLogs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgLogs")  
 def getOrgLogs(mist_session:_APISession, org_id:str, site_id:str=None, admin_name:str=None, message:str=None, sort:any=None, start:int=None, end:int=None, limit:int=100, page:int=1, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgLogs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/maps.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/maps.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/mxclusters.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/mxclusters.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgMxEdgeClusters")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgMxEdgeClusters")  
 def getOrgMxEdgeClusters(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgeClusters
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/mxedges.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/mxedges.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgMxEdges")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgMxEdges")  
 def getOrgMxEdges(mist_session:_APISession, org_id:str, for_sites:str="any", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdges
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -167,15 +167,15 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges/unassign"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgMxEdgeUpgrades")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgMxEdgeUpgrades")  
 def getOrgMxEdgeUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgeUpgrades
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/mxtunnels.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/mxtunnels.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgMxTunnels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgMxTunnels")  
 def getOrgMxTunnels(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxTunnels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/nacrules.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/nacrules.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgNacRules")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgNacRules")  
 def getOrgNacRules(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNacRules
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/nactags.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/nactags.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgNacTags")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgNacTags")  
 def getOrgNacTags(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNacTags
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/networks.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/networks.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgNetworks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgNetworks")  
 def getOrgNetworks(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNetworks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/networktemplates.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/networktemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgNetworkTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgNetworkTemplates")  
 def getOrgNetworkTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNetworkTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/ocdevices.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/ocdevices.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/orgs.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/orgs.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/otherdevices.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/otherdevices.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgOtherDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgOtherDevices")  
 def getOrgOtherDevices(mist_session:_APISession, org_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgOtherDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/pma.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/pma.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgPmaDashboards")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgPmaDashboards")  
 def getOrgPmaDashboards(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPmaDashboards
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/pskportals.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/pskportals.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgPskPortals")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgPskPortals")  
 def getOrgPskPortals(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPskPortals
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/psks.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/psks.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgPsks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgPsks")  
 def getOrgPsks(mist_session:_APISession, org_id:str, name:str=None, ssid:str=None, role:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPsks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/rftemplates.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/rftemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgRfTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgRfTemplates")  
 def getOrgRfTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgRfTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/sdkclients.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/sdkclients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/sdkinvites.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/sdkinvites.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSdkInvites")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSdkInvites")  
 def getSdkInvites(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSdkInvites
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/sdktemplates.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/sdktemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSdkTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSdkTemplates")  
 def getSdkTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSdkTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/secpolicies.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/secpolicies.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgSecPolicies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgSecPolicies")  
 def getOrgSecPolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSecPolicies
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/servicepolicies.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/servicepolicies.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgServicePolicies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgServicePolicies")  
 def getOrgServicePolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgServicePolicies
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/services.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgServices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgServices")  
 def getOrgServices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgServices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/setting.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/setting.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/sitegroups.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/sitegroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgSiteGroups")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgSiteGroups")  
 def getOrgSiteGroups(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSiteGroups
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/sites.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/sites.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgSites")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgSites")  
 def getOrgSites(mist_session:_APISession, org_id:str, limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSites
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/sitetemplates.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/sitetemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgSiteTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgSiteTemplates")  
 def getOrgSiteTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSiteTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/ssoroles.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/ssoroles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgSsoRoles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgSsoRoles")  
 def getOrgSsoRoles(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsoRoles
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/ssos.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/ssos.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgSsos")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgSsos")  
 def getOrgSsos(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsos
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -146,15 +146,15 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/ssos/{sso_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgSsoLatestFailures")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgSsoLatestFailures")  
 def getOrgSsoLatestFailures(mist_session:_APISession, org_id:str, sso_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsoLatestFailures
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/ssr.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/ssr.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/128routers/register_cmd"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgSsrUpgrades")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgSsrUpgrades")  
 def getOrgSsrUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsrUpgrades
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/stats.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgAssetsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgAssetsStats")  
 def getOrgAssetsStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssetsStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -241,15 +241,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/stats/bgp_peers/search"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgDevicesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgDevicesStats")  
 def getOrgDevicesStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", type:str="ap", status:str="all", site_id:str=None, mac:str=None, evpntopo_id:str=None, evpn_unused:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDevicesStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -334,15 +334,15 @@
     if site_id: query_params["site_id"]=site_id
     if mac: query_params["mac"]=mac
     if evpntopo_id: query_params["evpntopo_id"]=evpntopo_id
     if evpn_unused: query_params["evpn_unused"]=evpn_unused
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgMxEdgesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgMxEdgesStats")  
 def getOrgMxEdgesStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", for_site:str="false") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgesStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/subscriptions.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/subscriptions.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/templates.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgTemplates")  
 def getOrgTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/tickets.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/tickets.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgTickets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgTickets")  
 def getOrgTickets(mist_session:_APISession, org_id:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgTickets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/troubleshoot.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/troubleshoot.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/vpns.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/vpns.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgsVpns")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgsVpns")  
 def getOrgsVpns(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgsVpns
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/wan_client.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/wan_client.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/wan_clients.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/wan_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/webhooks.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/webhooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgWebhooks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgWebhooks")  
 def getOrgWebhooks(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWebhooks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/wired_clients.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/wired_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/wlans.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/wlans.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgWlans")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgWlans")  
 def getOrgWlans(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWlans
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/wxrules.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/wxrules.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgWxRules")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgWxRules")  
 def getOrgWxRules(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxRules
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/wxtags.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/wxtags.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgWxTags")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgWxTags")  
 def getOrgWxTags(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxTags
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/orgs/wxtunnels.py` & `mistapi-0.40.2/src/mistapi/api/v1/orgs/wxtunnels.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listOrgWxTunnels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listOrgWxTunnels")  
 def getOrgWxTunnels(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxTunnels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/recover/recover.py` & `mistapi-0.40.2/src/mistapi/api/v1/recover/recover.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/recover/verify.py` & `mistapi-0.40.2/src/mistapi/api/v1/recover/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/register/register.py` & `mistapi-0.40.2/src/mistapi/api/v1/register/register.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/register/verify.py` & `mistapi-0.40.2/src/mistapi/api/v1/register/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/self/__init__.py` & `mistapi-0.40.2/src/mistapi/api/v1/self/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/self/apitokens.py` & `mistapi-0.40.2/src/mistapi/api/v1/self/apitokens.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listApiTokens")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listApiTokens")  
 def getApiTokens(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApiTokens
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/self/logs.py` & `mistapi-0.40.2/src/mistapi/api/v1/self/logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSelfAuditLogs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSelfAuditLogs")  
 def getSelfAuditLogs(mist_session:_APISession, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSelfAuditLogs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/self/oauth.py` & `mistapi-0.40.2/src/mistapi/api/v1/self/oauth.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/self/self.py` & `mistapi-0.40.2/src/mistapi/api/v1/self/self.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/self/subscriptions.py` & `mistapi-0.40.2/src/mistapi/api/v1/self/subscriptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listAlarmSubscriptions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listAlarmSubscriptions")  
 def getAlarmSubscriptions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listAlarmSubscriptions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/self/two_factor.py` & `mistapi-0.40.2/src/mistapi/api/v1/self/two_factor.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/self/update.py` & `mistapi-0.40.2/src/mistapi/api/v1/self/update.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/__init__.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/alarms.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/alarms.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/anomaly.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/anomaly.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/apps.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/synthetic_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,50 +10,52 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteApps")  
-def getSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
+def getSiteSyntheticTestStatus(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteApps
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSyntheticTestStatus
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/apps"
+    uri = f"/api/v1/sites/{site_id}/synthetic_test"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
+def triggerSiteSyntheticTest(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteApps
+    API doc: https://doc.mist-lab.fr/#operation/triggerSiteSyntheticTest
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/apps"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/sites/{site_id}/synthetic_test"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/assetfilters.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/assetfilters.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteAssetFilters")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteAssetFilters")  
 def getSiteAssetFilters(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssetFilters
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/assets.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteAssets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteAssets")  
 def getSiteAssets(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/beacons.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/beacons.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteBeacons")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteBeacons")  
 def getSiteBeacons(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteBeacons
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/call.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/call.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/clients.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/count.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/count.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/deviceprofiles.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/deviceprofiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteDeviceProfilesDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteDeviceProfilesDerived")  
 def getSiteDeviceProfilesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDeviceProfilesDerived
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/devices.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteDevices")  
 def getSiteDevices(mist_session:_APISession, site_id:str, type:str="ap", name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -673,15 +673,15 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/upgrade/{upgrade_id}/cancel"
     resp = mist_session.mist_post(uri=uri)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteAvailableDeviceVersions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteAvailableDeviceVersions")  
 def getSiteAvailableDeviceVersions(mist_session:_APISession, site_id:str, type:str="ap", model:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAvailableDeviceVersions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/events.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/events.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/evpn_topologies.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/evpn_topologies.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/guests.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/guests.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteAllGuestAuthorizations")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteAllGuestAuthorizations")  
 def getSiteAllGuestAuthorizations(mist_session:_APISession, site_id:str, wlan_id:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAllGuestAuthorizations
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/insights.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/insights.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if interval: query_params["interval"]=interval
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteRogueAPs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteRogueAPs")  
 def getSiteRogueAPs(mist_session:_APISession, site_id:str, type:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d", interval:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRogueAPs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -159,15 +159,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if interval: query_params["interval"]=interval
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteRogueClients")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteRogueClients")  
 def getSiteRogueClients(mist_session:_APISession, site_id:str, limit:int=100, start:int=None, end:int=None, duration:str="1d", interval:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRogueClients
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/licenses.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/licenses.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/location.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/location.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/maps.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/maps.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteMaps")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteMaps")  
 def getSiteMaps(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMaps
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/mxedges.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/mxedges.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteMxEdges")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteMxEdges")  
 def getSiteMxEdges(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMxEdges
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/mxtunnels.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/mxtunnels.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/networks.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteNetworksDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteNetworksDerived")  
 def getSiteNetworksDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteNetworksDerived
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/otherdevices.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/otherdevices.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteOtherDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteOtherDevices")  
 def getSiteOtherDevices(mist_session:_APISession, site_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteOtherDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/pcaps.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/pcaps.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSitePacketCaptures")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSitePacketCaptures")  
 def getSitePacketCaptures(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", client_mac:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSitePacketCaptures
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/psks.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/psks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSitePsks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSitePsks")  
 def getSitePsks(mist_session:_APISession, site_id:str, ssid:str=None, role:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSitePsks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/rfdiags.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/rfdiags.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/rogues.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/rogues.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/rrm.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/rrm.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/rssizones.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/rssizones.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteRssiZones")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteRssiZones")  
 def getSiteRssiZones(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRssiZones
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/servicepolicies.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/servicepolicies.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteServicePoliciesDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteServicePoliciesDerived")  
 def getSiteServicePoliciesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteServicePoliciesDerived
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/services.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteServicesDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteServicesDerived")  
 def getSiteServicesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteServicesDerived
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/setting.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/setting.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/sites.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/sites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/skyatp.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/skyatp.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/sle.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/sle.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/ssr.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/ssr.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/stats.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     if distinct: query_params["distinct"]=distinct
     if device_mac: query_params["device_mac"]=device_mac
     if app: query_params["app"]=app
     if wired: query_params["wired"]=wired
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteAssetsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteAssetsStats")  
 def getSiteAssetsStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssetsStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -248,15 +248,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteBeaconsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteBeaconsStats")  
 def getSiteBeaconsStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteBeaconsStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -436,15 +436,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteWirelessClientsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteWirelessClientsStats")  
 def getSiteWirelessClientsStats(mist_session:_APISession, site_id:str, wired:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWirelessClientsStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -516,15 +516,15 @@
     """
     uri = f"/api/v1/sites/{site_id}/stats/clients/{client_mac}"
     query_params={}
     if wired: query_params["wired"]=wired
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteDevicesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteDevicesStats")  
 def getSiteDevicesStats(mist_session:_APISession, site_id:str, type:str="ap", status:str="all", page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDevicesStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -625,15 +625,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/devices/{device_id}/clients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteDiscoveredAssets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteDiscoveredAssets")  
 def getSiteDiscoveredAssets(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDiscoveredAssets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -972,15 +972,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/maps/{map_id}/sdkclients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteUnconnectedClientStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteUnconnectedClientStats")  
 def getSiteUnconnectedClientStats(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteUnconnectedClientStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -1017,15 +1017,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/maps/{map_id}/unconnected_clients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteMxEdgesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteMxEdgesStats")  
 def getSiteMxEdgesStats(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMxEdgesStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -1519,15 +1519,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/wxrules"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteZonesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteZonesStats")  
 def getSiteZonesStats(mist_session:_APISession, site_id:str, map_id:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteZonesStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/subscriptions.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/subscriptions.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/synthetic_test.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/wan_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,52 +10,33 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getSiteSyntheticTestStatus(mist_session:_APISession, site_id:str) -> _APIResponse:
+def countSiteWanClientEvents(mist_session:_APISession, site_id:str, distinct:str="type") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteSyntheticTestStatus
+    API doc: https://doc.mist-lab.fr/#operation/countSiteWanClientEvents
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/synthetic_test"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def triggerSiteSyntheticTest(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/triggerSiteSyntheticTest
-    
-    PARAMS
-    -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str site_id        
-    
-    BODY PARAMS
-    -----------
-    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    QUERY PARAMS
+    ------------
+    :param str distinct(type, hostname, ip, mfg, mac)        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/synthetic_test"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/wan_client/events/count"
+    query_params={}
+    if distinct: query_params["distinct"]=distinct
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/uisettings.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/uisettings.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/vbeacons.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/vbeacons.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteVBeacons")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteVBeacons")  
 def getSiteVBeacons(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteVBeacons
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/visits.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/visits.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/vpns.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/vpns.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteVpnsDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteVpnsDerived")  
 def getSiteVpnsDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteVpnsDerived
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/wan_clients.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/wan_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/webhooks.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/webhooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteWebhooks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteWebhooks")  
 def getSiteWebhooks(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWebhooks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/wired_clients.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/wired_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/wlans.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/wlans.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteWlans")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteWlans")  
 def getSiteWlans(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWlans
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/wxrules.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/wxrules.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteWxRules")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteWxRules")  
 def getSiteWxRules(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWxRules
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/wxtags.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/wxtags.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteWxTags")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteWxTags")  
 def getSiteWxTags(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWxTags
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/wxtunnels.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/wxtunnels.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteWxTunnels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteWxTunnels")  
 def getSiteWxTunnels(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWxTunnels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/sites/zones.py` & `mistapi-0.40.2/src/mistapi/api/v1/sites/zones.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.1", details="function replaced with listSiteZones")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.40.2", details="function replaced with listSiteZones")  
 def getSiteZones(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteZones
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/utils/test_telstra.py` & `mistapi-0.40.2/src/mistapi/api/v1/utils/test_telstra.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/api/v1/utils/test_twilio.py` & `mistapi-0.40.2/src/mistapi/api/v1/utils/test_twilio.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.40.1/src/mistapi/cli.py` & `mistapi-0.40.2/src/mistapi/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     This package is licensed under the MIT License.
 
 --------------------------------------------------------------------------------
 This module is providing some functions to simplify Mist API use.
 """
 
 import mistapi as mistapi
+from mistapi.__logger import console
 import sys
 import json
 from tabulate import tabulate
 
 
 ###########################################
 def _search_org(orgs, org_id):
@@ -33,14 +34,25 @@
         if val_int >= 0 and val_int <= val_max:
             return val_int
         else:
             return -1
     except:
         return -2
 
+###########################################
+#### DECORATOR
+def is_authenticated(func):
+    def wrapper(*args, **kwargs):
+        mist_session = args[0]
+        if mist_session.get_authentication_status():
+            return func(*args, **kwargs)
+        else:
+            console.critical("Not authenticated... Exiting...")
+            console.critical("Please une the \"login()\" function first...")            
+    return wrapper
 
 ###########################################
 #### CLI SELECTIONS
 def _forge_privileges(mist_session: mistapi.APISession, msp_id: str):
     """
     Function to generate user privileges for Orgs belonging to a MSP Account
 
@@ -56,62 +68,58 @@
     resp = mistapi.api.v1.msps.orgs.listMspOrgs(mist_session, msp_id)
     orgs = mistapi.get_all(mist_session, resp)
     custom_privileges = []
     for org in orgs:
         custom_privileges.append(mist_session.get_privilege_by_org_id(org["id"]))
     return custom_privileges
 
-
+@is_authenticated
 def _select_msp(mist_session: mistapi.APISession) -> list:
     """
     Function to list all the Mist MSPs allowed for the current user
     and ask to pick one. Return the list org ORG privileges based
     on the user selection
 
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
 
     RETURN
     -----------
     :return list - List of ORG privileges
     """
-    msp_accounts = [
-        priv for priv in mist_session.privileges if priv.get("scope") == "msp"
-    ]
+    msp_accounts = [ priv for priv in mist_session.privileges if priv.get("scope") == "msp" ]
     if len(msp_accounts) == 0:
         return mist_session.privileges
     else:
         msp_accounts = sorted(msp_accounts, key=lambda x: x["name"].lower())
         while True:
             i = -1
             print("\r\nAvailable MSP Accounts:")
             for privilege in msp_accounts:
                 i += 1
                 print(f"{i}) {privilege['name']} (id: {privilege['msp_id']})")
-            print()
-            print("n) Non-MSP Orgs")
-            print()
+
             resp = input(
-                f'\r\nSelect the MSP Account to use (0 to {i}, "n" to access Orgs not attached to an MSP Account, or "q" to quit): '
+                f'\r\nSelect the MSP Account to use (0 to {i}, "n" for None, or "q" to quit): '
             )
             if resp == "q":
                 sys.exit(0)
             elif resp.lower() == "n":
                 return [priv for priv in mist_session.privileges if not priv.get("msp_id")]
             else:
                 tested_val = _test_choice(resp, i)
                 if tested_val >= 0:
                     return _forge_privileges(mist_session, msp_accounts[tested_val]["msp_id"])
                 elif tested_val == -1:
                     print(f"{resp} is not part of the possibilities.")
                 elif tested_val == -2:
                     print("Only numbers are allowed.")
 
-
+@is_authenticated
 def select_org(mist_session: mistapi.APISession, allow_many=False) -> list:
     """
     Function to list all the Mist Orgs allowed for the current user
     and ask to pick one or many. Return the Org ID(s) of the selected
     org(s)
 
     PARAMS
@@ -186,15 +194,15 @@
                     selection_validated = False
                 if tested_val == -2:
                     print("Only numbers are allowed.")
                     selection_validated = False
             if selection_validated:
                 return resp_ids
 
-
+@is_authenticated
 def select_site(
     mist_session: mistapi.APISession, org_id=None, allow_many=False
 ) -> list:
     """
     Function to list all the Sites from a Mist Org and ask user to pick one
     or many. Return the Site ID(s) of the selected site(s)
```

### Comparing `mistapi-0.40.1/src/mistapi.egg-info/PKG-INFO` & `mistapi-0.40.2/src/mistapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistapi
-Version: 0.40.1
+Version: 0.40.2
 Summary: Python package to simplify the Mist System APIs usage
 Author-email: Thomas Munzer <tmunzer@juniper.net>
 License: MIT
 Project-URL: Source, https://github.com/tmunzer/mistapi_python
 Project-URL: Bug Tracker, https://github.com/tmunzer/mistapi_python/issues
 Keywords: Mist,Juniper,API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mistapi-0.40.1/src/mistapi.egg-info/SOURCES.txt` & `mistapi-0.40.2/src/mistapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

