---
title: "Get room"
description: "Read properties and relationships of the room object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get room

Namespace: microsoft.graph

Read properties and relationships of the [room](../resources/room.md) object.

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
GET ** Entity URI for microsoft.graph.room not found
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
If successful, this method returns a `200 OK` response code and [room](../resources/room.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_room"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.room not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.room"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1276

{
  "value": {
    "@odata.type": "#microsoft.graph.room",
    "id": "51d745b3-45b3-51d7-b345-d751b345d751",
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
    "emailAddress": "Email Address value",
    "nickname": "Nickname value",
    "building": "Building value",
    "floorNumber": 11,
    "label": "Label value",
    "capacity": 8,
    "bookingType": "String",
    "audioDeviceName": "Audio Device Name value",
    "videoDeviceName": "Video Device Name value",
    "displayDeviceName": "Display Device Name value",
    "isWheelChairAccessible": true,
    "tags": [
      "Tags value"
    ],
    "floorLabel": "Floor Label value"
  }
}
```

