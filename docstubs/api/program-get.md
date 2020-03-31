---
title: "Get program"
description: "Read properties and relationships of the program object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get program

Namespace: microsoft.graph

Read properties and relationships of the [program](../resources/program.md) object.

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
GET /programs/{programsId}
GET /programControls/{programControlsId}/program
GET /programs/{programsId}/controls/{programControlId}/program
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
If successful, this method returns a `200 OK` response code and [program](../resources/program.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_program"
}
-->
``` http
GET https://graph.microsoft.com/beta/programs/{programsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 204

{
  "value": {
    "@odata.type": "#microsoft.graph.program",
    "id": "3b90a8a8-a8a8-3b90-a8a8-903ba8a8903b",
    "displayName": "Display Name value",
    "description": "Description value"
  }
}
```

