---
title: "Get deviceManagementScriptDeviceState"
description: "Read properties and relationships of the deviceManagementScriptDeviceState object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get deviceManagementScriptDeviceState

Namespace: microsoft.graph

Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) object.

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
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
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
If successful, this method returns a `200 OK` response code and [deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementscriptdevicestate"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceManagementScriptDeviceState"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 362

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
    "id": "da14f40a-f40a-da14-0af4-14da0af414da",
    "runState": "String",
    "resultMessage": "Result Message value",
    "lastStateUpdateDateTime": "2016-12-31T23:59:16.4588852+03:00",
    "errorCode": 9,
    "errorDescription": "Error Description value"
  }
}
```

