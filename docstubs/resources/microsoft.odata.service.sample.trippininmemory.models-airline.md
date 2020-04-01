---
title: "Airline resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# Airline resource type


Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models



## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List Airlines](../api/microsoft.odata.service.sample.trippininmemory.models-airline-list.md)|[Airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md) collection|List properties and relationships of the [Airline](../resources/airline.md) objects.|
|[Get Airline](../api/microsoft.odata.service.sample.trippininmemory.models-airline-get.md)|[Airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md)|Read properties and relationships of the [Airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md) object.|
|[Create Airline](../api/microsoft.odata.service.sample.trippininmemory.models-airline-post-airlines.md)|[Airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md)|Create a new [Airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md) object.|
|[Delete Airline](../api/microsoft.odata.service.sample.trippininmemory.models-airline-delete.md)|None|Deletes a [Airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md).|
|[Update Airline](../api/microsoft.odata.service.sample.trippininmemory.models-airline-update.md)|[Airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md)|Update the properties of a [Airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|AirlineCode|String||
|Name|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.Airline",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.Airline",
  "AirlineCode": "String",
  "Name": "String"
}
```

