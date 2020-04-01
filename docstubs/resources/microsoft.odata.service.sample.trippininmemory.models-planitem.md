---
title: "PlanItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# PlanItem resource type


Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models



## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get PlanItem](../api/microsoft.odata.service.sample.trippininmemory.models-planitem-get.md)|[PlanItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md)|Read properties and relationships of the [PlanItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md) object.|
|[Update PlanItem](../api/microsoft.odata.service.sample.trippininmemory.models-planitem-update.md)|[PlanItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md)|Update the properties of a [PlanItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md) object.|
|[List PlanItems](../api/microsoft.odata.service.sample.trippininmemory.models-trip-list-planitems.md)|[PlanItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md) collection|Get the PlanItems from the PlanItems navigation property.|
|[Create PlanItems](../api/microsoft.odata.service.sample.trippininmemory.models-trip-post-planitems.md)|[PlanItem](../resources/microsoft.odata.service.sample.trippininmemory.models-planitem.md)|Create PlanItems by posting to the PlanItems collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|ConfirmationCode|String||
|Duration|Duration||
|EndsAt|DateTimeOffset||
|PlanItemId|Int32||
|StartsAt|DateTimeOffset||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.PlanItem",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.PlanItem",
  "PlanItemId": 1024,
  "ConfirmationCode": "String",
  "StartsAt": "String (timestamp)",
  "EndsAt": "String (timestamp)",
  "Duration": "String (duration)"
}
```

