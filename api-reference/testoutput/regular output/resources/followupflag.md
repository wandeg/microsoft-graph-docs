---
title: "followupFlag resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# followupFlag resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedDateTime|[dateTimeTimeZone](../resources/dateTimeTimeZone.md)||
|dueDateTime|[dateTimeTimeZone](../resources/dateTimeTimeZone.md)||
|flagStatus|Enumeration|. Possible values are: `notFlagged`, `complete`, `flagged`.|
|startDateTime|[dateTimeTimeZone](../resources/dateTimeTimeZone.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.followupFlag"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.followupFlag",
  "completedDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone",
    "dateTime": "String",
    "timeZone": "String"
  },
  "dueDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "startDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "flagStatus": "String"
}
```

