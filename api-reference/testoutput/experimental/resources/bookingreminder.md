---
title: "bookingReminder resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# bookingReminder resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|message|String|Message to send.|
|offset|Duration|How much time before an appointment the reminder should be sent.|
|recipients|Enumeration|Who should receive the reminder. Possible values are: `allAttendees`, `staff`, `customer`.|

## Relationships
None

## JSON Representation
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

