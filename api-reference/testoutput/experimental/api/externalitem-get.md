---
title: "Get externalItem"
description: "Read properties and relationships of the externalItem object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get externalItem

Namespace: microsoft.graph

Read properties and relationships of the [externalItem](../resources/externalitem.md) object.

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
GET /connections/{connectionsId}/items/{externalItemId}
GET /external/connections/{externalConnectionId}/items/{externalItemId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [externalItem](../resources/externalitem.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_externalitem"
}
-->
``` http
GET https://graph.microsoft.com/localtest/connections/{connectionsId}/items/{externalItemId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 470

{
  "value": {
    "@odata.type": "#microsoft.graph.externalItem",
    "id": "9ff1b63f-b63f-9ff1-3fb6-f19f3fb6f19f",
    "properties": {
      "@odata.type": "microsoft.graph.properties"
    },
    "content": "Content value",
    "acl": [
      {
        "@odata.type": "microsoft.graph.acl",
        "type": "String",
        "value": "Value value",
        "accessType": "String",
        "identitySource": "Identity Source value"
      }
    ]
  }
}
```

