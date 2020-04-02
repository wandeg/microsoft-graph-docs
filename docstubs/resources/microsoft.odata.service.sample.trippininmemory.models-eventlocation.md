---
title: "EventLocation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# EventLocation resource type


Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models




Inherits from [Location](../resources/location.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|Address|String| Inherited from [Location](../resources/microsoft.odata.service.sample.trippininmemory.models-location.md)|
|BuildingInfo|String||
|City|[City](../resources/microsoft.odata.service.sample.trippininmemory.models-city.md)| Inherited from [Location](../resources/microsoft.odata.service.sample.trippininmemory.models-location.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.EventLocation"
}
-->
``` json
{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.EventLocation",
  "Address": "String",
  "City": {
    "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.City",
    "Name": "String",
    "CountryRegion": "String",
    "Region": "String"
  },
  "BuildingInfo": "String"
}
```

