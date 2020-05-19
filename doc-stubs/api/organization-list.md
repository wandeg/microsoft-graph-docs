---
title: "List organizations"
description: "Get a list of the organization objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List organizations

Namespace: microsoft.graph

Get a list of the [organization](../resources/organization.md) objects and their properties.

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
GET /organization
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [organization](../resources/organization.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_organization"
}
-->
``` http
GET https://graph.microsoft.com/beta/organization
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.directoryservices.organization)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#Microsoft.DirectoryServices.organization",
      "id": "f2c1af2d-af2d-f2c1-2daf-c1f22dafc1f2",
      "deletedDateTime": "String (timestamp)",
      "assignedPlans": [
        {
          "@odata.type": "microsoft.graph.assignedPlan"
        }
      ],
      "businessPhones": [
        "String"
      ],
      "city": "String",
      "country": "String",
      "countryLetterCode": "String",
      "createdDateTime": "String (timestamp)",
      "directorySizeQuota": {
        "@odata.type": "microsoft.graph.directorySizeQuota"
      },
      "displayName": "String",
      "isMultipleDataLocationsForServicesEnabled": "Boolean",
      "marketingNotificationEmails": [
        "String"
      ],
      "onPremisesLastSyncDateTime": "String (timestamp)",
      "onPremisesSyncEnabled": "Boolean",
      "postalCode": "String",
      "preferredLanguage": "String",
      "privacyProfile": {
        "@odata.type": "microsoft.graph.privacyProfile"
      },
      "provisionedPlans": [
        {
          "@odata.type": "microsoft.graph.provisionedPlan"
        }
      ],
      "securityComplianceNotificationMails": [
        "String"
      ],
      "securityComplianceNotificationPhones": [
        "String"
      ],
      "state": "String",
      "street": "String",
      "technicalNotificationMails": [
        "String"
      ],
      "verifiedDomains": [
        {
          "@odata.type": "microsoft.graph.verifiedDomain"
        }
      ]
    }
  ]
}
```

