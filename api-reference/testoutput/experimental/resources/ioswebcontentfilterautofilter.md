---
title: "iosWebContentFilterAutoFilter resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# iosWebContentFilterAutoFilter resource type




Inherits from [iosWebContentFilterBase](../resources/iosWebContentFilterBase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedUrls|String collection|Additional URLs allowed for access|
|blockedUrls|String collection|Additional URLs blocked for access|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterAutoFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterAutoFilter",
  "allowedUrls": [
    "String"
  ],
  "blockedUrls": [
    "String"
  ]
}
```

