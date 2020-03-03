---
title: "educationCategory resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationCategory resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List educationCategories](../api/educationcategory-list.md)|[educationCategory](../resources/educationcategory.md) collection|List properties and relationships of the [educationCategory](../resources/educationcategory.md) objects.|
|[Get educationCategory](../api/educationcategory-get.md)|[educationCategory](../resources/educationcategory.md)|Read properties and relationships of the [educationCategory](../resources/educationcategory.md) object.|
|[Create educationCategory](../api/educationcategory-create.md)|[educationCategory](../resources/educationcategory.md)|Create a new [educationCategory](../resources/educationcategory.md) object.|
|[Delete educationCategory](../api/educationcategory-delete.md)|None|Deletes a [educationCategory](../resources/educationcategory.md).|
|[Update educationCategory](../api/educationcategory-update.md)|[educationCategory](../resources/educationcategory.md)|Update the properties of a [educationCategory](../resources/educationcategory.md) object.|

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

