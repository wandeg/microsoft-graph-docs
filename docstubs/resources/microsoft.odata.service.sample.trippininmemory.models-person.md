---
title: "person resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# person resource type


Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models



## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List persons](../api/microsoft.odata.service.sample.trippininmemory.models-person-list.md)|[person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) collection|List properties and relationships of the [person](../resources/person.md) objects.|
|[Get person](../api/microsoft.odata.service.sample.trippininmemory.models-person-get.md)|[person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md)|Read properties and relationships of the [person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) object.|
|[Create person](../api/microsoft.odata.service.sample.trippininmemory.models-person-post-people.md)|[person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md)|Create a new [person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) object.|
|[Delete person](../api/microsoft.odata.service.sample.trippininmemory.models-person-delete.md)|None|Deletes a [person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md).|
|[Update person](../api/microsoft.odata.service.sample.trippininmemory.models-person-update.md)|[person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md)|Update the properties of a [person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) object.|
|[shareTrip](../api/microsoft.odata.service.sample.trippininmemory.models-person-sharetrip.md)|None||
|[getFavoriteAirline](../api/microsoft.odata.service.sample.trippininmemory.models-person-getfavoriteairline.md)|[airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md)||
|[getFriendsTrips](../api/microsoft.odata.service.sample.trippininmemory.models-person-getfriendstrips.md)|[trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md) collection||
|[updatePersonLastName](../api/microsoft.odata.service.sample.trippininmemory.models-person-updatepersonlastname.md)|Boolean||
|[List friends](../api/microsoft.odata.service.sample.trippininmemory.models-person-list-friends.md)|[person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) collection|Get the persons from the friends navigation property.|
|[Create friends](../api/microsoft.odata.service.sample.trippininmemory.models-person-post-friends.md)|[person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md)|Create friends by posting to the friends collection.|
|[Get person](../api/microsoft.odata.service.sample.trippininmemory.models-person-get.md)|[person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md)|Read properties and relationships of the [person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) object.|
|[List trips](../api/microsoft.odata.service.sample.trippininmemory.models-person-list-trips.md)|[trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md) collection|Get the trips from the trips navigation property.|
|[Create trips](../api/microsoft.odata.service.sample.trippininmemory.models-person-post-trips.md)|[trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md)|Create trips by posting to the trips collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|addressInfo|[location](../resources/microsoft.odata.service.sample.trippininmemory.models-location.md) collection||
|age|Int64||
|emails|String collection||
|favoriteFeature|Enumeration| Possible values are: `feature1`, `feature2`, `feature3`, `feature4`.|
|features|Enumeration collection||
|firstName|String||
|gender|Enumeration| Possible values are: `male`, `female`, `unknow`.|
|homeAddress|[location](../resources/microsoft.odata.service.sample.trippininmemory.models-location.md)||
|lastName|String||
|middleName|String||
|userName|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|bestFriend|[person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md)||
|friends|[person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) collection||
|trips|[trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.person",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.person",
  "userName": "String",
  "firstName": "String",
  "lastName": "String",
  "middleName": "String",
  "gender": "String",
  "age": 1024,
  "emails": [
    "String"
  ],
  "addressInfo": [
    {
      "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.location",
      "address": "String",
      "city": {
        "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.city",
        "countryRegion": "String",
        "region": "String"
      }
    }
  ],
  "homeAddress": {
    "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.location"
  },
  "favoriteFeature": "String",
  "features": [
    "String"
  ]
}
```

