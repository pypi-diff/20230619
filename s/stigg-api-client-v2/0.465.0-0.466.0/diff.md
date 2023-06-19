# Comparing `tmp/stigg_api_client_v2-0.465.0.tar.gz` & `tmp/stigg_api_client_v2-0.466.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.465.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.466.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.465.0.tar` & `stigg_api_client_v2-0.466.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0     1644 2023-06-13 13:12:55.666973 stigg_api_client_v2-0.465.0/README.md
--rw-r--r--   0        0        0      653 2023-06-13 13:13:34.703776 stigg_api_client_v2-0.465.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-06-13 13:12:55.666973 stigg_api_client_v2-0.465.0/stigg/__init__.py
--rw-r--r--   0        0        0      363 2023-06-13 13:12:55.666973 stigg_api_client_v2-0.465.0/stigg/client.py
--rw-r--r--   0        0        0    39351 2023-06-13 13:13:32.947743 stigg_api_client_v2-0.465.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0     7303 2023-06-13 13:13:32.583736 stigg_api_client_v2-0.465.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0     1951 2023-06-13 13:13:32.583736 stigg_api_client_v2-0.465.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-06-13 13:13:31.639711 stigg_api_client_v2-0.465.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-06-13 13:13:31.655712 stigg_api_client_v2-0.465.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    69337 2023-06-13 13:13:32.795740 stigg_api_client_v2-0.465.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-06-13 13:13:31.679713 stigg_api_client_v2-0.465.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0      541 2023-06-13 13:13:31.759715 stigg_api_client_v2-0.465.0/stigg/generated/entitlements_updated.py
--rw-r--r--   0        0        0    23730 2023-06-13 13:13:29.299646 stigg_api_client_v2-0.465.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-06-13 13:13:31.643712 stigg_api_client_v2-0.465.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-06-13 13:13:31.651712 stigg_api_client_v2-0.465.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-06-13 13:13:32.583736 stigg_api_client_v2-0.465.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    53088 2023-06-13 13:13:32.583736 stigg_api_client_v2-0.465.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-06-13 13:13:31.699713 stigg_api_client_v2-0.465.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-06-13 13:13:31.707713 stigg_api_client_v2-0.465.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-06-13 13:13:31.691713 stigg_api_client_v2-0.465.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-06-13 13:13:31.743714 stigg_api_client_v2-0.465.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-06-13 13:13:31.719714 stigg_api_client_v2-0.465.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-06-13 13:13:31.715714 stigg_api_client_v2-0.465.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-06-13 13:13:31.751715 stigg_api_client_v2-0.465.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-06-13 13:13:31.711713 stigg_api_client_v2-0.465.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-06-13 13:13:31.727714 stigg_api_client_v2-0.465.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-06-13 13:13:31.735714 stigg_api_client_v2-0.465.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-06-13 13:13:31.607711 stigg_api_client_v2-0.465.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-06-13 13:13:31.603711 stigg_api_client_v2-0.465.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-06-13 13:13:31.627711 stigg_api_client_v2-0.465.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   125303 2023-06-13 13:13:31.583710 stigg_api_client_v2-0.465.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-06-13 13:13:31.687713 stigg_api_client_v2-0.465.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-06-13 13:13:31.595710 stigg_api_client_v2-0.465.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-06-13 13:13:31.623711 stigg_api_client_v2-0.465.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-06-13 13:13:31.671712 stigg_api_client_v2-0.465.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-06-13 13:13:31.667712 stigg_api_client_v2-0.465.0/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-06-13 13:13:31.663712 stigg_api_client_v2-0.465.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-06-13 13:13:32.587736 stigg_api_client_v2-0.465.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-06-13 13:13:31.611711 stigg_api_client_v2-0.465.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-06-13 13:13:31.631711 stigg_api_client_v2-0.465.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      451 2023-06-13 13:13:31.763715 stigg_api_client_v2-0.465.0/stigg/generated/usage_updated.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.465.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-06-19 12:32:55.301117 stigg_api_client_v2-0.466.0/README.md
+-rw-r--r--   0        0        0      653 2023-06-19 12:33:40.768710 stigg_api_client_v2-0.466.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-06-19 12:32:55.301117 stigg_api_client_v2-0.466.0/stigg/__init__.py
+-rw-r--r--   0        0        0      363 2023-06-19 12:32:55.301117 stigg_api_client_v2-0.466.0/stigg/client.py
+-rw-r--r--   0        0        0    39611 2023-06-19 12:33:39.148727 stigg_api_client_v2-0.466.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0     7303 2023-06-19 12:33:38.608733 stigg_api_client_v2-0.466.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0     1951 2023-06-19 12:33:38.608733 stigg_api_client_v2-0.466.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-06-19 12:33:37.828741 stigg_api_client_v2-0.466.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-06-19 12:33:37.848740 stigg_api_client_v2-0.466.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    70260 2023-06-19 12:33:38.924729 stigg_api_client_v2-0.466.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-06-19 12:33:37.872740 stigg_api_client_v2-0.466.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0      541 2023-06-19 12:33:37.956739 stigg_api_client_v2-0.466.0/stigg/generated/entitlements_updated.py
+-rw-r--r--   0        0        0    23730 2023-06-19 12:33:35.640763 stigg_api_client_v2-0.466.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-06-19 12:33:37.836741 stigg_api_client_v2-0.466.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-06-19 12:33:37.840741 stigg_api_client_v2-0.466.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-06-19 12:33:38.608733 stigg_api_client_v2-0.466.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    53605 2023-06-19 12:33:38.608733 stigg_api_client_v2-0.466.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-06-19 12:33:37.892740 stigg_api_client_v2-0.466.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-06-19 12:33:37.900740 stigg_api_client_v2-0.466.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-06-19 12:33:37.884740 stigg_api_client_v2-0.466.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-06-19 12:33:37.936740 stigg_api_client_v2-0.466.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-06-19 12:33:37.916740 stigg_api_client_v2-0.466.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-06-19 12:33:37.908740 stigg_api_client_v2-0.466.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-06-19 12:33:37.948739 stigg_api_client_v2-0.466.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-06-19 12:33:37.904740 stigg_api_client_v2-0.466.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-06-19 12:33:37.920740 stigg_api_client_v2-0.466.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-06-19 12:33:37.932740 stigg_api_client_v2-0.466.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-06-19 12:33:37.796741 stigg_api_client_v2-0.466.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-06-19 12:33:37.792741 stigg_api_client_v2-0.466.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-06-19 12:33:37.816741 stigg_api_client_v2-0.466.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   125303 2023-06-19 12:33:37.776741 stigg_api_client_v2-0.466.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-06-19 12:33:37.876740 stigg_api_client_v2-0.466.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-06-19 12:33:37.784741 stigg_api_client_v2-0.466.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-06-19 12:33:37.812741 stigg_api_client_v2-0.466.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-06-19 12:33:37.864740 stigg_api_client_v2-0.466.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-06-19 12:33:37.860740 stigg_api_client_v2-0.466.0/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-06-19 12:33:37.856740 stigg_api_client_v2-0.466.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-06-19 12:33:38.716731 stigg_api_client_v2-0.466.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-06-19 12:33:37.800741 stigg_api_client_v2-0.466.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-06-19 12:33:37.824741 stigg_api_client_v2-0.466.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-06-19 12:33:37.952739 stigg_api_client_v2-0.466.0/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0      451 2023-06-19 12:33:37.964739 stigg_api_client_v2-0.466.0/stigg/generated/usage_updated.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.466.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.465.0/README.md` & `stigg_api_client_v2-0.466.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.465.0/pyproject.toml` & `stigg_api_client_v2-0.466.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stigg-api-client-v2"
-version = "0.465.0"
+version = "0.466.0"
 description = ""
 authors = ["Stigg <support@stigg.io>"]
 readme = "README.md"
 packages = [{ include = "stigg" }]
 include = ["stigg/generated/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.466.0/stigg/generated/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 
 from .async_base_client import AsyncBaseClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
     CancelSubscriptionCancelSubscription,
 )
@@ -283,14 +283,16 @@
     TotalPriceFragmentSubTotal,
     TotalPriceFragmentTotal,
     TypographyConfigurationFragment,
     TypographyConfigurationFragmentBody,
     TypographyConfigurationFragmentH1,
     TypographyConfigurationFragmentH2,
     TypographyConfigurationFragmentH3,
+    UsageHistoryFragment,
+    UsageHistoryFragmentUsageMeasurements,
     UsageUpdatedFragment,
 )
 from .get_active_subscriptions import (
     GetActiveSubscriptions,
     GetActiveSubscriptionsGetActiveSubscriptions,
 )
 from .get_coupons import (
@@ -598,14 +600,15 @@
 from .report_event import ReportEvent
 from .report_usage import ReportUsage, ReportUsageCreateUsageMeasurement
 from .update_customer import UpdateCustomer, UpdateCustomerUpdateCustomer
 from .update_subscription import (
     UpdateSubscription,
     UpdateSubscriptionUpdateSubscription,
 )
+from .usage_history import UsageHistory, UsageHistoryUsageHistory
 from .usage_updated import UsageUpdated, UsageUpdatedUsageUpdated
 
 __all__ = [
     "AccessDeniedReason",
     "AccountStatus",
     "AddCompatibleAddonsToPlanInput",
     "AddonCreateInput",
@@ -1155,15 +1158,19 @@
     "UpdateSubscription",
     "UpdateSubscriptionEntitlementInput",
     "UpdateSubscriptionInput",
     "UpdateSubscriptionUpdateSubscription",
     "UpdateUserInput",
     "UsageEventReportInput",
     "UsageEventsReportInput",
+    "UsageHistory",
+    "UsageHistoryFragment",
+    "UsageHistoryFragmentUsageMeasurements",
     "UsageHistoryInput",
+    "UsageHistoryUsageHistory",
     "UsageMeasurementCreateInput",
     "UsageMeasurementFilter",
     "UsageMeasurementFilterCustomerFilter",
     "UsageMeasurementFilterFeatureFilter",
     "UsageMeasurementSort",
     "UsageMeasurementSortFields",
     "UsageUpdateBehavior",
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.466.0/stigg/generated/async_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.466.0/stigg/generated/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.466.0/stigg/generated/cancel_subscription.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/client.py` & `stigg_api_client_v2-0.466.0/stigg/generated/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 # Source: operations.graphql
 
 from typing import AsyncIterator
 
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
@@ -41,24 +41,26 @@
     SubscriptionCancellationInput,
     SubscriptionInput,
     SubscriptionMigrationInput,
     SubscriptionUpdateScheduleCancellationInput,
     UpdateCustomerInput,
     UpdateSubscriptionInput,
     UsageEventsReportInput,
+    UsageHistoryInput,
     UsageMeasurementCreateInput,
 )
 from .migrate_subscription_to_latest import MigrateSubscriptionToLatest
 from .provision_customer import ProvisionCustomer
 from .provision_subscription import ProvisionSubscription
 from .report_entitlement_check_requested import ReportEntitlementCheckRequested
 from .report_event import ReportEvent
 from .report_usage import ReportUsage
 from .update_customer import UpdateCustomer
 from .update_subscription import UpdateSubscription
+from .usage_history import UsageHistory
 from .usage_updated import UsageUpdated
 
 
 def gql(q: str) -> str:
     return q
 
 
@@ -2318,14 +2320,41 @@
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return GetMockPaywall.parse_obj(data)
 
+    async def usage_history(
+        self, usage_history_input: UsageHistoryInput
+    ) -> UsageHistory:
+        query = gql(
+            """
+            query UsageHistory($usageHistoryInput: UsageHistoryInput!) {
+              usageHistory(usageHistoryInput: $usageHistoryInput) {
+                ...UsageHistoryFragment
+              }
+            }
+
+            fragment UsageHistoryFragment on UsageHistory {
+              startDate
+              endDate
+              usageMeasurements {
+                date
+                value
+                isResetPoint
+              }
+            }
+            """
+        )
+        variables: dict[str, object] = {"usageHistoryInput": usage_history_input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return UsageHistory.parse_obj(data)
+
     async def entitlements_updated(self) -> AsyncIterator[EntitlementsUpdated]:
         query = gql(
             """
             subscription EntitlementsUpdated {
               entitlementsUpdated {
                 ...EntitlementsUpdatedPayload
               }
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.466.0/stigg/generated/update_subscription.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
 
 
-class CreateSubscription(BaseModel):
-    create_subscription: "CreateSubscriptionCreateSubscription" = Field(
-        alias="createSubscription"
+class UpdateSubscription(BaseModel):
+    update_subscription: "UpdateSubscriptionUpdateSubscription" = Field(
+        alias="updateSubscription"
     )
 
 
-class CreateSubscriptionCreateSubscription(SlimSubscriptionFragment):
+class UpdateSubscriptionUpdateSubscription(SlimSubscriptionFragment):
     pass
 
 
-CreateSubscription.update_forward_refs()
-CreateSubscriptionCreateSubscription.update_forward_refs()
+UpdateSubscription.update_forward_refs()
+UpdateSubscriptionUpdateSubscription.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/entitlements_updated.py` & `stigg_api_client_v2-0.466.0/stigg/generated/entitlements_updated.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import EntitlementsUpdatedPayload
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.466.0/stigg/generated/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerNotFound = "CustomerNotFound"
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.466.0/stigg/generated/estimate_subscription.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.466.0/stigg/generated/estimate_subscription_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.466.0/stigg/generated/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.466.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -124,25 +124,14 @@
     status: SyncStatus
 
 
 class CouponFragmentCustomers(BaseModel):
     id: str
 
 
-class SlimCustomerFragment(BaseModel):
-    id: str
-    name: Optional[str]
-    email: Optional[str]
-    created_at: Optional[Any] = Field(alias="createdAt")
-    updated_at: Any = Field(alias="updatedAt")
-    ref_id: str = Field(alias="refId")
-    billing_id: Optional[str] = Field(alias="billingId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class PromotionalEntitlementFragment(BaseModel):
     status: PromotionalEntitlementStatus
     usage_limit: Optional[float] = Field(alias="usageLimit")
     feature_id: str = Field(alias="featureId")
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
     end_date: Optional[Any] = Field(alias="endDate")
@@ -157,14 +146,25 @@
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     ref_id: str = Field(alias="refId")
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
 
 
+class SlimCustomerFragment(BaseModel):
+    id: str
+    name: Optional[str]
+    email: Optional[str]
+    created_at: Optional[Any] = Field(alias="createdAt")
+    updated_at: Any = Field(alias="updatedAt")
+    ref_id: str = Field(alias="refId")
+    billing_id: Optional[str] = Field(alias="billingId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class CustomerFragment(SlimCustomerFragment):
     has_payment_method: bool = Field(alias="hasPaymentMethod")
     has_active_subscription: bool = Field(alias="hasActiveSubscription")
     default_payment_expiration_month: Optional[int] = Field(
         alias="defaultPaymentExpirationMonth"
     )
     default_payment_expiration_year: Optional[int] = Field(
@@ -341,14 +341,21 @@
     end_date: Optional[Any] = Field(alias="endDate")
 
 
 class CustomerResourceFragment(BaseModel):
     resource_id: str = Field(alias="resourceId")
 
 
+class CustomerPortalSubscriptionAddon(BaseModel):
+    addon_id: str = Field(alias="addonId")
+    description: Optional[str]
+    display_name: str = Field(alias="displayName")
+    quantity: int
+
+
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional[
@@ -392,21 +399,14 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
-class CustomerPortalSubscriptionAddon(BaseModel):
-    addon_id: str = Field(alias="addonId")
-    description: Optional[str]
-    display_name: str = Field(alias="displayName")
-    quantity: int
-
-
 class CustomerPortalSubscriptionFragment(BaseModel):
     subscription_id: str = Field(alias="subscriptionId")
     plan_name: str = Field(alias="planName")
     pricing: "CustomerPortalSubscriptionFragmentPricing"
     status: SubscriptionStatus
     trial_remaining_days: Optional[int] = Field(alias="trialRemainingDays")
     billing_period_range: Optional[
@@ -532,14 +532,65 @@
 
 
 class TotalPriceFragmentTotal(BaseModel):
     amount: float
     currency: Currency
 
 
+class SubscriptionScheduledUpdateData(BaseModel):
+    subscription_schedule_type: SubscriptionScheduleType = Field(
+        alias="subscriptionScheduleType"
+    )
+    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
+    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
+    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
+        alias="targetPackage"
+    )
+    schedule_variables: Optional[
+        Annotated[
+            Union[
+                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
+            ],
+            Field(discriminator="typename__"),
+        ]
+    ] = Field(alias="scheduleVariables")
+
+
+class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
+    id: str
+    ref_id: str = Field(alias="refId")
+    display_name: str = Field(alias="displayName")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
+    BaseModel
+):
+    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
+    BaseModel
+):
+    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
+    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
+    BaseModel
+):
+    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
+    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
+    feature_id: Optional[str] = Field(alias="featureId")
+
+
 class ProductFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: Optional[str] = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     product_settings: "ProductFragmentProductSettings" = Field(alias="productSettings")
 
@@ -604,65 +655,14 @@
 
 
 class PlanFragmentDefaultTrialConfig(BaseModel):
     duration: float
     units: TrialPeriodUnits
 
 
-class SubscriptionScheduledUpdateData(BaseModel):
-    subscription_schedule_type: SubscriptionScheduleType = Field(
-        alias="subscriptionScheduleType"
-    )
-    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
-    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
-    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
-        alias="targetPackage"
-    )
-    schedule_variables: Optional[
-        Annotated[
-            Union[
-                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
-            ],
-            Field(discriminator="typename__"),
-        ]
-    ] = Field(alias="scheduleVariables")
-
-
-class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
-    id: str
-    ref_id: str = Field(alias="refId")
-    display_name: str = Field(alias="displayName")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
-    BaseModel
-):
-    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
-    BaseModel
-):
-    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
-    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
-    BaseModel
-):
-    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
-    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
-    feature_id: Optional[str] = Field(alias="featureId")
-
-
 class SubscriptionFragment(BaseModel):
     id: str
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
     trial_end_date: Optional[Any] = Field(alias="trialEndDate")
     cancellation_date: Optional[Any] = Field(alias="cancellationDate")
     effective_end_date: Optional[Any] = Field(alias="effectiveEndDate")
@@ -813,34 +813,14 @@
 class LayoutConfigurationFragment(BaseModel):
     alignment: Optional[Alignment]
     plan_width: Optional[float] = Field(alias="planWidth")
     plan_margin: Optional[float] = Field(alias="planMargin")
     plan_padding: Optional[float] = Field(alias="planPadding")
 
 
-class MockPaywallPackageEntitlementFragment(BaseModel):
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
-    display_name_override: Optional[str] = Field(alias="displayNameOverride")
-    feature: Optional["MockPaywallPackageEntitlementFragmentFeature"]
-
-
-class MockPaywallPackageEntitlementFragmentFeature(BaseModel):
-    feature_type: FeatureType = Field(alias="featureType")
-    meter_type: Optional[MeterType] = Field(alias="meterType")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-    display_name: str = Field(alias="displayName")
-    description: Optional[str]
-    ref_id: str = Field(alias="refId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class MockPaywallPriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -855,14 +835,34 @@
 
 class MockPaywallPriceFragmentFeature(BaseModel):
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
 
 
+class MockPaywallPackageEntitlementFragment(BaseModel):
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
+    display_name_override: Optional[str] = Field(alias="displayNameOverride")
+    feature: Optional["MockPaywallPackageEntitlementFragmentFeature"]
+
+
+class MockPaywallPackageEntitlementFragmentFeature(BaseModel):
+    feature_type: FeatureType = Field(alias="featureType")
+    meter_type: Optional[MeterType] = Field(alias="meterType")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    display_name: str = Field(alias="displayName")
+    description: Optional[str]
+    ref_id: str = Field(alias="refId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class MockPaywallAddonFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     billing_id: Optional[str] = Field(alias="billingId")
     entitlements: List["MockPaywallAddonFragmentEntitlements"]
@@ -1268,28 +1268,42 @@
 
 
 class SubscriptionPreviewFragmentProrationNetAmount(BaseModel):
     amount: float
     currency: Currency
 
 
+class UsageHistoryFragment(BaseModel):
+    start_date: Any = Field(alias="startDate")
+    end_date: Optional[Any] = Field(alias="endDate")
+    usage_measurements: List["UsageHistoryFragmentUsageMeasurements"] = Field(
+        alias="usageMeasurements"
+    )
+
+
+class UsageHistoryFragmentUsageMeasurements(BaseModel):
+    date: Any
+    value: float
+    is_reset_point: Optional[bool] = Field(alias="isResetPoint")
+
+
 PackageEntitlementFragment.update_forward_refs()
 PackageEntitlementFragmentFeature.update_forward_refs()
 PriceFragment.update_forward_refs()
 PriceFragmentPrice.update_forward_refs()
 PriceFragmentFeature.update_forward_refs()
 AddonFragment.update_forward_refs()
 AddonFragmentEntitlements.update_forward_refs()
 AddonFragmentPrices.update_forward_refs()
 CouponFragment.update_forward_refs()
 CouponFragmentSyncStates.update_forward_refs()
 CouponFragmentCustomers.update_forward_refs()
-SlimCustomerFragment.update_forward_refs()
 PromotionalEntitlementFragment.update_forward_refs()
 PromotionalEntitlementFragmentFeature.update_forward_refs()
+SlimCustomerFragment.update_forward_refs()
 CustomerFragment.update_forward_refs()
 CustomerFragmentTrialedPlans.update_forward_refs()
 CustomerFragmentExperimentInfo.update_forward_refs()
 CustomerFragmentCoupon.update_forward_refs()
 CustomerFragmentEligibleForTrial.update_forward_refs()
 CustomerFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalBillingInformation.update_forward_refs()
@@ -1305,20 +1319,20 @@
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
 CustomerPortalPromotionalEntitlement.update_forward_refs()
 CustomerResourceFragment.update_forward_refs()
+CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
-CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricing.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingFeature.update_forward_refs()
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
@@ -1332,30 +1346,30 @@
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
 TotalPriceFragment.update_forward_refs()
 TotalPriceFragmentSubTotal.update_forward_refs()
 TotalPriceFragmentTotal.update_forward_refs()
+SubscriptionScheduledUpdateData.update_forward_refs()
+SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 ProductFragment.update_forward_refs()
 ProductFragmentProductSettings.update_forward_refs()
 ProductFragmentProductSettingsDowngradePlan.update_forward_refs()
 PlanFragment.update_forward_refs()
 PlanFragmentProduct.update_forward_refs()
 PlanFragmentBasePlan.update_forward_refs()
 PlanFragmentEntitlements.update_forward_refs()
 PlanFragmentInheritedEntitlements.update_forward_refs()
 PlanFragmentCompatibleAddons.update_forward_refs()
 PlanFragmentPrices.update_forward_refs()
 PlanFragmentDefaultTrialConfig.update_forward_refs()
-SubscriptionScheduledUpdateData.update_forward_refs()
-SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 SubscriptionFragment.update_forward_refs()
 SubscriptionFragmentResource.update_forward_refs()
 SubscriptionFragmentExperimentInfo.update_forward_refs()
 SubscriptionFragmentPrices.update_forward_refs()
 SubscriptionFragmentPricesPrice.update_forward_refs()
 SubscriptionFragmentTotalPrice.update_forward_refs()
 SubscriptionFragmentPlan.update_forward_refs()
@@ -1371,19 +1385,19 @@
 UsageUpdatedFragment.update_forward_refs()
 EntitlementUsageUpdated.update_forward_refs()
 EntitlementUsageUpdatedUsage.update_forward_refs()
 EntitlementUsageUpdatedEntitlement.update_forward_refs()
 EntitlementsUpdatedPayload.update_forward_refs()
 EntitlementsUpdatedPayloadEntitlements.update_forward_refs()
 LayoutConfigurationFragment.update_forward_refs()
-MockPaywallPackageEntitlementFragment.update_forward_refs()
-MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallPriceFragment.update_forward_refs()
 MockPaywallPriceFragmentPrice.update_forward_refs()
 MockPaywallPriceFragmentFeature.update_forward_refs()
+MockPaywallPackageEntitlementFragment.update_forward_refs()
+MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallAddonFragment.update_forward_refs()
 MockPaywallAddonFragmentEntitlements.update_forward_refs()
 MockPaywallAddonFragmentPrices.update_forward_refs()
 MockPaywallPlanFragment.update_forward_refs()
 MockPaywallPlanFragmentProduct.update_forward_refs()
 MockPaywallPlanFragmentBasePlan.update_forward_refs()
 MockPaywallPlanFragmentEntitlements.update_forward_refs()
@@ -1439,7 +1453,9 @@
 SubscriptionPreviewFragmentSubscriptionTotalExcludingTax.update_forward_refs()
 SubscriptionPreviewFragmentSubscriptionTotal.update_forward_refs()
 SubscriptionPreviewFragmentSubscriptionTax.update_forward_refs()
 SubscriptionPreviewFragmentProration.update_forward_refs()
 SubscriptionPreviewFragmentProrationCredit.update_forward_refs()
 SubscriptionPreviewFragmentProrationDebit.update_forward_refs()
 SubscriptionPreviewFragmentProrationNetAmount.update_forward_refs()
+UsageHistoryFragment.update_forward_refs()
+UsageHistoryFragmentUsageMeasurements.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.466.0/stigg/generated/get_active_subscriptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.466.0/stigg/generated/get_coupons.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.466.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.466.0/stigg/generated/get_mock_paywall.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.466.0/stigg/generated/get_sdk_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.466.0/stigg/generated/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.466.0/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.466.0/stigg/generated/provision_customer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.466.0/stigg/generated/provision_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.466.0/stigg/generated/report_usage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.465.0/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.466.0/stigg/generated/create_subscription.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Generated by ariadne-codegen on 2023-06-13 13:13
+# Generated by ariadne-codegen on 2023-06-19 12:33
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
 
 
-class UpdateSubscription(BaseModel):
-    update_subscription: "UpdateSubscriptionUpdateSubscription" = Field(
-        alias="updateSubscription"
+class CreateSubscription(BaseModel):
+    create_subscription: "CreateSubscriptionCreateSubscription" = Field(
+        alias="createSubscription"
     )
 
 
-class UpdateSubscriptionUpdateSubscription(SlimSubscriptionFragment):
+class CreateSubscriptionCreateSubscription(SlimSubscriptionFragment):
     pass
 
 
-UpdateSubscription.update_forward_refs()
-UpdateSubscriptionUpdateSubscription.update_forward_refs()
+CreateSubscription.update_forward_refs()
+CreateSubscriptionCreateSubscription.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.465.0/PKG-INFO` & `stigg_api_client_v2-0.466.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.465.0
+Version: 0.466.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

