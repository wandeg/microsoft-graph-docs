---
title: "Get deviceManagement"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Get deviceManagement

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships a deviceManagement object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from most to least privileged) |
| :------------------------------------- | :------------------------------------------ |
| Delegated (work or school account)     |                                             |
| Delegated (personal Microsoft account) |                                             |
| Application                            |                                             |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

```http

```

## Optional query parameters

This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers

| Name          | Description               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}. Required. |

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [deviceManagement](../resources/deviceManagement.md) object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "get_devicemanagement"
}
-->

```http
GET https://graph.microsoft.com/beta/

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.deviceManagement"
}
-->

```http
HTTP 1.1 200 OK

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.deviceManagement",
  "accountMoveCompletionDateTime": "DateTimeOffset",
  "adminConsent": {
    "@odata.type": "#microsoft.graph.adminConsent",
    "shareAPNSData": "String",
    "shareUserExperienceAnalyticsData": "String"
  },
  "deviceProtectionOverview": {
    "@odata.type": "#microsoft.graph.deviceProtectionOverview",
    "cleanDeviceCount": "Int32",
    "criticalFailuresDeviceCount": "Int32",
    "inactiveThreatAgentDeviceCount": "Int32",
    "pendingFullScanDeviceCount": "Int32",
    "pendingManualStepsDeviceCount": "Int32",
    "pendingOfflineScanDeviceCount": "Int32",
    "pendingQuickScanDeviceCount": "Int32",
    "pendingRestartDeviceCount": "Int32",
    "pendingSignatureUpdateDeviceCount": "Int32",
    "totalReportedDeviceCount": "Int32",
    "unknownStateThreatAgentDeviceCount": "Int32"
  },
  "id": "String(identifier)",
  "managedDeviceCleanupSettings": {
    "@odata.type": "#microsoft.graph.managedDeviceCleanupSettings",
    "deviceInactivityBeforeRetirementInDays": "String"
  },
  "subscriptionState": "String",
  "subscriptions": "String",
  "userExperienceAnalyticsSettings": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsSettings",
    "configurationManagerDataConnectorConfigured": "Boolean"
  },
  "windowsMalwareOverview": {
    "@odata.type": "#microsoft.graph.windowsMalwareOverview",
    "malwareCategorySummary": [
      {
        "@odata.type": "#microsoft.graph.windowsMalwareCategoryCount",
        "category": "String",
        "deviceCount": "Int32",
        "lastUpdateDateTime": "DateTimeOffset"
      }
    ],
    "malwareDetectedDeviceCount": "Int32",
    "malwareExecutionStateSummary": [
      {
        "@odata.type": "#microsoft.graph.windowsMalwareExecutionStateCount",
        "deviceCount": "Int32",
        "executionState": "String",
        "lastUpdateDateTime": "DateTimeOffset"
      }
    ],
    "malwareNameSummary": [
      {
        "@odata.type": "#microsoft.graph.windowsMalwareNameCount",
        "deviceCount": "Int32",
        "lastUpdateDateTime": "DateTimeOffset",
        "malwareIdentifier": "String",
        "name": "String"
      }
    ],
    "malwareStateSummary": [
      {
        "@odata.type": "#microsoft.graph.windowsMalwareStateCount",
        "deviceCount": "Int32",
        "lastUpdateDateTime": "DateTimeOffset",
        "state": "String"
      }
    ],
    "osVersionsSummary": [
      {
        "@odata.type": "#microsoft.graph.osVersionCount",
        "deviceCount": "Int32",
        "lastUpdateDateTime": "DateTimeOffset",
        "osVersion": "String"
      }
    ]
  }
}
}

```