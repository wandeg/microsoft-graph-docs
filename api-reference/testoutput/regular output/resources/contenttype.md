---
title: "contentType resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# contentType resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get contentType](../api/contenttype-get.md)|[contentType](../resources/contentType.md)|Read properties and relationships of the [contentType](../resources/contenttype.md) object.|
|[Delete contentType](../api/contenttype-delete.md)|None|Deletes a [contentType](../resources/contenttype.md).|
|[Update contentType](../api/contenttype-update.md)|[contentType](../resources/contentType.md)|Update the properties of a [contentType](../resources/contenttype.md) object.|
|[List columnLinks](../api/contenttype-list-columnlinks.md)|[columnLink](../resources/columnLink.md) collection|Get the columnLinks from the columnLinks navigation property.|
|[Add columnLinks](../api/contenttype-post-columnlinks.md)|[columnLink](../resources/columnLink.md)|Add columnLinks by posting to the columnLinks collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
|group|String||
|hidden|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|inheritedFrom|[itemReference](../resources/itemReference.md)||
|name|String||
|order|[contentTypeOrder](../resources/contentTypeOrder.md)||
|parentId|String||
|readOnly|Boolean||
|sealed|Boolean||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|columnLinks|[columnLink](../resources/columnLink.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contentType",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.contentType",
  "id": "String (identifier)",
  "description": "String",
  "group": "String",
  "hidden": true,
  "inheritedFrom": {
    "@odata.type": "microsoft.graph.itemReference",
    "driveId": "String",
    "driveType": "String",
    "id": "String",
    "path": "String",
    "shareId": "String",
    "sharepointIds": {
      "@odata.type": "microsoft.graph.sharepointIds",
      "listId": "String",
      "listItemId": "String",
      "listItemUniqueId": "String",
      "siteId": "String",
      "siteUrl": "String",
      "webId": "String"
    }
  },
  "name": "String",
  "order": {
    "@odata.type": "microsoft.graph.contentTypeOrder",
    "default": true,
    "position": 1024
  },
  "parentId": "String",
  "readOnly": true,
  "sealed": true
}
```

