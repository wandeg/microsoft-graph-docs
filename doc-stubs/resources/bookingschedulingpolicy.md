---
title: "bookingSchedulingPolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# bookingSchedulingPolicy resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowStaffSelection|Boolean|**TODO: Add Description**|
|maximumAdvance|Duration|**TODO: Add Description**|
|minimumLeadTime|Duration|**TODO: Add Description**|
|sendConfirmationsToOwner|Boolean|**TODO: Add Description**|
|timeSlotInterval|Duration|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "sendConfirmationsToOwner": "Boolean",
  "allowStaffSelection": "Boolean"
}
```

