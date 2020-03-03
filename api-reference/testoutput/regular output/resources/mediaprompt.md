---
title: "mediaPrompt resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# mediaPrompt resource type




Inherits from [prompt](../resources/prompt.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|mediaInfo|[mediaInfo](../resources/mediaInfo.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaPrompt"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaPrompt",
  "mediaInfo": {
    "@odata.type": "microsoft.graph.mediaInfo",
    "uri": "String",
    "resourceId": "String"
  }
}
```

