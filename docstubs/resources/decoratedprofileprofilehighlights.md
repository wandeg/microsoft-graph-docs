---
title: "DecoratedProfileProfileHighlights resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# DecoratedProfileProfileHighlights resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|birthday|[Birthday](../resources/birthday.md)||
|meetNewHire|[MeetNewHire](../resources/meetnewhire.md)||
|positionChange|[PositionChange](../resources/positionchange.md)||
|sharedConnections|[SharedConnections](../resources/sharedconnections.md)||
|sharedEducations|[SharedEducations](../resources/sharededucations.md)||
|sharedExperiences|[SharedExperiences](../resources/sharedexperiences.md)||
|workAnniversary|[WorkAnniversary](../resources/workanniversary.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.DecoratedProfileProfileHighlights"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.DecoratedProfileProfileHighlights",
  "birthday": {
    "@odata.type": "microsoft.graph.Birthday",
    "celebratedOn": {
      "@odata.type": "microsoft.graph.Date",
      "day": 1024,
      "month": 1024,
      "year": 1024
    }
  },
  "meetNewHire": {
    "@odata.type": "microsoft.graph.MeetNewHire",
    "name": "String",
    "logo": "String",
    "url": "String",
    "location": "String",
    "hiredOn": {
      "@odata.type": "microsoft.graph.Date"
    }
  },
  "positionChange": {
    "@odata.type": "microsoft.graph.PositionChange",
    "newPosition": {
      "@odata.type": "microsoft.graph.Position",
      "title": "String",
      "startEndDate": {
        "@odata.type": "microsoft.graph.DateRange",
        "start": {
          "@odata.type": "microsoft.graph.Date"
        },
        "end": {
          "@odata.type": "microsoft.graph.Date"
        }
      },
      "description": "String"
    },
    "oldPosition": {
      "@odata.type": "microsoft.graph.Position"
    },
    "positionChangeType": "String"
  },
  "sharedConnections": {
    "@odata.type": "microsoft.graph.SharedConnections",
    "topSharedConnections": [
      {
        "@odata.type": "microsoft.graph.SharedConnection",
        "firstName": "String",
        "lastName": "String",
        "picture": "String"
      }
    ],
    "totalCount": 1024,
    "sharedConnectionPage": "String"
  },
  "sharedEducations": {
    "@odata.type": "microsoft.graph.SharedEducations",
    "sharedEducations": [
      {
        "@odata.type": "microsoft.graph.SharedEducation",
        "overlapInfo": {
          "@odata.type": "microsoft.graph.OverlapInfo",
          "detail": {
            "@odata.type": "microsoft.graph.OverlapInfoDetail",
            "dateRange": {
              "@odata.type": "microsoft.graph.DateRange"
            },
            "duration": {
              "@odata.type": "microsoft.graph.Duration",
              "numDays": 1024,
              "numMonths": 1024,
              "numYears": 1024
            }
          },
          "overlapType": "String"
        }
      }
    ]
  },
  "sharedExperiences": {
    "@odata.type": "microsoft.graph.SharedExperiences",
    "sharedExperiences": [
      {
        "@odata.type": "microsoft.graph.SharedExperience"
      }
    ]
  },
  "workAnniversary": {
    "@odata.type": "microsoft.graph.WorkAnniversary",
    "startedOn": {
      "@odata.type": "microsoft.graph.Date"
    },
    "numberOfYears": 1024
  }
}
```

