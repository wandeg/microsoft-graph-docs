---
title: "eventLocation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# eventLocation resource type


Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models




Inherits from [location](../resources/location.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|String| Inherited from [location](../resources/microsoft.odata.service.sample.trippininmemory.models-location.md)|
|buildingInfo|String||
|city|[city](../resources/microsoft.odata.service.sample.trippininmemory.models-city.md)| Inherited from [location](../resources/microsoft.odata.service.sample.trippininmemory.models-location.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.eventLocation"
}
-->
``` json
{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.eventLocation",
  "address": "String",
  "city": {
    "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.city",
    "name": "String",
    "countryRegion": "String",
    "region": "String"
  },
  "buildingInfo": "String"
}
```

