---
title: "contentType resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# contentType resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get contentType](../api/contenttype-get.md)|[contentType](../resources/contenttype.md)|Read properties and relationships of a [contentType](../resources/contenttype.md) object.|
|[Update contentType](../api/contenttype-update.md)|[contentType](../resources/contenttype.md)|Update the properties of a [contentType](../resources/contenttype.md) object.|
|[List columnLinks](../api/contenttype-list-columnlinks.md)|[columnLink](../resources/columnlink.md) collection|Get the columnLinks from the columnLinks navigation property.|
|[Create columnLinks](../api/contenttype-post-columnlinks.md)|[columnLink](../resources/columnlink.md)|Create a new columnLinks object.|
|[Delete columnLinks](../api/contenttype-delete-columnlinks.md)|None|Delete a columnLinks object.|
|[Update columnLinks](../api/contenttype-update-columnlinks.md)|[columnLink](../resources/columnlink.md)|Update the properties of a columnLinks object.|
|[Get columnLink](../api/columnlink-get.md)|[columnLink](../resources/columnlink.md)|Read properties and relationships of a [columnLink](../resources/columnlink.md) object.|
|[List contentTypes](../api/site-list-contenttypes.md)|[contentType](../resources/contenttype.md) collection|Get the contentTypes from the contentTypes navigation property.|
|[Create contentTypes](../api/site-post-contenttypes.md)|[contentType](../resources/contenttype.md)|Create a new contentTypes object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|group|String|**TODO: Add Description**|
|hidden|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|inheritedFrom|[itemReference](../resources/itemreference.md)|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|order|[contentTypeOrder](../resources/contenttypeorder.md)|**TODO: Add Description**|
|parentId|String|**TODO: Add Description**|
|readOnly|Boolean|**TODO: Add Description**|
|sealed|Boolean|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|columnLinks|[columnLink](../resources/columnlink.md) collection|**TODO: Add Description**|

## JSON representation
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

