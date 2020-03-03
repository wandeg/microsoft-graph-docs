---
title: "List workPositions"
description: "List properties and relationships of the workPosition objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List workPositions

Namespace: microsoft.graph

List properties and relationships of the [workPosition](../resources/workposition.md) objects.

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
GET /me/profile/positions
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [workPosition](../resources/workposition.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workposition"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/profile/positions
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workposition)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2060

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workPosition",
      "id": "9b98c28c-c28c-9b98-8cc2-989b8cc2989b",
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
      "detail": {
        "@odata.type": "microsoft.graph.positionDetail",
        "company": {
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
        "description": "Description value",
        "endMonthYear": "Date",
        "jobTitle": "Job Title value",
        "role": "Role value",
        "startMonthYear": "Date",
        "summary": "Summary value"
      }
    }
  ]
}
```

