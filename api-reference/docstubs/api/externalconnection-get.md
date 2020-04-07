---
title: "Get externalConnection"
description: "Read properties and relationships of the externalConnection object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get externalConnection

Namespace: microsoft.graph

Read properties and relationships of the [externalConnection](../resources/externalconnection.md) object.

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
GET /connections/{connectionsId}
GET /external/connections/{externalConnectionId}
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
If successful, this method returns a `200 OK` response code and [externalConnection](../resources/externalconnection.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_externalconnection"
}
-->
``` http
GET https://graph.microsoft.com/beta/connections/{connectionsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnection"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "value": {
    "@odata.type": "#microsoft.graph.externalConnection",
    "id": "f6dca5e1-a5e1-f6dc-e1a5-dcf6e1a5dcf6",
    "name": "Name value",
    "description": "Description value",
    "configuration": {
      "@odata.type": "microsoft.graph.configuration",
      "authorizedApps": [
        "Authorized Apps value"
      ]
    }
  }
}
```

