---
title: "Person resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# Person resource type


Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models



## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List Persons](../api/microsoft.odata.service.sample.trippininmemory.models-person-list.md)|[Person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) collection|List properties and relationships of the [Person](../resources/person.md) objects.|
|[Get Person](../api/microsoft.odata.service.sample.trippininmemory.models-person-get.md)|[Person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md)|Read properties and relationships of the [Person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) object.|
|[Create Person](../api/microsoft.odata.service.sample.trippininmemory.models-person-post-people.md)|[Person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md)|Create a new [Person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) object.|
|[Delete Person](../api/microsoft.odata.service.sample.trippininmemory.models-person-delete.md)|None|Deletes a [Person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md).|
|[Update Person](../api/microsoft.odata.service.sample.trippininmemory.models-person-update.md)|[Person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md)|Update the properties of a [Person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) object.|
|[ShareTrip](../api/microsoft.odata.service.sample.trippininmemory.models-person-sharetrip.md)|None||
|[GetFavoriteAirline](../api/microsoft.odata.service.sample.trippininmemory.models-person-getfavoriteairline.md)|[Airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md)||
|[GetFriendsTrips](../api/microsoft.odata.service.sample.trippininmemory.models-person-getfriendstrips.md)|[Trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md) collection||
|[UpdatePersonLastName](../api/microsoft.odata.service.sample.trippininmemory.models-person-updatepersonlastname.md)|Boolean||
|[List Friends](../api/microsoft.odata.service.sample.trippininmemory.models-person-list-friends.md)|[Person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) collection|Get the Persons from the Friends navigation property.|
|[Create Friends](../api/microsoft.odata.service.sample.trippininmemory.models-person-post-friends.md)|[Person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md)|Create Friends by posting to the Friends collection.|
|[Get Person](../api/microsoft.odata.service.sample.trippininmemory.models-person-get.md)|[Person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md)|Read properties and relationships of the [Person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) object.|
|[List Trips](../api/microsoft.odata.service.sample.trippininmemory.models-person-list-trips.md)|[Trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md) collection|Get the Trips from the Trips navigation property.|
|[Create Trips](../api/microsoft.odata.service.sample.trippininmemory.models-person-post-trips.md)|[Trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md)|Create Trips by posting to the Trips collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|AddressInfo|[Location](../resources/microsoft.odata.service.sample.trippininmemory.models-location.md) collection||
|Age|Int64||
|Emails|String collection||
|FavoriteFeature|Enumeration| Possible values are: `Feature1`, `Feature2`, `Feature3`, `Feature4`.|
|Features|Enumeration collection||
|FirstName|String||
|Gender|Enumeration| Possible values are: `Male`, `Female`, `Unknow`.|
|HomeAddress|[Location](../resources/microsoft.odata.service.sample.trippininmemory.models-location.md)||
|LastName|String||
|MiddleName|String||
|UserName|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|BestFriend|[Person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md)||
|Friends|[Person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) collection||
|Trips|[Trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.Person",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.Person",
  "UserName": "String",
  "FirstName": "String",
  "LastName": "String",
  "MiddleName": "String",
  "Gender": "String",
  "Age": 1024,
  "Emails": [
    "String"
  ],
  "AddressInfo": [
    {
      "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.Location",
      "Address": "String",
      "City": {
        "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.City",
        "CountryRegion": "String",
        "Region": "String"
      }
    }
  ],
  "HomeAddress": {
    "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.Location"
  },
  "FavoriteFeature": "String",
  "Features": [
    "String"
  ]
}
```

