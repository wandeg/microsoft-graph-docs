---
title: "Update Result"
description: "Update the properties of a Result object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update Result

Namespace: microsoft.graph

Update the properties of a [Result](../resources/result.md) object.

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
PATCH /graph/{graphId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [Result](../resources/result.md) object.

The following table shows the properties that are required when you create the [Result](../resources/result.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|entities|[ResultEntities](../resources/resultentities.md)||
|aggregations|[LIAggregations](../resources/liaggregations.md) collection||
|metadata|[Metadata](../resources/metadata.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [Result](../resources/result.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_result"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/graph/{graphId}
Content-type: application/json
Content-length: 11820

{
  "@odata.type": "#microsoft.graph.Result",
  "entities": {
    "@odata.type": "microsoft.graph.ResultEntities",
    "lIFieldOfStudyArray": {
      "@odata.type": "microsoft.graph.LIFieldOfStudyArray",
      "fieldsOfStudy": [
        {
          "@odata.type": "microsoft.graph.LIFieldOfStudy",
          "id": "Id value",
          "name": {
            "@odata.type": "microsoft.graph.MultiLocaleString",
            "localized": [
              {
                "@odata.type": "microsoft.graph.StringMapElement",
                "key": "Key value",
                "value": "Value value"
              }
            ],
            "preferredLocale": {
              "@odata.type": "microsoft.graph.Locale",
              "language": "Language value",
              "country": "Country value",
              "variant": "Variant value"
            }
          }
        }
      ]
    },
    "lILocationArray": {
      "@odata.type": "microsoft.graph.LILocationArray",
      "locations": [
        {
          "@odata.type": "microsoft.graph.LILocation",
          "name": "Name value"
        }
      ]
    },
    "lIMemberArray": {
      "@odata.type": "microsoft.graph.LIMemberArray",
      "members": [
        {
          "@odata.type": "microsoft.graph.LIMember",
          "mutualConnections": {
            "@odata.type": "microsoft.graph.LIMutualConnections",
            "mutualConnections": [
              {
                "@odata.type": "microsoft.graph.LIMemberDetails",
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
                  "@odata.type": "microsoft.graph.MultiLocaleRichText",
                  "localized": [
                    {
                      "@odata.type": "microsoft.graph.RichTextMapElement",
                      "value": {
                        "@odata.type": "microsoft.graph.RichText",
                        "rawText": "Raw Text value",
                        "rtData": [
                          {
                            "@odata.type": "microsoft.graph.RTData",
                            "type": "Type value",
                            "startIdx": 8,
                            "endIdx": 6,
                            "attribute": [
                              {
                                "@odata.type": "microsoft.graph.RTAttribute"
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
                "profilePicture": "Profile Picture value",
                "defaultLocale": {
                  "@odata.type": "microsoft.graph.Locale"
                },
                "profileUrl": "https://example.com/profileUrl/",
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
                      "day": 3,
                      "month": 5,
                      "year": 4
                    },
                    "endMonthYear": {
                      "@odata.type": "microsoft.graph.Date"
                    },
                    "company": {
                      "@odata.type": "microsoft.graph.LIOrganization",
                      "logoV2": "Logo V2 value",
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
                            "line1": "Line1 value",
                            "line2": "Line2 value",
                            "line3": "Line3 value",
                            "line4": "Line4 value",
                            "city": "City value",
                            "geographicAreaType": "String",
                            "geographicArea": "Geographic Area value",
                            "postalCode": "Postal Code value"
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
                    "url": "Url value"
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
                  "Emails value"
                ],
                "connectionInfo": {
                  "@odata.type": "microsoft.graph.LIMemberConnectionInfo",
                  "count": 5,
                  "countObfuscated": true
                },
                "location": {
                  "@odata.type": "microsoft.graph.LILocation"
                }
              }
            ],
            "totalCount": 10,
            "mutualConnectionsPage": "Mutual Connections Page value"
          },
          "invitation": {
            "@odata.type": "microsoft.graph.LIInvite",
            "viewerCanConnectViewee": true,
            "invitationSentFromViewer": true,
            "pendingInvitationSentFromViewee": {
              "@odata.type": "microsoft.graph.LIInviteDetails",
              "invitationId": "Invitation Id value",
              "validationToken": "Validation Token value"
            }
          }
        }
      ]
    },
    "lIOrganizationArray": {
      "@odata.type": "microsoft.graph.LIOrganizationArray",
      "organizations": [
        {
          "@odata.type": "microsoft.graph.LIOrganization"
        }
      ]
    },
    "lISkillArray": {
      "@odata.type": "microsoft.graph.LISkillArray"
    },
    "lITitleArray": {
      "@odata.type": "microsoft.graph.LITitleArray",
      "titles": [
        {
          "@odata.type": "microsoft.graph.LITitle"
        }
      ]
    }
  },
  "aggregations": [
    {
      "@odata.type": "microsoft.graph.LIAggregations",
      "aggregationField": "Aggregation Field value",
      "buckets": [
        {
          "@odata.type": "microsoft.graph.LIAggregationBucket",
          "term": "Term value"
        }
      ]
    }
  ],
  "metadata": {
    "@odata.type": "microsoft.graph.Metadata",
    "total": 5,
    "searchMatches": [
      {
        "@odata.type": "microsoft.graph.SearchMatch",
        "matchInfo": [
          {
            "@odata.type": "microsoft.graph.LIQueryTermMatchInfo",
            "fieldName": "Field Name value"
          }
        ]
      }
    ]
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 11869

{
  "@odata.type": "#microsoft.graph.Result",
  "id": "357bf094-f094-357b-94f0-7b3594f07b35",
  "entities": {
    "@odata.type": "microsoft.graph.ResultEntities",
    "lIFieldOfStudyArray": {
      "@odata.type": "microsoft.graph.LIFieldOfStudyArray",
      "fieldsOfStudy": [
        {
          "@odata.type": "microsoft.graph.LIFieldOfStudy",
          "id": "Id value",
          "name": {
            "@odata.type": "microsoft.graph.MultiLocaleString",
            "localized": [
              {
                "@odata.type": "microsoft.graph.StringMapElement",
                "key": "Key value",
                "value": "Value value"
              }
            ],
            "preferredLocale": {
              "@odata.type": "microsoft.graph.Locale",
              "language": "Language value",
              "country": "Country value",
              "variant": "Variant value"
            }
          }
        }
      ]
    },
    "lILocationArray": {
      "@odata.type": "microsoft.graph.LILocationArray",
      "locations": [
        {
          "@odata.type": "microsoft.graph.LILocation",
          "name": "Name value"
        }
      ]
    },
    "lIMemberArray": {
      "@odata.type": "microsoft.graph.LIMemberArray",
      "members": [
        {
          "@odata.type": "microsoft.graph.LIMember",
          "mutualConnections": {
            "@odata.type": "microsoft.graph.LIMutualConnections",
            "mutualConnections": [
              {
                "@odata.type": "microsoft.graph.LIMemberDetails",
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
                  "@odata.type": "microsoft.graph.MultiLocaleRichText",
                  "localized": [
                    {
                      "@odata.type": "microsoft.graph.RichTextMapElement",
                      "value": {
                        "@odata.type": "microsoft.graph.RichText",
                        "rawText": "Raw Text value",
                        "rtData": [
                          {
                            "@odata.type": "microsoft.graph.RTData",
                            "type": "Type value",
                            "startIdx": 8,
                            "endIdx": 6,
                            "attribute": [
                              {
                                "@odata.type": "microsoft.graph.RTAttribute"
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
                "profilePicture": "Profile Picture value",
                "defaultLocale": {
                  "@odata.type": "microsoft.graph.Locale"
                },
                "profileUrl": "https://example.com/profileUrl/",
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
                      "day": 3,
                      "month": 5,
                      "year": 4
                    },
                    "endMonthYear": {
                      "@odata.type": "microsoft.graph.Date"
                    },
                    "company": {
                      "@odata.type": "microsoft.graph.LIOrganization",
                      "logoV2": "Logo V2 value",
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
                            "line1": "Line1 value",
                            "line2": "Line2 value",
                            "line3": "Line3 value",
                            "line4": "Line4 value",
                            "city": "City value",
                            "geographicAreaType": "String",
                            "geographicArea": "Geographic Area value",
                            "postalCode": "Postal Code value"
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
                    "url": "Url value"
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
                  "Emails value"
                ],
                "connectionInfo": {
                  "@odata.type": "microsoft.graph.LIMemberConnectionInfo",
                  "count": 5,
                  "countObfuscated": true
                },
                "location": {
                  "@odata.type": "microsoft.graph.LILocation"
                }
              }
            ],
            "totalCount": 10,
            "mutualConnectionsPage": "Mutual Connections Page value"
          },
          "invitation": {
            "@odata.type": "microsoft.graph.LIInvite",
            "viewerCanConnectViewee": true,
            "invitationSentFromViewer": true,
            "pendingInvitationSentFromViewee": {
              "@odata.type": "microsoft.graph.LIInviteDetails",
              "invitationId": "Invitation Id value",
              "validationToken": "Validation Token value"
            }
          }
        }
      ]
    },
    "lIOrganizationArray": {
      "@odata.type": "microsoft.graph.LIOrganizationArray",
      "organizations": [
        {
          "@odata.type": "microsoft.graph.LIOrganization"
        }
      ]
    },
    "lISkillArray": {
      "@odata.type": "microsoft.graph.LISkillArray"
    },
    "lITitleArray": {
      "@odata.type": "microsoft.graph.LITitleArray",
      "titles": [
        {
          "@odata.type": "microsoft.graph.LITitle"
        }
      ]
    }
  },
  "aggregations": [
    {
      "@odata.type": "microsoft.graph.LIAggregations",
      "aggregationField": "Aggregation Field value",
      "buckets": [
        {
          "@odata.type": "microsoft.graph.LIAggregationBucket",
          "term": "Term value"
        }
      ]
    }
  ],
  "metadata": {
    "@odata.type": "microsoft.graph.Metadata",
    "total": 5,
    "searchMatches": [
      {
        "@odata.type": "microsoft.graph.SearchMatch",
        "matchInfo": [
          {
            "@odata.type": "microsoft.graph.LIQueryTermMatchInfo",
            "fieldName": "Field Name value"
          }
        ]
      }
    ]
  }
}
```

