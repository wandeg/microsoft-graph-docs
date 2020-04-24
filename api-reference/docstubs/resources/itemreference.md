---
title: "itemReference resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# itemReference resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|driveId|String|**TODO: Add Description**|
|driveType|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|path|String|**TODO: Add Description**|
|shareId|String|**TODO: Add Description**|
|sharepointIds|[sharepointIds](../resources/sharepointids.md)|**TODO: Add Description**|
|siteId|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.itemReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemReference",
  "driveId": "String",
  "driveType": "String",
  "id": "String (identifier)",
  "name": "String",
  "path": "String",
  "shareId": "String",
  "sharepointIds": {
    "@odata.type": "microsoft.graph.sharepointIds",
    "listId": "String",
    "listItemId": "String",
    "listItemUniqueId": "String",
    "siteId": "String",
    "siteUrl": "String",
    "tenantId": "String",
    "webId": "String"
  },
  "siteId": "String"
}
```

