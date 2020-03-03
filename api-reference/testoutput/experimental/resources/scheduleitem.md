---
title: "scheduleItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# scheduleItem resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|end|[dateTimeTimeZone](../resources/dateTimeTimeZone.md)||
|isPrivate|Boolean||
|location|String||
|start|[dateTimeTimeZone](../resources/dateTimeTimeZone.md)||
|status|Enumeration|. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|
|subject|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.scheduleItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.scheduleItem",
  "start": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone",
    "dateTime": "String",
    "timeZone": "String"
  },
  "end": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "isPrivate": true,
  "status": "String",
  "subject": "String",
  "location": "String"
}
```

