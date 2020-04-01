---
title: "Trip resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# Trip resource type


Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models



## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get Trip](../api/microsoft.odata.service.sample.trippininmemory.models-trip-get.md)|[Trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md)|Read properties and relationships of the [Trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md) object.|
|[Update Trip](../api/microsoft.odata.service.sample.trippininmemory.models-trip-update.md)|[Trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md)|Update the properties of a [Trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md) object.|
|[GetInvolvedPeople](../api/microsoft.odata.service.sample.trippininmemory.models-trip-getinvolvedpeople.md)|[Person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) collection||
|[List PlanItems](../api/microsoft.odata.service.sample.trippininmemory.models-trip-list-planitems.md)|[PlanItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md) collection|Get the PlanItems from the PlanItems navigation property.|
|[Create PlanItems](../api/microsoft.odata.service.sample.trippininmemory.models-trip-post-planitems.md)|[PlanItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md)|Create PlanItems by posting to the PlanItems collection.|
|[List Trips](../api/microsoft.odata.service.sample.trippininmemory.models-person-list-trips.md)|[Trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md) collection|Get the Trips from the Trips navigation property.|
|[Create Trips](../api/microsoft.odata.service.sample.trippininmemory.models-person-post-trips.md)|[Trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md)|Create Trips by posting to the Trips collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|Budget|Single||
|Description|String||
|EndsAt|DateTimeOffset||
|Name|String||
|ShareId|Guid||
|StartsAt|DateTimeOffset||
|Tags|String collection||
|TripId|Int32||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|PlanItems|[PlanItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.Trip",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.Trip",
  "TripId": 1024,
  "ShareId": "Guid",
  "Name": "String",
  "Budget": "Single",
  "Description": "String",
  "Tags": [
    "String"
  ],
  "StartsAt": "String (timestamp)",
  "EndsAt": "String (timestamp)"
}
```

