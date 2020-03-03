---
title: "educationCategory resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# educationCategory resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationCategory](../api/educationcategory-get.md)|[educationCategory](../resources/educationCategory.md)|Read properties and relationships of the [educationCategory](../resources/educationcategory.md) object.|
|[Delete educationCategory](../api/educationcategory-delete.md)|None|Deletes a [educationCategory](../resources/educationcategory.md).|
|[Update educationCategory](../api/educationcategory-update.md)|[educationCategory](../resources/educationCategory.md)|Update the properties of a [educationCategory](../resources/educationcategory.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationCategory",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationCategory",
  "id": "String (identifier)",
  "displayName": "String"
}
```

