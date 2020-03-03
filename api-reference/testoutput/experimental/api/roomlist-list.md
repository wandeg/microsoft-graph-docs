---
title: "List roomLists"
description: "List properties and relationships of the roomList objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List roomLists

Namespace: microsoft.graph

List properties and relationships of the [roomList](../resources/roomlist.md) objects.

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
GET ** Collection URI for microsoft.graph.roomList not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [roomList](../resources/roomlist.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_roomlist"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.roomList not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.roomlist)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 890

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roomList",
      "id": "e819daf2-daf2-e819-f2da-19e8f2da19e8",
      "displayName": "Display Name value",
      "geoCoordinates": {
        "@odata.type": "microsoft.graph.outlookGeoCoordinates",
        "altitude": "Double",
        "latitude": "Double",
        "longitude": "Double",
        "accuracy": "Double",
        "altitudeAccuracy": "Double"
      },
      "phone": "Phone value",
      "address": {
        "@odata.type": "microsoft.graph.physicalAddress",
        "type": "String",
        "postOfficeBox": "Post Office Box value",
        "street": "Street value",
        "city": "City value",
        "state": "State value",
        "countryOrRegion": "Country Or Region value",
        "postalCode": "Postal Code value"
      },
      "emailAddress": "Email Address value"
    }
  ]
}
```

