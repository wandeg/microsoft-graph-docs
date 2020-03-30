---
title: "Update deviceManagementScriptDeviceState"
description: "Update the properties of a deviceManagementScriptDeviceState object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceManagementScriptDeviceState

Namespace: microsoft.graph

Update the properties of a [deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) object.

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
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) object.

The following table shows the properties that are required when you create the [deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|runState|Enumeration| Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|resultMessage|String||
|lastStateUpdateDateTime|DateTimeOffset||
|errorCode|Int32||
|errorDescription|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementscriptdevicestate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
Content-type: application/json
Content-length: 280

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "runState": "String",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:01:25.8019336+03:00",
  "errorCode": 9,
  "errorDescription": "Error Description value"
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
Content-Length: 329

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "id": "74aaeec4-eec4-74aa-c4ee-aa74c4eeaa74",
  "runState": "String",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:01:25.8019336+03:00",
  "errorCode": 9,
  "errorDescription": "Error Description value"
}
```

