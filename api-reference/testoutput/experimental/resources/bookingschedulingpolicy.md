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
|allowStaffSelection|Boolean|Allow customers to choose a specific person for the booking.|
|maximumAdvance|Duration|Maximum number of days in advance that a booking can be made.|
|minimumLeadTime|Duration|Minimum lead time for bookings and cancellations.|
|sendConfirmationsToOwner|Boolean|Notify the business via email when a booking is created or changed.|
|timeSlotInterval|Duration|Duration of each time slot.|

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

