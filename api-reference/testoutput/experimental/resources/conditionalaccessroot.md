---
title: "conditionalAccessRoot resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# conditionalAccessRoot resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get conditionalAccessRoot](../api/conditionalaccessroot-get.md)|[conditionalAccessRoot](../resources/conditionalaccessroot.md)|Read properties and relationships of the [conditionalAccessRoot](../resources/conditionalaccessroot.md) object.|
|[Update conditionalAccessRoot](../api/conditionalaccessroot-update.md)|[conditionalAccessRoot](../resources/conditionalaccessroot.md)|Update the properties of a [conditionalAccessRoot](../resources/conditionalaccessroot.md) object.|
|[List policies](../api/conditionalaccessroot-list-policies.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) collection|Get the conditionalAccessPolicies from the policies navigation property.|
|[Add policies](../api/conditionalaccessroot-post-policies.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)|Add policies by posting to the policies collection.|
|[List namedLocations](../api/conditionalaccessroot-list-namedlocations.md)|[namedLocation](../resources/namedlocation.md) collection|Get the namedLocations from the namedLocations navigation property.|
|[Add namedLocations](../api/conditionalaccessroot-post-namedlocations.md)|[namedLocation](../resources/namedlocation.md)|Add namedLocations by posting to the namedLocations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|namedLocations|[namedLocation](../resources/namedlocation.md) collection||
|policies|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conditionalAccessRoot",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conditionalAccessRoot",
  "id": "String (identifier)"
}
```

