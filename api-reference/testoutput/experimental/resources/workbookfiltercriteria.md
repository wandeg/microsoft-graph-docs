---
title: "workbookFilterCriteria resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookFilterCriteria resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|color|String||
|criterion1|String||
|criterion2|String||
|dynamicCriteria|String||
|filterOn|String||
|icon|[workbookIcon](../resources/workbookIcon.md)||
|operator|String||
|values|[Json](../resources/Json.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.workbookFilterCriteria"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookFilterCriteria",
  "color": "String",
  "criterion1": "String",
  "criterion2": "String",
  "dynamicCriteria": "String",
  "filterOn": "String",
  "icon": {
    "@odata.type": "microsoft.graph.workbookIcon",
    "index": 1024,
    "set": "String"
  },
  "operator": "String",
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

