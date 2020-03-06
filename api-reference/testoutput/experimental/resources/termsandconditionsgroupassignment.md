---
title: "termsAndConditionsGroupAssignment resource type"
description: "A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group. Users in the group will be required to accept the terms in order to have devices enrolled into Intune."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# termsAndConditionsGroupAssignment resource type


Namespace: microsoft.graph

A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group. Users in the group will be required to accept the terms in order to have devices enrolled into Intune.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get termsAndConditionsGroupAssignment](../api/termsandconditionsgroupassignment-get.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md)|Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) object.|
|[Update termsAndConditionsGroupAssignment](../api/termsandconditionsgroupassignment-update.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md)|Update the properties of a [termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) object.|
|[Get termsAndConditions](../api/termsandconditions-get.md)|[termsAndConditions](../resources/termsandconditions.md)|Read properties and relationships of the [termsAndConditions](../resources/termsandconditions.md) object.|
|[List groupAssignments](../api/termsandconditions-list-groupassignments.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) collection|Get the termsAndConditionsGroupAssignments from the groupAssignments navigation property.|
|[Add groupAssignments](../api/termsandconditions-post-groupassignments.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md)|Add groupAssignments by posting to the groupAssignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|targetGroupId|String|Unique identifier of a group that the T&C policy is assigned to.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|termsAndConditions|[termsAndConditions](../resources/termsandconditions.md)|Navigation link to the terms and conditions that are assigned.|

## JSON representation
Here is a JSON representation of the resource.
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

