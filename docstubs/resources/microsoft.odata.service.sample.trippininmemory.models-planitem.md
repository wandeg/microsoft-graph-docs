---
title: "planItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# planItem resource type


Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models



## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get planItem](../api/microsoft.odata.service.sample.trippininmemory.models-planitem-get.md)|[planItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md)|Read properties and relationships of the [planItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md) object.|
|[Update planItem](../api/microsoft.odata.service.sample.trippininmemory.models-planitem-update.md)|[planItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md)|Update the properties of a [planItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|confirmationCode|String||
|duration|Duration||
|endsAtDateTime|DateTimeOffset||
|planItemId|Int32||
|startsAtDateTime|DateTimeOffset||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.planItem",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.planItem",
  "planItemId": 1024,
  "confirmationCode": "String",
  "startsAtDateTime": "String (timestamp)",
  "endsAtDateTime": "String (timestamp)",
  "duration": "String (duration)"
}
```

