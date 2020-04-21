---
title: "Update directoryRole"
description: "Update the properties of a directoryRole object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
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

## Request body
In the request body, supply a JSON representation for the [directoryRole](../resources/directoryrole.md) object.

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
  "deletedDateTime": "2016-12-31T23:57:29.5624424+00:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "roleTemplateId": "Role Template Id value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
  "id": "bb5b6679-6679-bb5b-7966-5bbb79665bbb",
  "deletedDateTime": "2016-12-31T23:57:29.5624424+00:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "roleTemplateId": "Role Template Id value"
}
```

