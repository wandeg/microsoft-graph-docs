---
title: "List projects"
description: "Get the projectParticipations from the projects navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List projects

Namespace: microsoft.graph

Get the projectParticipations from the projects navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/projects
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [projectParticipation](../resources/projectparticipation.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_projectparticipation"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/profile/projects
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.projectparticipation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2491

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.projectParticipation",
      "id": "d1f1db93-db93-d1f1-93db-f1d193dbf1d1",
      "allowedAudiences": "String",
      "inference": {
        "@odata.type": "microsoft.graph.inferenceData",
        "confidenceScore": "Double",
        "userHasVerifiedAccuracy": true
      },
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet",
        "application": {
          "@odata.type": "microsoft.graph.identity",
          "id": "Id value",
          "displayName": "Display Name value"
        },
        "device": {
          "@odata.type": "microsoft.graph.identity"
        },
        "user": {
          "@odata.type": "microsoft.graph.identity"
        }
      },
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "categories": [
        "Categories value"
      ],
      "client": {
        "@odata.type": "microsoft.graph.companyDetail",
        "pronunciation": "Pronunciation value",
        "department": "Department value",
        "officeLocation": "Office Location value",
        "address": {
          "@odata.type": "microsoft.graph.physicalAddress",
          "type": "String",
          "postOfficeBox": "Post Office Box value",
          "street": "Street value",
          "city": "City value",
          "state": "State value",
          "countryOrRegion": "Country Or Region value",
          "postalCode": "Postal Code value"
        },
        "webUrl": "https://example.com/webUrl/"
      },
      "displayName": "Display Name value",
      "detail": {
        "@odata.type": "microsoft.graph.positionDetail",
        "company": {
          "@odata.type": "microsoft.graph.companyDetail"
        },
        "description": "Description value",
        "endMonthYear": "Date",
        "jobTitle": "Job Title value",
        "role": "Role value",
        "startMonthYear": "Date",
        "summary": "Summary value"
      },
      "colleagues": [
        {
          "@odata.type": "microsoft.graph.relatedPerson",
          "relationship": "String",
          "userPrincipalName": "User Principal Name value"
        }
      ],
      "sponsors": [
        {
          "@odata.type": "microsoft.graph.relatedPerson"
        }
      ]
    }
  ]
}
```

