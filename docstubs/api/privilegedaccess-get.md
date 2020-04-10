---
title: "Get privilegedAccess"
description: "Read properties and relationships of the privilegedAccess object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get privilegedAccess

Namespace: microsoft.graph

Read properties and relationships of the [privilegedAccess](../resources/privilegedaccess.md) object.

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
GET /privilegedAccess/{privilegedAccessId}
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
If successful, this method returns a `200 OK` response code and [privilegedAccess](../resources/privilegedaccess.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_privilegedaccess"
}
-->
``` http
GET https://graph.microsoft.com/beta/privilegedAccess/{privilegedAccessId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedAccess"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 172

{
  "value": {
    "@odata.type": "#microsoft.graph.privilegedAccess",
    "id": "e16ed839-d839-e16e-39d8-6ee139d86ee1",
    "displayName": "Display Name value"
  }
}
```

