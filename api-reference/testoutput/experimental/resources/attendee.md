---
title: "attendee resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# attendee resource type




Inherits from [attendeeBase](../resources/attendeeBase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|emailAddress|[emailAddress](../resources/emailAddress.md)| Inherited from [recipient](../resources/recipient.md)|
|proposedNewTime|[timeSlot](../resources/timeSlot.md)||
|status|[responseStatus](../resources/responseStatus.md)||
|type|Enumeration| Inherited from [attendeeBase](../resources/attendeeBase.md). Possible values are: `required`, `optional`, `resource`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attendee"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attendee",
  "emailAddress": {
    "@odata.type": "microsoft.graph.emailAddress",
    "name": "String",
    "address": "String"
  },
  "type": "String",
  "status": {
    "@odata.type": "microsoft.graph.responseStatus",
    "response": "String",
    "time": "String (timestamp)"
  },
  "proposedNewTime": {
    "@odata.type": "microsoft.graph.timeSlot",
    "start": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone",
      "dateTime": "String",
      "timeZone": "String"
    },
    "end": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    }
  }
}
```

