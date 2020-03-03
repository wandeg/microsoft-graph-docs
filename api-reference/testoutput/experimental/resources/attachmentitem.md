---
title: "attachmentItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# attachmentItem resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|attachmentType|Enumeration|. Possible values are: `file`, `item`, `reference`.|
|contentType|String||
|isInline|Boolean||
|name|String||
|size|Int64||

## Relationships
None

## JSON Representation
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

