---
title: "DecoratedProfileMapElement resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# DecoratedProfileMapElement resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|key|String||
|value|[DecoratedProfile](../resources/decoratedprofile.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.DecoratedProfileMapElement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.DecoratedProfileMapElement",
  "key": "String",
  "value": {
    "@odata.type": "#microsoft.graph.DecoratedProfile",
    "id": "String (identifier)",
    "profileUrl": "String",
    "firstName": "String",
    "lastName": "String",
    "headline": "String",
    "industryName": "String",
    "summary": "String",
    "location": "String",
    "picture": "String",
    "recentPositions": [
      {
        "@odata.type": "microsoft.graph.Position",
        "name": "String",
        "logo": "String",
        "url": "String",
        "title": "String",
        "startEndDate": {
          "@odata.type": "microsoft.graph.DateRange",
          "start": {
            "@odata.type": "microsoft.graph.Date",
            "day": 1024,
            "month": 1024,
            "year": 1024
          },
          "end": {
            "@odata.type": "microsoft.graph.Date"
          }
        },
        "description": "String"
      }
    ],
    "totalPositionCount": 1024,
    "recentEducations": [
      {
        "@odata.type": "microsoft.graph.Education",
        "degreeName": "String",
        "fieldOfStudy": "String"
      }
    ],
    "totalEducationCount": 1024,
    "skills": [
      "String"
    ],
    "emails": [
      "String"
    ],
    "phoneNumbers": [
      {
        "@odata.type": "microsoft.graph.PhoneNumber",
        "number": "String",
        "extension": "String",
        "type": "String"
      }
    ],
    "ims": [
      {
        "@odata.type": "microsoft.graph.IM",
        "id": "String",
        "provider": "String"
      }
    ],
    "websites": [
      {
        "@odata.type": "microsoft.graph.liWebsite",
        "category": "String"
      }
    ],
    "bornOn": {
      "@odata.type": "microsoft.graph.Date"
    },
    "locale": {
      "@odata.type": "microsoft.graph.Locale",
      "language": "String",
      "country": "String",
      "variant": "String"
    },
    "connection": {
      "@odata.type": "microsoft.graph.Connection",
      "count": 1024,
      "countObfuscated": true
    },
    "connected": true,
    "connectionDegree": "String",
    "invitationSentFromViewer": true,
    "pendingInvitationSentFromViewee": {
      "@odata.type": "microsoft.graph.liInvitation",
      "invitationId": "String",
      "validationToken": "String"
    },
    "simpleProfileHighlights": [
      {
        "@odata.type": "microsoft.graph.SimpleProfileHighlight",
        "detail": "String",
        "type": "String",
        "link": "String"
      }
    ],
    "profileHighlights": [
      {
        "@odata.type": "microsoft.graph.DecoratedProfileProfileHighlights",
        "birthday": {
          "@odata.type": "microsoft.graph.Birthday",
          "celebratedOn": {
            "@odata.type": "microsoft.graph.Date"
          }
        },
        "meetNewHire": {
          "@odata.type": "microsoft.graph.MeetNewHire",
          "hiredOn": {
            "@odata.type": "microsoft.graph.Date"
          }
        },
        "positionChange": {
          "@odata.type": "microsoft.graph.PositionChange",
          "newPosition": {
            "@odata.type": "microsoft.graph.Position"
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
              "@odata.type": "microsoft.graph.SharedConnection"
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
    ],
    "viewerCanConnectViewee": true,
    "viewerCanFollowViewee": true,
    "salesNavigatorInfo": {
      "@odata.type": "microsoft.graph.SalesNavigatorInfo",
      "teamlinkInfo": {
        "@odata.type": "microsoft.graph.SalesNavigatorTeamlinkInfo",
        "countOfTotalTeamlinkConnections": 1024,
        "teamlinkSearchUrl": "String",
        "topTeamlinks": [
          {
            "@odata.type": "microsoft.graph.SalesNavigatorPersonInfo",
            "photoUrl": "String"
          }
        ]
      },
      "insights": [
        {
          "@odata.type": "microsoft.graph.SalesNavigatorInsight",
          "createdAt": 1024,
          "insightType": "String",
          "insightUrl": "String",
          "person": {
            "@odata.type": "microsoft.graph.SalesNavigatorPersonInfo"
          }
        }
      ],
      "savedLead": true,
      "savedAccount": {
        "@odata.type": "microsoft.graph.LinkedInOrganization"
      },
      "contractName": "String",
      "contractChooserUrl": "String"
    }
  }
}
```

