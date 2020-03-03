---
title: "subscribedSku resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# subscribedSku resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List subscribedSkus](../api/subscribedsku-list.md)|[subscribedSku](../resources/subscribedSku.md) collection|List properties and relationships of the [subscribedSku](../resources/subscribedsku.md) objects.|
|[Get subscribedSku](../api/subscribedsku-get.md)|[subscribedSku](../resources/subscribedSku.md)|Read properties and relationships of the [subscribedSku](../resources/subscribedsku.md) object.|
|[Create subscribedSku](../api/subscribedsku-post-subscribedskus.md)|[subscribedSku](../resources/subscribedSku.md)|Create a new [subscribedSku](../resources/subscribedsku.md) object.|
|[Delete subscribedSku](../api/subscribedsku-delete.md)|None|Deletes a [subscribedSku](../resources/subscribedsku.md).|
|[Update subscribedSku](../api/subscribedsku-update.md)|[subscribedSku](../resources/subscribedSku.md)|Update the properties of a [subscribedSku](../resources/subscribedsku.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appliesTo|String||
|capabilityStatus|String||
|consumedUnits|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|prepaidUnits|[licenseUnitsDetail](../resources/licenseUnitsDetail.md)||
|servicePlans|[servicePlanInfo](../resources/servicePlanInfo.md) collection||
|skuId|Guid||
|skuPartNumber|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.subscribedSku",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subscribedSku",
  "id": "String (identifier)",
  "capabilityStatus": "String",
  "consumedUnits": 1024,
  "prepaidUnits": {
    "@odata.type": "microsoft.graph.licenseUnitsDetail"
  },
  "servicePlans": [
    {
      "@odata.type": "microsoft.graph.servicePlanInfo"
    }
  ],
  "skuId": "Guid",
  "skuPartNumber": "String",
  "appliesTo": "String"
}
```

