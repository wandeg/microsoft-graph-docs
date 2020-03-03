---
title: "List operations"
description: "Get the connectionOperations from the operations navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List operations

Namespace: microsoft.graph

Get the connectionOperations from the operations navigation property.

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
GET /connections/{connectionsId}/operations
GET /external/connections/{externalConnectionId}/operations
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [connectionOperation](../resources/connectionoperation.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_connectionoperation"
}
-->
``` http
GET https://graph.microsoft.com/localtest/connections/{connectionsId}/operations
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.connectionoperation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 501

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.connectionOperation",
      "id": "21156cef-6cef-2115-ef6c-1521ef6c1521",
      "status": "String",
      "error": {
        "@odata.type": "microsoft.graph.errorDetail",
        "errorCode": "Error Code value",
        "message": "Message value",
        "details": [
          {
            "@odata.type": "microsoft.graph.innerErrorDetail",
            "source": "Source value"
          }
        ]
      }
    }
  ]
}
```

