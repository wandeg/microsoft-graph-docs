---
title: "LIMember resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# LIMember resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|certifications|[LIMemberCertification](../resources/limembercertification.md) collection||
|connectionInfo|[LIMemberConnectionInfo](../resources/limemberconnectioninfo.md)||
|defaultLocale|[Locale](../resources/locale.md)||
|educations|[LIMemberEducation](../resources/limembereducation.md) collection||
|emails|String collection||
|firstName|[MultiLocaleString](../resources/multilocalestring.md)||
|headline|[MultiLocaleString](../resources/multilocalestring.md)||
|honors|[LIMemberHonor](../resources/limemberhonor.md) collection||
|id|String||
|industryName|[MultiLocaleString](../resources/multilocalestring.md)||
|invitation|[LIInvite](../resources/liinvite.md)||
|languages|[LIMemberLanguage](../resources/limemberlanguage.md) collection||
|lastName|[MultiLocaleString](../resources/multilocalestring.md)||
|location|[LILocation](../resources/lilocation.md)||
|mutualConnections|[LIMutualConnections](../resources/limutualconnections.md)||
|organizations|[LIMemberOrganization](../resources/limemberorganization.md) collection||
|patents|[LIMemberPatent](../resources/limemberpatent.md) collection||
|positions|[LIMemberPosition](../resources/limemberposition.md) collection||
|profilePicture|String||
|profileUrl|String||
|projects|[LIMemberProject](../resources/limemberproject.md) collection||
|publications|[LIMemberPublication](../resources/limemberpublication.md) collection||
|skills|[LISkill](../resources/liskill.md) collection||
|summary|[MultiLocaleRichText](../resources/multilocalerichtext.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIMember"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIMember",
  "mutualConnections": {
    "@odata.type": "microsoft.graph.LIMutualConnections",
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
  },
  "invitation": {
    "@odata.type": "microsoft.graph.LIInvite",
    "viewerCanConnectViewee": true,
    "invitationSentFromViewer": true,
    "pendingInvitationSentFromViewee": {
      "@odata.type": "microsoft.graph.LIInviteDetails",
      "invitationId": "String",
      "validationToken": "String"
    }
  },
  "id": "String (identifier)",
  "firstName": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "lastName": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "headline": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "summary": {
    "@odata.type": "microsoft.graph.MultiLocaleRichText"
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
      "@odata.type": "microsoft.graph.LIMemberPosition"
    }
  ],
  "educations": [
    {
      "@odata.type": "microsoft.graph.LIMemberEducation"
    }
  ],
  "certifications": [
    {
      "@odata.type": "microsoft.graph.LIMemberCertification"
    }
  ],
  "honors": [
    {
      "@odata.type": "microsoft.graph.LIMemberHonor"
    }
  ],
  "languages": [
    {
      "@odata.type": "microsoft.graph.LIMemberLanguage"
    }
  ],
  "organizations": [
    {
      "@odata.type": "microsoft.graph.LIMemberOrganization"
    }
  ],
  "patents": [
    {
      "@odata.type": "microsoft.graph.LIMemberPatent"
    }
  ],
  "projects": [
    {
      "@odata.type": "microsoft.graph.LIMemberProject"
    }
  ],
  "publications": [
    {
      "@odata.type": "microsoft.graph.LIMemberPublication"
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
    "@odata.type": "microsoft.graph.LIMemberConnectionInfo"
  },
  "location": {
    "@odata.type": "microsoft.graph.LILocation"
  }
}
```

