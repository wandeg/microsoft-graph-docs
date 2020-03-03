---
title: "plannerGroup resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# plannerGroup resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List plannerGroups](../api/plannergroup-list.md)|[plannerGroup](../resources/plannerGroup.md) collection|List properties and relationships of the [plannerGroup](../resources/plannergroup.md) objects.|
|[Get plannerGroup](../api/plannergroup-get.md)|[plannerGroup](../resources/plannerGroup.md)|Read properties and relationships of the [plannerGroup](../resources/plannergroup.md) object.|
|[Create plannerGroup](../api/plannergroup-create.md)|[plannerGroup](../resources/plannerGroup.md)|Create a new [plannerGroup](../resources/plannergroup.md) object.|
|[Delete plannerGroup](../api/plannergroup-delete.md)|None|Deletes a [plannerGroup](../resources/plannergroup.md).|
|[Update plannerGroup](../api/plannergroup-update.md)|[plannerGroup](../resources/plannerGroup.md)|Update the properties of a [plannerGroup](../resources/plannergroup.md) object.|
|[List plans](../api/plannergroup-list-plans.md)|[plannerPlan](../resources/plannerPlan.md) collection|Get the plannerPlans from the plans navigation property.|
|[Create plans](../api/plannergroup-post-plans.md)|[plannerPlan](../resources/plannerPlan.md)|Create plans by posting to the plans collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|plans|[plannerPlan](../resources/plannerPlan.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerGroup",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerGroup",
  "id": "String (identifier)"
}
```

