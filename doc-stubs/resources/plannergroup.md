---
title: "plannerGroup resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# plannerGroup resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List planner](../api/group-list-planner.md)|[plannerGroup](../resources/plannergroup.md) collection|Get the plannerGroups from the planner navigation property.|
|[Create planner](../api/group-post-planner.md)|[plannerGroup](../resources/plannergroup.md)|Create a new planner object.|
|[Delete planner](../api/group-delete-planner.md)|None|Delete a [plannerGroup](../resources/plannergroup.md) object.|
|[Update planner](../api/group-update-planner.md)|[plannerGroup](../resources/plannergroup.md)|Update the properties of a planner object.|
|[Get planner](../api/group-get-plannergroup.md)|[plannerGroup](../resources/plannergroup.md)|Read the properties and relationships of a [plannerGroup](../resources/plannergroup.md) object.|
|[List plans](../api/plannergroup-list-plans.md)|[plannerPlan](../resources/plannerplan.md) collection|Get the plannerPlans from the plans navigation property.|
|[Add plans](../api/plannergroup-post-plans.md)|[plannerPlan](../resources/plannerplan.md)|Add plans by posting to the plans collection.|
|[Remove plans](../api/plannergroup-delete-plans.md)|None|Remove a [plannerPlan](../resources/plannerplan.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|plans|[plannerPlan](../resources/plannerplan.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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

