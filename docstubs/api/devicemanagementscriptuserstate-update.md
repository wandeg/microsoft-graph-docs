---
title: "Update deviceManagementScriptUserState"
description: "Update the properties of a deviceManagementScriptUserState object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceManagementScriptUserState

Namespace: microsoft.graph

Update the properties of a [deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md) object.

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
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md) object.

The following table shows the properties that are required when you create the [deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|successDeviceCount|Int32||
|errorDeviceCount|Int32||
|userPrincipalName|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementscriptuserstate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
Content-type: application/json
Content-length: 180

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
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
Content-Length: 229

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "id": "5028334b-334b-5028-4b33-28504b332850",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```

