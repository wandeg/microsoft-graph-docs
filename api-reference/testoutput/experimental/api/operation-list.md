---
title: "List operations"
description: "List properties and relationships of the operation objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List operations

Namespace: microsoft.graph

List properties and relationships of the [operation](../resources/operation.md) objects.

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
GET ** Collection URI for microsoft.graph.operation not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [operation](../resources/operation.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_operation"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.operation not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.operation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 296

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.operation",
      "id": "b3e200dd-00dd-b3e2-dd00-e2b3dd00e2b3",
      "status": "String",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "lastActionDateTime": "2016-12-31T23:56:52.9868016+03:00"
    }
  ]
}
```

