---
title: "trip resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# trip resource type


Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models



## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get trip](../api/microsoft.odata.service.sample.trippininmemory.models-trip-get.md)|[trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md)|Read properties and relationships of the [trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md) object.|
|[Update trip](../api/microsoft.odata.service.sample.trippininmemory.models-trip-update.md)|[trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md)|Update the properties of a [trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md) object.|
|[getInvolvedPeople](../api/microsoft.odata.service.sample.trippininmemory.models-trip-getinvolvedpeople.md)|[person](../resources/microsoft.odata.service.sample.trippininmemory.models-person.md) collection||
|[List planItems](../api/microsoft.odata.service.sample.trippininmemory.models-trip-list-planitems.md)|[planItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md) collection|Get the planItems from the planItems navigation property.|
|[Create planItems](../api/microsoft.odata.service.sample.trippininmemory.models-trip-post-planitems.md)|[planItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md)|Create planItems by posting to the planItems collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|budget|Single||
|description|String||
|endsAt|DateTimeOffset||
|name|String||
|shareId|Guid||
|startsAtDateTime|DateTimeOffset||
|tags|String collection||
|tripId|Int32||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|planItems|[planItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.trip",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.trip",
  "tripId": 1024,
  "shareId": "Guid",
  "name": "String",
  "budget": "Single",
  "description": "String",
  "tags": [
    "String"
  ],
  "startsAtDateTime": "String (timestamp)",
  "endsAt": "String (timestamp)"
}
```

