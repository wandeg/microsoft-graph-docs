---
title: "Update directoryRoleTemplate"
description: "Update the properties of a directoryRoleTemplate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update directoryRoleTemplate

Namespace: microsoft.graph

Update the properties of a [directoryRoleTemplate](../resources/directoryroletemplate.md) object.

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
PATCH /directoryRoleTemplates/{directoryRoleTemplatesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [directoryRoleTemplate](../resources/directoryroletemplate.md) object.

The following table shows the properties that are required when you create the [directoryRoleTemplate](../resources/directoryroletemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String||
|displayName|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [directoryRoleTemplate](../resources/directoryroletemplate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_directoryroletemplate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/directoryRoleTemplates/{directoryRoleTemplatesId}
Content-type: application/json
Content-length: 201

{
  "@odata.type": "#microsoft.graph.directoryRoleTemplate",
  "deletedDateTime": "2017-01-01T00:01:42.7296606+00:00",
  "description": "Description value",
  "displayName": "Display Name value"
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
Content-Length: 250

{
  "@odata.type": "#microsoft.graph.directoryRoleTemplate",
  "id": "a161b916-b916-a161-16b9-61a116b961a1",
  "deletedDateTime": "2017-01-01T00:01:42.7296606+00:00",
  "description": "Description value",
  "displayName": "Display Name value"
}
```

