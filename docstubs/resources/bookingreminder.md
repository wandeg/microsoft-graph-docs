---
title: "bookingReminder resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# bookingReminder resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|message|String||
|offset|Duration||
|recipients|Enumeration| Possible values are: `allAttendees`, `staff`, `customer`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bookingReminder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingReminder",
  "offset": "String (duration)",
  "recipients": "String",
  "message": "String"
}
```

