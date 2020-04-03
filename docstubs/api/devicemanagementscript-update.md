---
title: "Update deviceManagementScript"
description: "Update the properties of a deviceManagementScript object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceManagementScript

Namespace: microsoft.graph

Update the properties of a [deviceManagementScript](../resources/devicemanagementscript.md) object.

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
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementScript](../resources/devicemanagementscript.md) object.

The following table shows the properties that are required when you create the [deviceManagementScript](../resources/devicemanagementscript.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|enforceSignatureCheck|Boolean||
|runAs32Bit|Boolean||
|displayName|String||
|description|String||
|scriptContent|Binary||
|createdDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||
|runAsAccount|Enumeration| Possible values are: `system`, `user`.|
|fileName|String||
|roleScopeTagIds|String collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/devicemanagementscript.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementscript"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
Content-type: application/json
Content-length: 369

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "displayName": "Display Name value",
  "description": "Description value",
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "runAsAccount": "String",
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
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
Content-Length: 541

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "a2e71ebe-1ebe-a2e7-be1e-e7a2be1ee7a2",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "displayName": "Display Name value",
  "description": "Description value",
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
  "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
  "runAsAccount": "String",
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

