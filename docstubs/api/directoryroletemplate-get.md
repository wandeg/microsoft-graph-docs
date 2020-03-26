---
title: "Get directoryRoleTemplate"
description: "Read properties and relationships of the directoryRoleTemplate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get directoryRoleTemplate

Namespace: microsoft.graph

Read properties and relationships of the [directoryRoleTemplate](../resources/directoryroletemplate.md) object.

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
GET /directoryRoleTemplates/{directoryRoleTemplatesId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [directoryRoleTemplate](../resources/directoryroletemplate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplate"
}
-->
``` http
GET https://graph.microsoft.com/beta/directoryRoleTemplates/{directoryRoleTemplatesId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "value": {
    "@odata.type": "#microsoft.graph.directoryRoleTemplate",
    "id": "be40dcf2-dcf2-be40-f2dc-40bef2dc40be",
    "deletedDateTime": "2017-01-01T00:03:00.2666497+00:00",
    "description": "Description value",
    "displayName": "Display Name value"
  }
}
```

