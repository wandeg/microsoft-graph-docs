---
title: "airport resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# airport resource type


Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models



## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List airports](../api/microsoft.odata.service.sample.trippininmemory.models-airport-list.md)|[airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md) collection|List properties and relationships of the [airport](../resources/airport.md) objects.|
|[Get airport](../api/microsoft.odata.service.sample.trippininmemory.models-airport-get.md)|[airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md)|Read properties and relationships of the [airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md) object.|
|[Create airport](../api/microsoft.odata.service.sample.trippininmemory.models-airport-post-airports.md)|[airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md)|Create a new [airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md) object.|
|[Delete airport](../api/microsoft.odata.service.sample.trippininmemory.models-airport-delete.md)|None|Deletes a [airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md).|
|[Update airport](../api/microsoft.odata.service.sample.trippininmemory.models-airport-update.md)|[airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md)|Update the properties of a [airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|airpLocation|[airportLocation](../resources/microsoft.odata.service.sample.trippininmemory.models-airportlocation.md)||
|iataCode|String||
|icaoCode|String||
|name|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.airport",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.airport",
  "icaoCode": "String",
  "name": "String",
  "iataCode": "String",
  "airpLocation": {
    "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.airportLocation"
  }
}
```

