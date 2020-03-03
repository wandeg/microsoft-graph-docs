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

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /bookingBusinesses/{bookingBusinessesId}/customers/{bookingCustomerId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [bookingCustomer](../resources/bookingcustomer.md) object.

The following table shows the properties that are required when you create the [bookingCustomer](../resources/bookingcustomer.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|Display name of this entity.
The display name is suitable for human-readable interfaces. Inherited from [bookingNamedEntity](../resources/bookingnamedentity.md)|
|emailAddress|String|The e-mail address of this person. Inherited from [bookingPerson](../resources/bookingperson.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_bookingcustomer"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/bookingBusinesses/{bookingBusinessesId}/customers/{bookingCustomerId}
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
  "id": "626ab662-b662-626a-62b6-6a6262b66a62",
  "displayName": "Display Name value",
  "emailAddress": "Email Address value"
}
```

