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
|[Get educationCategory](../api/educationcategory-get.md)|[educationCategory](../resources/educationcategory.md)|Read properties and relationships of the [educationCategory](../resources/educationcategory.md) object.|
|[Update educationCategory](../api/educationcategory-update.md)|[educationCategory](../resources/educationcategory.md)|Update the properties of a [educationCategory](../resources/educationcategory.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
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

