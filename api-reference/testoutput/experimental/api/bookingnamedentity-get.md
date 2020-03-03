---
title: "Get bookingNamedEntity"
description: "Read properties and relationships of the bookingNamedEntity object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get bookingNamedEntity

Namespace: microsoft.graph

Read properties and relationships of the [bookingNamedEntity](../resources/bookingnamedentity.md) object.

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
GET ** Entity URI for microsoft.graph.bookingNamedEntity not found
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
If successful, this method returns a `200 OK` response code and [bookingNamedEntity](../resources/bookingnamedentity.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_bookingnamedentity"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.bookingNamedEntity not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingNamedEntity"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 174

{
  "value": {
    "@odata.type": "#microsoft.graph.bookingNamedEntity",
    "id": "dcbf6554-6554-dcbf-5465-bfdc5465bfdc",
    "displayName": "Display Name value"
  }
}
```

