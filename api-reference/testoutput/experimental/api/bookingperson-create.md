---
title: "Create bookingPerson"
description: "Create a new bookingPerson object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create bookingPerson

Namespace: microsoft.graph

Create a new [bookingPerson](../resources/bookingperson.md) object.

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
POST ** Collection URI for microsoft.graph.bookingPerson not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [bookingPerson](../resources/bookingperson.md) object.

The following table shows the properties that are required when you create the [bookingPerson](../resources/bookingperson.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|Display name of this entity.
The display name is suitable for human-readable interfaces. Inherited from [bookingNamedEntity](../resources/bookingnamedentity.md)|
|emailAddress|String|The e-mail address of this person.|



## Response
If successful, this method returns a `201 Created` response code and a [bookingPerson](../resources/bookingperson.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_bookingperson_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.bookingPerson not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingperson"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.bookingPerson",
  "id": "c464f74e-f74e-c464-4ef7-64c44ef764c4",
  "displayName": "Display Name value",
  "emailAddress": "Email Address value"
}
```

