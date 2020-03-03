---
title: "Update directoryRole"
description: "Update the properties of a directoryRole object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update directoryRole

Update the properties of a [directoryRole](../resources/directoryrole.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /directoryRoles/{directoryRolesId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [directoryRole](../resources/directoryRole.md) object.

The following table shows the properties that are required when you create the [directoryRole](../resources/directoryrole.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryObject.md)|
|description|String||
|displayName|String||
|roleTemplateId|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [directoryRole](../resources/directoryrole.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_directoryrole"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/directoryRoles/{directoryRolesId}
Content-type: application/json
Content-length: 240

{
  "@odata.type": "#microsoft.graph.directoryRole",
  "deletedDateTime": "2017-01-01T00:00:34.0507931+03:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "roleTemplateId": "Role Template Id value"
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
Content-Length: 289

{
  "@odata.type": "#microsoft.graph.directoryRole",
  "id": "712127af-27af-7121-af27-2171af272171",
  "deletedDateTime": "2017-01-01T00:00:34.0507931+03:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "roleTemplateId": "Role Template Id value"
}
```

