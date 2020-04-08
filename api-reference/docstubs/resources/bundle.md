---
title: "bundle resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# bundle resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|album|[album](../resources/album.md)||
|childCount|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bundle"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bundle",
  "childCount": 1024,
  "album": {
    "@odata.type": "microsoft.graph.album",
    "coverImageItemId": "String"
  }
}
```

