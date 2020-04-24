---
title: "termsAndConditionsGroupAssignment resource type"
description: "A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group. Users in the group will be required to accept the terms in order to have devices enrolled into Intune."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# termsAndConditionsGroupAssignment resource type


Namespace: microsoft.graph

A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group. Users in the group will be required to accept the terms in order to have devices enrolled into Intune.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get termsAndConditionsGroupAssignment](../api/termsandconditionsgroupassignment-get.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md)|Read the properties and relationships of a [termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) object.|
|[Update termsAndConditionsGroupAssignment](../api/termsandconditionsgroupassignment-update.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md)|Update the properties of a [termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) object.|
|[List termsAndConditions](../api/termsandconditionsgroupassignment-list-termsandconditions.md)|[termsAndConditions](../resources/termsandconditions.md) collection|Get the termsAndConditions from the termsAndConditions navigation property.|
|[Add termsAndConditions](../api/termsandconditionsgroupassignment-post-termsandconditions.md)|[termsAndConditions](../resources/termsandconditions.md)|Add termsAndConditions by posting to the termsAndConditions collection.|
|[Remove termsAndConditions](../api/termsandconditionsgroupassignment-delete-termsandconditions.md)|None|Remove a [termsAndConditions](../resources/termsandconditions.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
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

