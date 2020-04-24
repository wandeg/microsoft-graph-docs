---
title: "List positions"
description: "Get the workPositions from the positions navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List positions

Namespace: microsoft.graph

Get the workPositions from the positions navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /invitations/{invitationsId}/invitedUser/profile/positions
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [workPosition](../resources/workposition.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_workposition"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/profile/positions
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workposition)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workPosition",
      "id": "4a865f9a-5f9a-4a86-9a5f-864a9a5f864a",
      "allowedAudiences": "String",
      "inference": {
        "@odata.type": "microsoft.graph.inferenceData",
        "confidenceScore": "Double",
        "userHasVerifiedAccuracy": true
      },
      "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
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
      "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
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

