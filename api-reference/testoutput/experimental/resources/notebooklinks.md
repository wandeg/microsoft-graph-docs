---
title: "notebookLinks resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# notebookLinks resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|oneNoteClientUrl|[externalLink](../resources/externalLink.md)||
|oneNoteWebUrl|[externalLink](../resources/externalLink.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.notebookLinks"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.notebookLinks",
  "oneNoteClientUrl": {
    "@odata.type": "microsoft.graph.externalLink",
    "href": "String"
  },
  "oneNoteWebUrl": {
    "@odata.type": "microsoft.graph.externalLink"
  }
}
```

