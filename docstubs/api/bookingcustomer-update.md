---
title: "Update bookingCustomer"
description: "Update the properties of a bookingCustomer object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update bookingCustomer

Namespace: microsoft.graph

Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.

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
PATCH /bookingBusinesses/{bookingBusinessesId}/customers/{bookingCustomerId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [bookingCustomer](../resources/bookingcustomer.md) object.

The following table shows the properties that are required when you create the [bookingCustomer](../resources/bookingcustomer.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String| Inherited from [bookingNamedEntity](../resources/bookingnamedentity.md)|
|emailAddress|String| Inherited from [bookingPerson](../resources/bookingperson.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_bookingcustomer"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/{bookingBusinessesId}/customers/{bookingCustomerId}
Content-type: application/json
Content-length: 139

{
  "@odata.type": "#microsoft.graph.bookingCustomer",
  "displayName": "Display Name value",
  "emailAddress": "Email Address value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 188

{
  "@odata.type": "#microsoft.graph.bookingCustomer",
  "id": "3685a03e-a03e-3685-3ea0-85363ea08536",
  "displayName": "Display Name value",
  "emailAddress": "Email Address value"
}
```

