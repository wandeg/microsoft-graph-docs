---
title: "Update deviceManagementIntentDeviceStateSummary"
description: "Update the properties of a deviceManagementIntentDeviceStateSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceManagementIntentDeviceStateSummary

Namespace: microsoft.graph

Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/devicemanagementintentdevicestatesummary.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementIntentDeviceStateSummary](../resources/devicemanagementintentdevicestatesummary.md) object.

The following table shows the properties that are required when you create the [deviceManagementIntentDeviceStateSummary](../resources/devicemanagementintentdevicestatesummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|conflictCount|Int32||
|errorCount|Int32||
|failedCount|Int32||
|notApplicableCount|Int32||
|notApplicablePlatformCount|Int32||
|successCount|Int32||



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceStateSummary](../resources/devicemanagementintentdevicestatesummary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementintentdevicestatesummary"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
Content-type: application/json
Content-length: 237

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 286

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
  "id": "47480b65-0b65-4748-650b-4847650b4847",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12
}
```

