---
title: "mediaPrompt resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mediaPrompt resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [prompt](../resources/prompt.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|mediaInfo|[mediaInfo](../resources/mediainfo.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

