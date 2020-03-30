---
title: "Get bookingCustomer"
description: "Read properties and relationships of the bookingCustomer object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get bookingCustomer

Namespace: microsoft.graph

Read properties and relationships of the [bookingCustomer](../resources/bookingcustomer.md) object.

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
GET /bookingBusinesses/{bookingBusinessesId}/customers/{bookingCustomerId}
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
If successful, this method returns a `200 OK` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_bookingcustomer"
}
-->
``` http
GET https://graph.microsoft.com/beta/bookingBusinesses/{bookingBusinessesId}/customers/{bookingCustomerId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "value": {
    "@odata.type": "#microsoft.graph.bookingCustomer",
    "id": "ca55f813-f813-ca55-13f8-55ca13f855ca",
    "displayName": "Display Name value",
    "emailAddress": "Email Address value"
  }
}
```

