---
title: "folder resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# folder resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|childCount|Int32||
|view|[folderView](../resources/folderView.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.folder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.folder",
  "childCount": 1024,
  "view": {
    "@odata.type": "microsoft.graph.folderView",
    "sortBy": "String",
    "sortOrder": "String",
    "viewType": "String"
  }
}
```

