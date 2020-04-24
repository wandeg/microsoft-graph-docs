---
title: "mobileAppCategory resource type"
description: "Contains properties for a single Intune app category."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mobileAppCategory resource type


Namespace: microsoft.graph

Contains properties for a single Intune app category.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get mobileAppCategory](../api/mobileappcategory-get.md)|[mobileAppCategory](../resources/mobileappcategory.md)|Read the properties and relationships of a [mobileAppCategory](../resources/mobileappcategory.md) object.|
|[Update mobileAppCategory](../api/mobileappcategory-update.md)|[mobileAppCategory](../resources/mobileappcategory.md)|Update the properties of a [mobileAppCategory](../resources/mobileappcategory.md) object.|
|[List categories](../api/mobileapp-list-categories.md)|[mobileAppCategory](../resources/mobileappcategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Add categories](../api/mobileapp-post-categories.md)|[mobileAppCategory](../resources/mobileappcategory.md)|Add categories by posting to the categories collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The name of the app category.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the mobileAppCategory was last modified.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppCategory",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

