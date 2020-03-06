---
title: "calendarSharingMessageAction resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# calendarSharingMessageAction resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|Enumeration|. Possible values are: `accept`, `acceptAndViewCalendar`, `viewCalendar`, `addThisCalendar`.|
|actionType|Enumeration|. Possible values are: `accept`.|
|importance|Enumeration|. Possible values are: `primary`, `secondary`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.calendarSharingMessageAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.calendarSharingMessageAction",
  "importance": "String",
  "actionType": "String",
  "action": "String"
}
```

