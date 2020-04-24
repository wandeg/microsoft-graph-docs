---
title: "onenotePatchContentCommand resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# onenotePatchContentCommand resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|onenotePatchActionType|**TODO: Add Description**. Possible values are: `Replace`, `Append`, `Delete`, `Insert`, `Prepend`.|
|content|String|**TODO: Add Description**|
|position|onenotePatchInsertPosition|**TODO: Add Description**. Possible values are: `After`, `Before`.|
|target|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.onenotePatchContentCommand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onenotePatchContentCommand",
  "action": "String",
  "target": "String",
  "content": "String",
  "position": "String"
}
```

