---
title: "meetingTimeSuggestionsResult resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# meetingTimeSuggestionsResult resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|emptySuggestionsReason|String|**TODO: Add Description**|
|meetingTimeSuggestions|[meetingTimeSuggestion](../resources/meetingtimesuggestion.md) collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.meetingTimeSuggestionsResult",
  "meetingTimeSuggestions": [
    {
      "@odata.type": "microsoft.graph.meetingTimeSuggestion",
      "confidence": "Double",
      "order": 1024,
      "organizerAvailability": "String",
      "attendeeAvailability": [
        {
          "@odata.type": "microsoft.graph.attendeeAvailability",
          "attendee": {
            "@odata.type": "microsoft.graph.attendeeBase",
            "emailAddress": {
              "@odata.type": "microsoft.graph.emailAddress",
              "name": "String",
              "address": "String"
            },
            "type": "String"
          },
          "availability": "String"
        }
      ],
      "locations": [
        {
          "@odata.type": "microsoft.graph.location",
          "displayName": "String",
          "locationEmailAddress": "String",
          "address": {
            "@odata.type": "microsoft.graph.physicalAddress",
            "type": "String",
            "postOfficeBox": "String",
            "street": "String",
            "city": "String",
            "state": "String",
            "countryOrRegion": "String",
            "postalCode": "String"
          },
          "coordinates": {
            "@odata.type": "microsoft.graph.outlookGeoCoordinates",
            "altitude": "Double",
            "latitude": "Double",
            "longitude": "Double",
            "accuracy": "Double",
            "altitudeAccuracy": "Double"
          },
          "locationUri": "String",
          "locationType": "String",
          "uniqueId": "String",
          "uniqueIdType": "String"
        }
      ],
      "suggestionReason": "String",
      "meetingTimeSlot": {
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
  ],
  "emptySuggestionsReason": "String"
}
```

