---
title: "Create room"
description: "Create a new room object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create room

Namespace: microsoft.graph

Create a new [room](../resources/room.md) object.

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
POST ** Collection URI for microsoft.graph.room not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [room](../resources/room.md) object.

The following table shows the properties that are required when you create the [room](../resources/room.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String| Inherited from [place](../resources/place.md)|
|geoCoordinates|[outlookGeoCoordinates](../resources/outlookgeocoordinates.md)| Inherited from [place](../resources/place.md)|
|phone|String| Inherited from [place](../resources/place.md)|
|address|[physicalAddress](../resources/physicaladdress.md)| Inherited from [place](../resources/place.md)|
|emailAddress|String||
|nickname|String||
|building|String||
|floorNumber|Int32||
|label|String||
|capacity|Int32||
|bookingType|Enumeration|. Possible values are: `unknown`, `standard`, `reserved`.|
|audioDeviceName|String||
|videoDeviceName|String||
|displayDeviceName|String||
|isWheelChairAccessible|Boolean||
|tags|String collection||
|floorLabel|String||



## Response
If successful, this method returns a `201 Created` response code and a [room](../resources/room.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_room_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.room not found
Content-type: application/json
Content-length: 1134

{
  "@odata.type": "#microsoft.graph.room",
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
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1183

{
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
```

