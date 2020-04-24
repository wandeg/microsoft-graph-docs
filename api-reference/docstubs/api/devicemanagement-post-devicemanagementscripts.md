---
title: "Create deviceManagementScripts"
description: "Create a new deviceManagementScripts object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create deviceManagementScripts

Namespace: microsoft.graph

Create a new deviceManagementScripts object.

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
POST /deviceManagement/deviceManagementScripts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [deviceManagementScript](../resources/devicemanagementscript.md) object.

The following table shows the properties that are required when you create the [deviceManagementScript](../resources/devicemanagementscript.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|enforceSignatureCheck|Boolean|Indicate whether the script signature needs be checked.|
|runAs32Bit|Boolean|A value indicating whether the PowerShell script should run as 32-bit|
|displayName|String|Name of the device management script.|
|description|String|Optional description for the device management script.|
|scriptContent|Binary|The script content.|
|createdDateTime|DateTimeOffset|The date and time the device management script was created. This property is read-only.|
|lastModifiedDateTime|DateTimeOffset|The date and time the device management script was last modified. This property is read-only.|
|runAsAccount|runAsAccountType|Indicates the type of execution context. Possible values are: `system`, `user`.|
|fileName|String|Script file name.|
|roleScopeTagIds|String collection|List of Scope Tag IDs for this PowerShellScript instance.|



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/devicemanagementscript.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementscript_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
Content-Type: application/json
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementscript"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "cde7842f-842f-cde7-2f84-e7cd2f84e7cd",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "displayName": "Display Name value",
  "description": "Description value",
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "runAsAccount": "String",
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

