---
title: "Get directoryRole"
description: "Read properties and relationships of a directoryRole object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get directoryRole

Namespace: Microsoft.DirectoryServices

Read properties and relationships of a [directoryRole](../resources/microsoft.directoryservices-directoryrole.md) object.

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
GET /directoryRoles/{directoryRolesId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [directoryRole](../resources/microsoft.directoryservices-directoryrole.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}
-->
``` http
GET https://graph.microsoft.com/changelog/directoryRoles/{directoryRolesId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.directoryRole"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#Microsoft.DirectoryServices.directoryRole",
    "id": "7e645940-5940-7e64-4059-647e4059647e",
    "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "roleTemplateId": "Role Template Id value"
  }
}
```

