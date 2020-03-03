---
title: "List educationalActivities"
description: "Get the educationalActivities from the educationalActivities navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List educationalActivities

Namespace: microsoft.graph

Get the educationalActivities from the educationalActivities navigation property.

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
GET /me/profile/educationalActivities
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [educationalActivity](../resources/educationalactivity.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_educationalactivity"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/profile/educationalActivities
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.educationalactivity)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2015

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationalActivity",
      "id": "e4f9f389-f389-e4f9-89f3-f9e489f3f9e4",
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
      "completionMonthYear": "Date",
      "endMonthYear": "Date",
      "institution": {
        "@odata.type": "microsoft.graph.institutionData",
        "description": "Description value",
        "location": {
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
      "program": {
        "@odata.type": "microsoft.graph.educationalActivityDetail",
        "abbreviation": "Abbreviation value",
        "activities": "Activities value",
        "awards": "Awards value",
        "fieldsOfStudy": "Fields Of Study value",
        "grade": "Grade value",
        "notes": "Notes value"
      },
      "startMonthYear": "Date"
    }
  ]
}
```

