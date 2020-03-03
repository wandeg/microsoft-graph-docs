---
title: "Update roomList"
description: "Update the properties of a roomList object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update roomList

Update the properties of a [roomList](../resources/roomlist.md) object.

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
PATCH ** Entity URI for microsoft.graph.roomList not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [roomList](../resources/roomList.md) object.

The following table shows the properties that are required when you create the [roomList](../resources/roomlist.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String| Inherited from [place](../resources/place.md)|
|geoCoordinates|[outlookGeoCoordinates](../resources/outlookGeoCoordinates.md)| Inherited from [place](../resources/place.md)|
|phone|String| Inherited from [place](../resources/place.md)|
|address|[physicalAddress](../resources/physicalAddress.md)| Inherited from [place](../resources/place.md)|
|emailAddress|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [roomList](../resources/roomlist.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_roomlist"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.roomList not found
Content-type: application/json
Content-length: 716

{
  "@odata.type": "#microsoft.graph.roomList",
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
Content-Length: 765

{
  "@odata.type": "#microsoft.graph.roomList",
  "id": "d51acab5-cab5-d51a-b5ca-1ad5b5ca1ad5",
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
```

