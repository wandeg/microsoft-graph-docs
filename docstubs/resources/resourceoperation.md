---
title: "resourceOperation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# resourceOperation resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get resourceOperation](../api/resourceoperation-get.md)|[resourceOperation](../resources/resourceoperation.md)|Read properties and relationships of the [resourceOperation](../resources/resourceoperation.md) object.|
|[Update resourceOperation](../api/resourceoperation-update.md)|[resourceOperation](../resources/resourceoperation.md)|Update the properties of a [resourceOperation](../resources/resourceoperation.md) object.|
|[getScopesForUser](../api/resourceoperation-getscopesforuser.md)|String collection||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actionName|String||
|description|String||
|enabledForScopeValidation|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|resource|String||
|resourceName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "String (identifier)",
  "resource": "String",
  "resourceName": "String",
  "actionName": "String",
  "description": "String",
  "enabledForScopeValidation": true
}
```

