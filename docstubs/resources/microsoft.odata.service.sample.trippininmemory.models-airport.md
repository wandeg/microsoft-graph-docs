---
title: "Airport resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# Airport resource type


Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models



## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List Airports](../api/microsoft.odata.service.sample.trippininmemory.models-airport-list.md)|[Airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md) collection|List properties and relationships of the [Airport](../resources/airport.md) objects.|
|[Get Airport](../api/microsoft.odata.service.sample.trippininmemory.models-airport-get.md)|[Airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md)|Read properties and relationships of the [Airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md) object.|
|[Create Airport](../api/microsoft.odata.service.sample.trippininmemory.models-airport-post-airports.md)|[Airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md)|Create a new [Airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md) object.|
|[Delete Airport](../api/microsoft.odata.service.sample.trippininmemory.models-airport-delete.md)|None|Deletes a [Airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md).|
|[Update Airport](../api/microsoft.odata.service.sample.trippininmemory.models-airport-update.md)|[Airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md)|Update the properties of a [Airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|IataCode|String||
|IcaoCode|String||
|Location|[AirportLocation](../resources/microsoft.odata.service.sample.trippininmemory.models-airportlocation.md)||
|Name|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.Airport",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.Airport",
  "IcaoCode": "String",
  "Name": "String",
  "IataCode": "String",
  "Location": {
    "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.AirportLocation"
  }
}
```

