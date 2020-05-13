---
title: "meetingTimeSuggestion resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# meetingTimeSuggestion resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|attendeeAvailability|[attendeeAvailability](../resources/attendeeavailability.md) collection|**TODO: Add Description**|
|confidence|Double|**TODO: Add Description**|
|locations|[location](../resources/location.md) collection|**TODO: Add Description**|
|meetingTimeSlot|[timeSlot](../resources/timeslot.md)|**TODO: Add Description**|
|order|Int32|**TODO: Add Description**|
|organizerAvailability|freeBusyStatus|**TODO: Add Description**. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|
|suggestionReason|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.meetingTimeSuggestion",
  "confidence": "Double",
  "order": "Integer",
  "organizerAvailability": "String",
  "attendeeAvailability": [
    {
      "@odata.type": "microsoft.graph.attendeeAvailability"
    }
  ],
  "locations": [
    {
      "@odata.type": "microsoft.graph.location"
    }
  ],
  "suggestionReason": "String",
  "meetingTimeSlot": {
    "@odata.type": "microsoft.graph.timeSlot"
  }
}
```

