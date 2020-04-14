---
title: "airline resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# airline resource type


Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models



## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List airlines](../api/microsoft.odata.service.sample.trippininmemory.models-airline-list.md)|[airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md) collection|List properties and relationships of the [airline](../resources/airline.md) objects.|
|[Get airline](../api/microsoft.odata.service.sample.trippininmemory.models-airline-get.md)|[airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md)|Read properties and relationships of the [airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md) object.|
|[Create airline](../api/microsoft.odata.service.sample.trippininmemory.models-airline-post-airlines.md)|[airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md)|Create a new [airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md) object.|
|[Delete airline](../api/microsoft.odata.service.sample.trippininmemory.models-airline-delete.md)|None|Deletes a [airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md).|
|[Update airline](../api/microsoft.odata.service.sample.trippininmemory.models-airline-update.md)|[airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md)|Update the properties of a [airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|airlineCode|String||
|name|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.airline",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.airline",
  "airlineCode": "String",
  "name": "String"
}
```

