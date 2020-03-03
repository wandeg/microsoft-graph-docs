---
title: "Update bookingPerson"
description: "Update the properties of a bookingPerson object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update bookingPerson

Update the properties of a [bookingPerson](../resources/bookingperson.md) object.

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
PATCH ** Entity URI for microsoft.graph.bookingPerson not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [bookingPerson](../resources/bookingPerson.md) object.

The following table shows the properties that are required when you create the [bookingPerson](../resources/bookingperson.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|Display name of this entity.
The display name is suitable for human-readable interfaces. Inherited from [bookingNamedEntity](../resources/bookingNamedEntity.md)|
|emailAddress|String|The e-mail address of this person.|



## Response
If successful, this method returns a `200 OK` response code and an updated [bookingPerson](../resources/bookingperson.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_bookingperson"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.bookingPerson not found
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.bookingPerson",
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
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.bookingPerson",
  "id": "a66bf211-f211-a66b-11f2-6ba611f26ba6",
  "displayName": "Display Name value",
  "emailAddress": "Email Address value"
}
```

