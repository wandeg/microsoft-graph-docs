---
title: "Update directoryRole"
description: "Update the properties of a directoryRole object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update directoryRole

Namespace: microsoft.graph

Update the properties of a [directoryRole](../resources/directoryrole.md) object.

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
PATCH /directoryRoles/{directoryRolesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [directoryRole](../resources/directoryrole.md) object.

The following table shows the properties that are required when you create the [directoryRole](../resources/directoryrole.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|roleTemplateId|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [directoryRole](../resources/directoryrole.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_directoryrole"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/directoryRoles/{directoryRolesId}
Content-Type: application/json
Content-length: 240

{
  "@odata.type": "#microsoft.graph.directoryRole",
  "deletedDateTime": "2017-01-01T00:02:07.4980046+03:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "roleTemplateId": "Role Template Id value"
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
  "@odata.type": "#microsoft.graph.directoryRole",
  "id": "ed3d394a-394a-ed3d-4a39-3ded4a393ded",
  "deletedDateTime": "2017-01-01T00:02:07.4980046+03:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "roleTemplateId": "Role Template Id value"
}
```

