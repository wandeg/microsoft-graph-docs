---
title: "List deviceManagementIntentDeviceSettingStateSummaries"
description: "List properties and relationships of the deviceManagementIntentDeviceSettingStateSummary objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceManagementIntentDeviceSettingStateSummaries

Namespace: microsoft.graph

List properties and relationships of the [deviceManagementIntentDeviceSettingStateSummary](../resources/devicemanagementintentdevicesettingstatesummary.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentDeviceSettingStateSummary](../resources/devicemanagementintentdevicesettingstatesummary.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementintentdevicesettingstatesummary"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicemanagementintentdevicesettingstatesummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
      "id": "19d40817-0817-19d4-1708-d4191708d419",
      "settingName": "Setting Name value",
      "compliantCount": 14,
      "conflictCount": 13,
      "errorCount": 10,
      "nonCompliantCount": 1,
      "notApplicableCount": 2,
      "remediatedCount": 15
    }
  ]
}
```

