---
title: "Education resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# Education resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|degreeName|String||
|description|String||
|fieldOfStudy|String||
|location|String||
|logo|String||
|name|String||
|startEndDate|[DateRange](../resources/daterange.md)||
|url|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.Education"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.Education",
  "name": "String",
  "logo": "String",
  "url": "String",
  "location": "String",
  "degreeName": "String",
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
  "fieldOfStudy": "String",
  "description": "String"
}
```

