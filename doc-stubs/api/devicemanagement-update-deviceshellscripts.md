---
title: "Update deviceShellScripts"
description: "Update the properties of a deviceShellScripts object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deviceShellScripts

Namespace: microsoft.graph

Update the properties of a deviceShellScripts object.

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
PATCH /deviceManagement/deviceShellScripts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceShellScript](../resources/deviceshellscript.md) object.

The following table shows the properties that are required when you create the [deviceShellScript](../resources/deviceshellscript.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|executionFrequency|Duration|**TODO: Add Description**|
|retryCount|Int32|**TODO: Add Description**|
|blockExecutionNotifications|Boolean|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|scriptContent|Binary|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|runAsAccount|runAsAccountType|**TODO: Add Description**. Possible values are: `system`, `user`.|
|fileName|String|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [deviceShellScript](../resources/deviceshellscript.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_deviceshellscripts"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts
Content-Type: application/json
Content-length: 362

{
  "@odata.type": "#microsoft.graph.deviceShellScript",
  "executionFrequency": "String (duration)",
  "retryCount": "Integer",
  "blockExecutionNotifications": "Boolean",
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceShellScript",
  "id": "4f138aea-8aea-4f13-ea8a-134fea8a134f",
  "executionFrequency": "String (duration)",
  "retryCount": "Integer",
  "blockExecutionNotifications": "Boolean",
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

