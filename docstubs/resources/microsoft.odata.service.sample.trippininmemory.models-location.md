---
title: "location resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# location resource type


Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models



## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|String||
|city|[city](../resources/microsoft.odata.service.sample.trippininmemory.models-city.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.location"
}
-->
``` json
{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.location",
  "address": "String",
  "city": {
    "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.city",
    "name": "String",
    "countryRegion": "String",
    "region": "String"
  }
}
```

