---
title: "attachmentItem resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# attachmentItem resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|attachmentType|attachmentType|**TODO: Add Description**. Possible values are: `file`, `item`, `reference`.|
|contentType|String|**TODO: Add Description**|
|isInline|Boolean|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|size|Int64|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attachmentItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attachmentItem",
  "attachmentType": "String",
  "name": "String",
  "size": 1024,
  "contentType": "String",
  "isInline": true
}
```

