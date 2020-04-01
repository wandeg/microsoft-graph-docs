---
title: "Location resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# Location resource type


Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models



## Properties
|Property|Type|Description|
|:---|:---|:---|
|Address|String||
|City|[City](../resources/microsoft.odata.service.sample.trippininmemory.models-city.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.Location"
}
-->
``` json
{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.Location",
  "Address": "String",
  "City": {
    "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.City",
    "Name": "String",
    "CountryRegion": "String",
    "Region": "String"
  }
}
```

