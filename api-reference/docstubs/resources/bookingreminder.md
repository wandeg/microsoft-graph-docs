---
title: "bookingReminder resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# bookingReminder resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|message|String|Message to send.|
|offset|Duration|How much time before an appointment the reminder should be sent.|
|recipients|bookingReminderRecipients|Who should receive the reminder. Possible values are: `allAttendees`, `staff`, `customer`.|

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

