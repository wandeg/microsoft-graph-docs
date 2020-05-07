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
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceManagementScript](../resources/devicemanagementscript.md) object.

The following table shows the properties that are required when you create the [deviceManagementScript](../resources/devicemanagementscript.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|enforceSignatureCheck|Boolean|**TODO: Add Description**|
|runAs32Bit|Boolean|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|scriptContent|Binary|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|runAsAccount|runAsAccountType|**TODO: Add Description**. Possible values are: `system`, `user`.|
|fileName|String|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|



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
Content-length: 315

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "enforceSignatureCheck": "Boolean",
  "runAs32Bit": "Boolean",
  "displayName": "String",
  "description": "String",
  "scriptContent": "Binary",
  "runAsAccount": "String",
  "fileName": "String",
  "roleScopeTagIds": [
    "String"
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
  "id": "a5dd2be4-2be4-a5dd-e42b-dda5e42bdda5",
  "enforceSignatureCheck": "Boolean",
  "runAs32Bit": "Boolean",
  "displayName": "String",
  "description": "String",
  "scriptContent": "Binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "fileName": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```

