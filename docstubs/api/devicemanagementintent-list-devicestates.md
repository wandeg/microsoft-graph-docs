---
title: "List deviceStates"
description: "Get the deviceManagementIntentDeviceStates from the deviceStates navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceStates

Namespace: microsoft.graph

Get the deviceManagementIntentDeviceStates from the deviceStates navigation property.

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
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementintentdevicestate"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates
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
      "id": "3982da0d-da0d-3982-0dda-82390dda8239",
      "userPrincipalName": "User Principal Name value",
      "userName": "User Name value",
      "deviceDisplayName": "Device Display Name value",
      "lastReportedDateTime": "2016-12-31T23:59:04.0371883+03:00",
      "state": "String",
      "deviceId": "Device Id value"
    }
  ]
}
```

