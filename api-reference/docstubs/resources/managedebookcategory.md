---
title: "managedEBookCategory resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedEBookCategory resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedEBookCategory](../api/managedebookcategory-get.md)|[managedEBookCategory](../resources/managedebookcategory.md)|Read properties and relationships of the [managedEBookCategory](../resources/managedebookcategory.md) object.|
|[Update managedEBookCategory](../api/managedebookcategory-update.md)|[managedEBookCategory](../resources/managedebookcategory.md)|Update the properties of a [managedEBookCategory](../resources/managedebookcategory.md) object.|
|[List categories](../api/managedebook-list-categories.md)|[managedEBookCategory](../resources/managedebookcategory.md) collection|Get the managedEBookCategories from the categories navigation property.|
|[Create categories](../api/managedebook-post-categories.md)|[managedEBookCategory](../resources/managedebookcategory.md)|Create categories by posting to the categories collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookCategory",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

