---
title: "Get operation"
description: "Read properties and relationships of the operation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get operation

Namespace: microsoft.graph

Read properties and relationships of the [operation](../resources/operation.md) object.

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
GET ** Entity URI for microsoft.graph.operation not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [operation](../resources/operation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_operation"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.operation not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.operation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": {
    "@odata.type": "#microsoft.graph.operation",
    "id": "deb6e012-e012-deb6-12e0-b6de12e0b6de",
    "status": "String",
    "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
    "lastActionDateTime": "2017-01-01T00:03:19.3737597+03:00"
  }
}
```

