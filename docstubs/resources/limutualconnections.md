---
title: "LIMutualConnections resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# LIMutualConnections resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|mutualConnections|[LIMemberDetails](../resources/limemberdetails.md) collection||
|mutualConnectionsPage|String||
|totalCount|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIMutualConnections"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIMutualConnections",
  "mutualConnections": [
    {
      "@odata.type": "microsoft.graph.LIMemberDetails",
      "id": "String",
      "firstName": {
        "@odata.type": "microsoft.graph.MultiLocaleString",
        "localized": [
          {
            "@odata.type": "microsoft.graph.StringMapElement",
            "key": "String",
            "value": "String"
          }
        ],
        "preferredLocale": {
          "@odata.type": "microsoft.graph.Locale",
          "language": "String",
          "country": "String",
          "variant": "String"
        }
      },
      "lastName": {
        "@odata.type": "microsoft.graph.MultiLocaleString"
      },
      "headline": {
        "@odata.type": "microsoft.graph.MultiLocaleString"
      },
      "summary": {
        "@odata.type": "microsoft.graph.MultiLocaleRichText",
        "localized": [
          {
            "@odata.type": "microsoft.graph.RichTextMapElement",
            "value": {
              "@odata.type": "microsoft.graph.RichText",
              "rawText": "String",
              "rtData": [
                {
                  "@odata.type": "microsoft.graph.RTData",
                  "type": "String",
                  "startIdx": 1024,
                  "endIdx": 1024,
                  "attribute": [
                    {
                      "@odata.type": "microsoft.graph.RTAttribute",
                      "name": "String"
                    }
                  ]
                }
              ]
            }
          }
        ]
      },
      "industryName": {
        "@odata.type": "microsoft.graph.MultiLocaleString"
      },
      "profilePicture": "String",
      "defaultLocale": {
        "@odata.type": "microsoft.graph.Locale"
      },
      "profileUrl": "String",
      "positions": [
        {
          "@odata.type": "microsoft.graph.LIMemberPosition",
          "title": {
            "@odata.type": "microsoft.graph.MultiLocaleString"
          },
          "description": {
            "@odata.type": "microsoft.graph.MultiLocaleRichText"
          },
          "startMonthYear": {
            "@odata.type": "microsoft.graph.Date",
            "day": 1024,
            "month": 1024,
            "year": 1024
          },
          "endMonthYear": {
            "@odata.type": "microsoft.graph.Date"
          },
          "company": {
            "@odata.type": "microsoft.graph.LIOrganization",
            "name": {
              "@odata.type": "microsoft.graph.MultiLocaleString"
            },
            "logoV2": "String",
            "website": {
              "@odata.type": "microsoft.graph.MultiLocaleUrl",
              "localized": [
                {
                  "@odata.type": "microsoft.graph.UrlMapElement"
                }
              ]
            },
            "locations": [
              {
                "@odata.type": "microsoft.graph.LIOrganizationLocationInfo",
                "address": {
                  "@odata.type": "microsoft.graph.Address",
                  "line1": "String",
                  "line2": "String",
                  "line3": "String",
                  "line4": "String",
                  "city": "String",
                  "geographicAreaType": "String",
                  "geographicArea": "String",
                  "postalCode": "String"
                },
                "locationType": "String",
                "standardizedLocation": {
                  "@odata.type": "microsoft.graph.LILocation"
                }
              }
            ],
            "industries": [
              {
                "@odata.type": "microsoft.graph.LIIndustry"
              }
            ]
          },
          "locationName": {
            "@odata.type": "microsoft.graph.MultiLocaleString"
          }
        }
      ],
      "educations": [
        {
          "@odata.type": "microsoft.graph.LIMemberEducation",
          "degreeName": {
            "@odata.type": "microsoft.graph.MultiLocaleString"
          },
          "activities": {
            "@odata.type": "microsoft.graph.MultiLocaleString"
          },
          "notes": {
            "@odata.type": "microsoft.graph.MultiLocaleRichText"
          },
          "school": {
            "@odata.type": "microsoft.graph.LIOrganization"
          },
          "fieldsOfStudy": [
            {
              "@odata.type": "microsoft.graph.LIMemberFieldOfStudy",
              "fieldOfStudyName": {
                "@odata.type": "microsoft.graph.MultiLocaleString"
              }
            }
          ],
          "fieldsOfStudyV2": [
            {
              "@odata.type": "microsoft.graph.LIFieldOfStudy"
            }
          ]
        }
      ],
      "certifications": [
        {
          "@odata.type": "microsoft.graph.LIMemberCertification",
          "licenseNumber": {
            "@odata.type": "microsoft.graph.MultiLocaleString"
          },
          "authority": {
            "@odata.type": "microsoft.graph.MultiLocaleString"
          },
          "url": "String"
        }
      ],
      "honors": [
        {
          "@odata.type": "microsoft.graph.LIMemberHonor",
          "issueDate": {
            "@odata.type": "microsoft.graph.Date"
          },
          "issuer": {
            "@odata.type": "microsoft.graph.MultiLocaleString"
          }
        }
      ],
      "languages": [
        {
          "@odata.type": "microsoft.graph.LIMemberLanguage",
          "proficiency": "String"
        }
      ],
      "organizations": [
        {
          "@odata.type": "microsoft.graph.LIMemberOrganization",
          "position": {
            "@odata.type": "microsoft.graph.MultiLocaleString"
          }
        }
      ],
      "patents": [
        {
          "@odata.type": "microsoft.graph.LIMemberPatent",
          "pending": true,
          "number": {
            "@odata.type": "microsoft.graph.MultiLocaleString"
          }
        }
      ],
      "projects": [
        {
          "@odata.type": "microsoft.graph.LIMemberProject"
        }
      ],
      "publications": [
        {
          "@odata.type": "microsoft.graph.LIMemberPublication",
          "date": {
            "@odata.type": "microsoft.graph.Date"
          },
          "publisher": {
            "@odata.type": "microsoft.graph.MultiLocaleString"
          }
        }
      ],
      "skills": [
        {
          "@odata.type": "microsoft.graph.LISkill"
        }
      ],
      "emails": [
        "String"
      ],
      "connectionInfo": {
        "@odata.type": "microsoft.graph.LIMemberConnectionInfo",
        "count": 1024,
        "countObfuscated": true
      },
      "location": {
        "@odata.type": "microsoft.graph.LILocation"
      }
    }
  ],
  "totalCount": 1024,
  "mutualConnectionsPage": "String"
}
```

