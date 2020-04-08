---
title: "termsAndConditionsGroupAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# termsAndConditionsGroupAssignment resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get termsAndConditionsGroupAssignment](../api/termsandconditionsgroupassignment-get.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md)|Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) object.|
|[Update termsAndConditionsGroupAssignment](../api/termsandconditionsgroupassignment-update.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md)|Update the properties of a [termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) object.|
|[Get termsAndConditions](../api/termsandconditions-get.md)|[termsAndConditions](../resources/termsandconditions.md)|Read properties and relationships of the [termsAndConditions](../resources/termsandconditions.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|targetGroupId|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|termsAndConditions|[termsAndConditions](../resources/termsandconditions.md)||

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

