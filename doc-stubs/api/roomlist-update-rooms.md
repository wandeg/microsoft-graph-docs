---
title: "Update rooms"
description: "Update the properties of a rooms object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update rooms

Namespace: microsoft.graph

Update the properties of a rooms object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roomList/rooms
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [room](../resources/room.md) object.

The following table shows the properties that are required when you create the [room](../resources/room.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description** Inherited from [place](../resources/place.md)|
|geoCoordinates|[outlookGeoCoordinates](../resources/outlookgeocoordinates.md)|**TODO: Add Description** Inherited from [place](../resources/place.md)|
|phone|String|**TODO: Add Description** Inherited from [place](../resources/place.md)|
|address|[physicalAddress](../resources/physicaladdress.md)|**TODO: Add Description** Inherited from [place](../resources/place.md)|
|emailAddress|String|**TODO: Add Description**|
|nickname|String|**TODO: Add Description**|
|building|String|**TODO: Add Description**|
|floorNumber|Int32|**TODO: Add Description**|
|label|String|**TODO: Add Description**|
|capacity|Int32|**TODO: Add Description**|
|bookingType|bookingType|**TODO: Add Description**. Possible values are: `unknown`, `standard`, `reserved`.|
|audioDeviceName|String|**TODO: Add Description**|
|videoDeviceName|String|**TODO: Add Description**|
|displayDeviceName|String|**TODO: Add Description**|
|isWheelChairAccessible|Boolean|**TODO: Add Description**|
|tags|String collection|**TODO: Add Description**|
|floorLabel|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [room](../resources/room.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_rooms"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/roomList/rooms
Content-Type: application/json
Content-length: 643

{
  "@odata.type": "#microsoft.graph.room",
  "displayName": "String",
  "geoCoordinates": {
    "@odata.type": "microsoft.graph.outlookGeoCoordinates"
  },
  "phone": "String",
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "emailAddress": "String",
  "nickname": "String",
  "building": "String",
  "floorNumber": "Integer",
  "label": "String",
  "capacity": "Integer",
  "bookingType": "String",
  "audioDeviceName": "String",
  "videoDeviceName": "String",
  "displayDeviceName": "String",
  "isWheelChairAccessible": "Boolean",
  "tags": [
    "String"
  ],
  "floorLabel": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.room",
  "id": "008d0368-0368-008d-6803-8d0068038d00",
  "displayName": "String",
  "geoCoordinates": {
    "@odata.type": "microsoft.graph.outlookGeoCoordinates"
  },
  "phone": "String",
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "emailAddress": "String",
  "nickname": "String",
  "building": "String",
  "floorNumber": "Integer",
  "label": "String",
  "capacity": "Integer",
  "bookingType": "String",
  "audioDeviceName": "String",
  "videoDeviceName": "String",
  "displayDeviceName": "String",
  "isWheelChairAccessible": "Boolean",
  "tags": [
    "String"
  ],
  "floorLabel": "String"
}
```

