---
title: "SimpleProfileHighlight resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# SimpleProfileHighlight resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|detail|String||
|link|String||
|picture|String||
|title|String||
|type|Enumeration| Possible values are: `SharedConnections`, `SharedExperiences`, `SharedEducations`, `SharedGroups`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.SimpleProfileHighlight"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.SimpleProfileHighlight",
  "title": "String",
  "detail": "String",
  "type": "String",
  "picture": "String",
  "link": "String"
}
```

