---
title: "Update directoryRole"
description: "Update the properties of a directoryRole object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update directoryRole

Namespace: Microsoft.DirectoryServices

Update the properties of a [directoryRole](../resources/microsoft.directoryservices-directoryrole.md) object.

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
In the request body, supply a JSON representation for the [directoryRole](../resources/microsoft.directoryservices-directoryrole.md) object.

The following table shows the properties that are required when you create the [directoryRole](../resources/microsoft.directoryservices-directoryrole.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|roleTemplateId|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [directoryRole](../resources/microsoft.directoryservices-directoryrole.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_directoryrole"
}
-->
``` http
PATCH https://graph.microsoft.com/changelog/directoryRoles/{directoryRolesId}
Content-Type: application/json
Content-length: 252

{
  "@odata.type": "#Microsoft.DirectoryServices.directoryRole",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
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
  "@odata.type": "#Microsoft.DirectoryServices.directoryRole",
  "id": "7e645940-5940-7e64-4059-647e4059647e",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "roleTemplateId": "Role Template Id value"
}
```

