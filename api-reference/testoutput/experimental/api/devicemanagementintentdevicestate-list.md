---
title: "List deviceManagementIntentDeviceStates"
description: "List properties and relationships of the deviceManagementIntentDeviceState objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceManagementIntentDeviceStates

Namespace: microsoft.graph

List properties and relationships of the [deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md) objects.

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
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementintentdevicestate"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicemanagementintentdevicestate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 449

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
      "id": "3bbb7e8f-7e8f-3bbb-8f7e-bb3b8f7ebb3b",
      "userPrincipalName": "User Principal Name value",
      "userName": "User Name value",
      "deviceDisplayName": "Device Display Name value",
      "lastReportedDateTime": "2017-01-01T00:01:11.3421719+03:00",
      "state": "String",
      "deviceId": "Device Id value"
    }
  ]
}
```

