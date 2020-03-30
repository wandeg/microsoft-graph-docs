---
title: "Get workPosition"
description: "Read properties and relationships of the workPosition object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get workPosition

Namespace: microsoft.graph

Read properties and relationships of the [workPosition](../resources/workposition.md) object.

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
GET /me/profile/positions/{workPositionId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [workPosition](../resources/workposition.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workposition"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/positions/{workPositionId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workPosition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1935

{
  "value": {
    "@odata.type": "#microsoft.graph.workPosition",
    "id": "89cc717b-717b-89cc-7b71-cc897b71cc89",
    "allowedAudiences": "String",
    "inference": {
      "@odata.type": "microsoft.graph.inferenceData",
      "confidenceScore": "Double",
      "userHasVerifiedAccuracy": true
    },
    "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
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
    "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
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
}
```

