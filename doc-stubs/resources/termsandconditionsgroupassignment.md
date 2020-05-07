---
title: "termsAndConditionsGroupAssignment resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# termsAndConditionsGroupAssignment resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List termsAndConditions](../api/termsandconditionsgroupassignment-list-termsandconditions.md)|[termsAndConditions](../resources/termsandconditions.md) collection|Get the termsAndConditions from the termsAndConditions navigation property.|
|[Add termsAndConditions](../api/termsandconditionsgroupassignment-post-termsandconditions.md)|[termsAndConditions](../resources/termsandconditions.md)|Add termsAndConditions by posting to the termsAndConditions collection.|
|[Remove termsAndConditions](../api/termsandconditionsgroupassignment-delete-termsandconditions.md)|None|Remove a [termsAndConditions](../resources/termsandconditions.md) object.|
|[List groupAssignments](../api/termsandconditions-list-groupassignments.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) collection|Get the termsAndConditionsGroupAssignments from the groupAssignments navigation property.|
|[Create groupAssignments](../api/termsandconditions-post-groupassignments.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md)|Create a new groupAssignments object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|targetGroupId|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|termsAndConditions|[termsAndConditions](../resources/termsandconditions.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsGroupAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```

