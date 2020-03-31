---
title: "Position resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# Position resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
|location|String||
|logo|String||
|name|String||
|startEndDate|[DateRange](../resources/daterange.md)||
|title|String||
|url|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.Position"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.Position",
  "name": "String",
  "logo": "String",
  "url": "String",
  "location": "String",
  "title": "String",
  "startEndDate": {
    "@odata.type": "microsoft.graph.DateRange",
    "start": {
      "@odata.type": "microsoft.graph.Date",
      "day": 1024,
      "month": 1024,
      "year": 1024
    },
    "end": {
      "@odata.type": "microsoft.graph.Date"
    }
  },
  "description": "String"
}
```

