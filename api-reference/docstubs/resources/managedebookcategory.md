---
title: "managedEBookCategory resource type"
description: "Contains properties for a single Intune eBook category."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedEBookCategory resource type


Namespace: microsoft.graph

Contains properties for a single Intune eBook category.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedEBookCategory](../api/managedebookcategory-get.md)|[managedEBookCategory](../resources/managedebookcategory.md)|Read the properties and relationships of a [managedEBookCategory](../resources/managedebookcategory.md) object.|
|[Update managedEBookCategory](../api/managedebookcategory-update.md)|[managedEBookCategory](../resources/managedebookcategory.md)|Update the properties of a [managedEBookCategory](../resources/managedebookcategory.md) object.|
|[List categories](../api/managedebook-list-categories.md)|[managedEBookCategory](../resources/managedebookcategory.md) collection|Get the managedEBookCategories from the categories navigation property.|
|[Add categories](../api/managedebook-post-categories.md)|[managedEBookCategory](../resources/managedebookcategory.md)|Add categories by posting to the categories collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The name of the eBook category.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the ManagedEBookCategory was last modified.|

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

