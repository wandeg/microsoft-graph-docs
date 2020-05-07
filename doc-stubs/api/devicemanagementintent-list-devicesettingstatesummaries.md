---
title: "List deviceSettingStateSummaries"
description: "Get the deviceManagementIntentDeviceSettingStateSummaries from the deviceSettingStateSummaries navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List deviceSettingStateSummaries

Namespace: microsoft.graph

Get the deviceManagementIntentDeviceSettingStateSummaries from the deviceSettingStateSummaries navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentDeviceSettingStateSummary](../resources/devicemanagementintentdevicesettingstatesummary.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementintentdevicesettingstatesummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicemanagementintentdevicesettingstatesummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
      "id": "5cdf7a38-7a38-5cdf-387a-df5c387adf5c",
      "settingName": "String",
      "compliantCount": "Integer",
      "conflictCount": "Integer",
      "errorCount": "Integer",
      "nonCompliantCount": "Integer",
      "notApplicableCount": "Integer",
      "remediatedCount": "Integer"
    }
  ]
}
```

