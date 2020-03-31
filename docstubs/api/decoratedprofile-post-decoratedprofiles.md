---
title: "Create DecoratedProfile"
description: "Create a new DecoratedProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create DecoratedProfile

Namespace: microsoft.graph

Create a new [DecoratedProfile](../resources/decoratedprofile.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /decoratedProfiles
POST /decoratedProfileSearchResults/{decoratedProfileSearchResultsId}/profiles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [DecoratedProfile](../resources/decoratedprofile.md) object.

The following table shows the properties that are required when you create the [DecoratedProfile](../resources/decoratedprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|profileUrl|String||
|firstName|String||
|lastName|String||
|headline|String||
|industryName|String||
|summary|String||
|location|String||
|picture|String||
|recentPositions|[Position](../resources/position.md) collection||
|totalPositionCount|Int32||
|recentEducations|[Education](../resources/education.md) collection||
|totalEducationCount|Int32||
|skills|String collection||
|emails|String collection||
|phoneNumbers|[PhoneNumber](../resources/phonenumber.md) collection||
|ims|[IM](../resources/im.md) collection||
|websites|[liWebsite](../resources/liwebsite.md) collection||
|bornOn|[Date](../resources/date.md)||
|locale|[Locale](../resources/locale.md)||
|connection|[Connection](../resources/connection.md)||
|connected|Boolean||
|connectionDegree|Enumeration| Possible values are: `OUT_OF_NETWORK`, `SELF`, `DISTANCE_1`, `DISTANCE_2`, `DISTANCE_3`.|
|invitationSentFromViewer|Boolean||
|pendingInvitationSentFromViewee|[liInvitation](../resources/liinvitation.md)||
|simpleProfileHighlights|[SimpleProfileHighlight](../resources/simpleprofilehighlight.md) collection||
|profileHighlights|[DecoratedProfileProfileHighlights](../resources/decoratedprofileprofilehighlights.md) collection||
|viewerCanConnectViewee|Boolean||
|viewerCanFollowViewee|Boolean||
|salesNavigatorInfo|[SalesNavigatorInfo](../resources/salesnavigatorinfo.md)||



## Response
If successful, this method returns a `201 Created` response code and a [DecoratedProfile](../resources/decoratedprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_decoratedprofile_from_decoratedprofiles"
}
-->
``` http
POST https://graph.microsoft.com/beta/decoratedProfiles
Content-type: application/json
Content-length: 5997

{
  "@odata.type": "#microsoft.graph.DecoratedProfile",
  "profileUrl": "https://example.com/profileUrl/",
  "firstName": "First Name value",
  "lastName": "Last Name value",
  "headline": "Headline value",
  "industryName": "Industry Name value",
  "summary": "Summary value",
  "location": "Location value",
  "picture": "Picture value",
  "recentPositions": [
    {
      "@odata.type": "microsoft.graph.Position",
      "name": "Name value",
      "logo": "Logo value",
      "url": "Url value",
      "title": "Title value",
      "startEndDate": {
        "@odata.type": "microsoft.graph.DateRange",
        "start": {
          "@odata.type": "microsoft.graph.Date",
          "day": 3,
          "month": 5,
          "year": 4
        },
        "end": {
          "@odata.type": "microsoft.graph.Date"
        }
      },
      "description": "Description value"
    }
  ],
  "totalPositionCount": 2,
  "recentEducations": [
    {
      "@odata.type": "microsoft.graph.Education",
      "degreeName": "Degree Name value",
      "fieldOfStudy": "Field Of Study value"
    }
  ],
  "totalEducationCount": 3,
  "skills": [
    "Skills value"
  ],
  "emails": [
    "Emails value"
  ],
  "phoneNumbers": [
    {
      "@odata.type": "microsoft.graph.PhoneNumber",
      "number": "Number value",
      "extension": "Extension value",
      "type": "String"
    }
  ],
  "ims": [
    {
      "@odata.type": "microsoft.graph.IM",
      "id": "Id value",
      "provider": "Provider value"
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
    "language": "Language value",
    "country": "Country value",
    "variant": "Variant value"
  },
  "connection": {
    "@odata.type": "microsoft.graph.Connection",
    "count": 5,
    "countObfuscated": true
  },
  "connected": true,
  "connectionDegree": "String",
  "invitationSentFromViewer": true,
  "pendingInvitationSentFromViewee": {
    "@odata.type": "microsoft.graph.liInvitation",
    "invitationId": "Invitation Id value",
    "validationToken": "Validation Token value"
  },
  "simpleProfileHighlights": [
    {
      "@odata.type": "microsoft.graph.SimpleProfileHighlight",
      "detail": "Detail value",
      "type": "String",
      "link": "Link value"
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
        "totalCount": 10,
        "sharedConnectionPage": "Shared Connection Page value"
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
                  "numDays": 7,
                  "numMonths": 9,
                  "numYears": 8
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
        "numberOfYears": 13
      }
    }
  ],
  "viewerCanConnectViewee": true,
  "viewerCanFollowViewee": true,
  "salesNavigatorInfo": {
    "@odata.type": "microsoft.graph.SalesNavigatorInfo",
    "teamlinkInfo": {
      "@odata.type": "microsoft.graph.SalesNavigatorTeamlinkInfo",
      "countOfTotalTeamlinkConnections": 15,
      "teamlinkSearchUrl": "https://example.com/teamlinkSearchUrl/",
      "topTeamlinks": [
        {
          "@odata.type": "microsoft.graph.SalesNavigatorPersonInfo",
          "photoUrl": "https://example.com/photoUrl/"
        }
      ]
    },
    "insights": [
      {
        "@odata.type": "microsoft.graph.SalesNavigatorInsight",
        "createdAt": 9,
        "insightType": "String",
        "insightUrl": "https://example.com/insightUrl/",
        "person": {
          "@odata.type": "microsoft.graph.SalesNavigatorPersonInfo"
        }
      }
    ],
    "savedLead": true,
    "savedAccount": {
      "@odata.type": "microsoft.graph.LinkedInOrganization"
    },
    "contractName": "Contract Name value",
    "contractChooserUrl": "https://example.com/contractChooserUrl/"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.decoratedprofile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 6046

{
  "@odata.type": "#microsoft.graph.DecoratedProfile",
  "id": "95a8fc58-fc58-95a8-58fc-a89558fca895",
  "profileUrl": "https://example.com/profileUrl/",
  "firstName": "First Name value",
  "lastName": "Last Name value",
  "headline": "Headline value",
  "industryName": "Industry Name value",
  "summary": "Summary value",
  "location": "Location value",
  "picture": "Picture value",
  "recentPositions": [
    {
      "@odata.type": "microsoft.graph.Position",
      "name": "Name value",
      "logo": "Logo value",
      "url": "Url value",
      "title": "Title value",
      "startEndDate": {
        "@odata.type": "microsoft.graph.DateRange",
        "start": {
          "@odata.type": "microsoft.graph.Date",
          "day": 3,
          "month": 5,
          "year": 4
        },
        "end": {
          "@odata.type": "microsoft.graph.Date"
        }
      },
      "description": "Description value"
    }
  ],
  "totalPositionCount": 2,
  "recentEducations": [
    {
      "@odata.type": "microsoft.graph.Education",
      "degreeName": "Degree Name value",
      "fieldOfStudy": "Field Of Study value"
    }
  ],
  "totalEducationCount": 3,
  "skills": [
    "Skills value"
  ],
  "emails": [
    "Emails value"
  ],
  "phoneNumbers": [
    {
      "@odata.type": "microsoft.graph.PhoneNumber",
      "number": "Number value",
      "extension": "Extension value",
      "type": "String"
    }
  ],
  "ims": [
    {
      "@odata.type": "microsoft.graph.IM",
      "id": "Id value",
      "provider": "Provider value"
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
    "language": "Language value",
    "country": "Country value",
    "variant": "Variant value"
  },
  "connection": {
    "@odata.type": "microsoft.graph.Connection",
    "count": 5,
    "countObfuscated": true
  },
  "connected": true,
  "connectionDegree": "String",
  "invitationSentFromViewer": true,
  "pendingInvitationSentFromViewee": {
    "@odata.type": "microsoft.graph.liInvitation",
    "invitationId": "Invitation Id value",
    "validationToken": "Validation Token value"
  },
  "simpleProfileHighlights": [
    {
      "@odata.type": "microsoft.graph.SimpleProfileHighlight",
      "detail": "Detail value",
      "type": "String",
      "link": "Link value"
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
        "totalCount": 10,
        "sharedConnectionPage": "Shared Connection Page value"
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
                  "numDays": 7,
                  "numMonths": 9,
                  "numYears": 8
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
        "numberOfYears": 13
      }
    }
  ],
  "viewerCanConnectViewee": true,
  "viewerCanFollowViewee": true,
  "salesNavigatorInfo": {
    "@odata.type": "microsoft.graph.SalesNavigatorInfo",
    "teamlinkInfo": {
      "@odata.type": "microsoft.graph.SalesNavigatorTeamlinkInfo",
      "countOfTotalTeamlinkConnections": 15,
      "teamlinkSearchUrl": "https://example.com/teamlinkSearchUrl/",
      "topTeamlinks": [
        {
          "@odata.type": "microsoft.graph.SalesNavigatorPersonInfo",
          "photoUrl": "https://example.com/photoUrl/"
        }
      ]
    },
    "insights": [
      {
        "@odata.type": "microsoft.graph.SalesNavigatorInsight",
        "createdAt": 9,
        "insightType": "String",
        "insightUrl": "https://example.com/insightUrl/",
        "person": {
          "@odata.type": "microsoft.graph.SalesNavigatorPersonInfo"
        }
      }
    ],
    "savedLead": true,
    "savedAccount": {
      "@odata.type": "microsoft.graph.LinkedInOrganization"
    },
    "contractName": "Contract Name value",
    "contractChooserUrl": "https://example.com/contractChooserUrl/"
  }
}
```

