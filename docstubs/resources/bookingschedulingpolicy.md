---
title: "bookingSchedulingPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# bookingSchedulingPolicy resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowStaffSelection|Boolean||
|maximumAdvance|Duration||
|minimumLeadTime|Duration||
|sendConfirmationsToOwner|Boolean||
|timeSlotInterval|Duration||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bookingSchedulingPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingSchedulingPolicy",
  "timeSlotInterval": "String (duration)",
  "minimumLeadTime": "String (duration)",
  "maximumAdvance": "String (duration)",
  "sendConfirmationsToOwner": true,
  "allowStaffSelection": true
}
```

