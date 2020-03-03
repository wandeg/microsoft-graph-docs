---
title: "plannerPlanDetails resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# plannerPlanDetails resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List plannerPlanDetailses](../api/plannerplandetails-list.md)|[plannerPlanDetails](../resources/plannerPlanDetails.md) collection|List properties and relationships of the [plannerPlanDetails](../resources/plannerplandetails.md) objects.|
|[Get plannerPlanDetails](../api/plannerplandetails-get.md)|[plannerPlanDetails](../resources/plannerPlanDetails.md)|Read properties and relationships of the [plannerPlanDetails](../resources/plannerplandetails.md) object.|
|[Create plannerPlanDetails](../api/plannerplandetails-create.md)|[plannerPlanDetails](../resources/plannerPlanDetails.md)|Create a new [plannerPlanDetails](../resources/plannerplandetails.md) object.|
|[Delete plannerPlanDetails](../api/plannerplandetails-delete.md)|None|Deletes a [plannerPlanDetails](../resources/plannerplandetails.md).|
|[Update plannerPlanDetails](../api/plannerplandetails-update.md)|[plannerPlanDetails](../resources/plannerPlanDetails.md)|Update the properties of a [plannerPlanDetails](../resources/plannerplandetails.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|categoryDescriptions|[plannerCategoryDescriptions](../resources/plannerCategoryDescriptions.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|sharedWith|[plannerUserIds](../resources/plannerUserIds.md)||

## Relationships
None

## JSON Representation
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

