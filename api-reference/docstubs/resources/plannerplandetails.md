---
title: "plannerPlanDetails resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# plannerPlanDetails resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get plannerPlanDetails](../api/plannerplandetails-get.md)|[plannerPlanDetails](../resources/plannerplandetails.md)|Read properties and relationships of a [plannerPlanDetails](../resources/plannerplandetails.md) object.|
|[Update plannerPlanDetails](../api/plannerplandetails-update.md)|[plannerPlanDetails](../resources/plannerplandetails.md)|Update the properties of a [plannerPlanDetails](../resources/plannerplandetails.md) object.|
|[List details](../api/plannerplan-list-details.md)|[plannerPlanDetails](../resources/plannerplandetails.md) collection|Get the plannerPlanDetails from the details navigation property.|
|[Create details](../api/plannerplan-post-details.md)|[plannerPlanDetails](../resources/plannerplandetails.md)|Create a new details object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|categoryDescriptions|[plannerCategoryDescriptions](../resources/plannercategorydescriptions.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|sharedWith|[plannerUserIds](../resources/planneruserids.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerPlanDetails",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerPlanDetails",
  "id": "String (identifier)",
  "sharedWith": {
    "@odata.type": "microsoft.graph.plannerUserIds"
  },
  "categoryDescriptions": {
    "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
  }
}
```

