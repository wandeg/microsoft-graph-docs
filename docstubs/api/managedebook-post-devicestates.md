---
title: "Add deviceStates"
description: "Add deviceStates by posting to the deviceStates collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add deviceStates

Namespace: microsoft.graph

Add deviceStates by posting to the deviceStates collection.

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
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceInstallState](../resources/deviceinstallstate.md) object.

The following table shows the properties that are required when you create the [deviceInstallState](../resources/deviceinstallstate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deviceName|String||
|deviceId|String||
|lastSyncDateTime|DateTimeOffset||
|installState|Enumeration| Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.|
|errorCode|String||
|osVersion|String||
|osDescription|String||
|userName|String||



## Response
If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/deviceinstallstate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_deviceinstallstate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2016-12-31T23:57:45.5058522+00:00",
  "installState": "String",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceinstallstate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 420

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "817d167d-167d-817d-7d16-7d817d167d81",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2016-12-31T23:57:45.5058522+00:00",
  "installState": "String",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```

