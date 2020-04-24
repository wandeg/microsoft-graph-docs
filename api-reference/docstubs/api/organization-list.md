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
|Authorization|Bearer {token}. Required|

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
  "@odata.type": "collection(microsoft.graph.organization)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.organization",
      "id": "83072924-2924-8307-2429-078324290783",
      "deletedDateTime": "2017-01-01T00:02:07.4980046+03:00",
      "assignedPlans": [
        {
          "@odata.type": "microsoft.graph.assignedPlan",
          "assignedDateTime": "2016-12-31T23:56:57.6905634+03:00",
          "capabilityStatus": "Capability Status value",
          "service": "Service value",
          "servicePlanId": "ba5fb184-b184-ba5f-84b1-5fba84b15fba"
        }
      ],
      "businessPhones": [
        "Business Phones value"
      ],
      "city": "City value",
      "country": "Country value",
      "countryLetterCode": "Country Letter Code value",
      "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
      "directorySizeQuota": {
        "@odata.type": "microsoft.graph.directorySizeQuota",
        "used": 4,
        "total": 5
      },
      "displayName": "Display Name value",
      "isMultipleDataLocationsForServicesEnabled": true,
      "marketingNotificationEmails": [
        "Marketing Notification Emails value"
      ],
      "onPremisesLastSyncDateTime": "2017-01-01T00:01:17.7456992+03:00",
      "onPremisesSyncEnabled": true,
      "postalCode": "Postal Code value",
      "preferredLanguage": "Preferred Language value",
      "privacyProfile": {
        "@odata.type": "microsoft.graph.privacyProfile",
        "contactEmail": "Contact Email value",
        "statementUrl": "https://example.com/statementUrl/"
      },
      "provisionedPlans": [
        {
          "@odata.type": "microsoft.graph.provisionedPlan",
          "provisioningStatus": "Provisioning Status value"
        }
      ],
      "securityComplianceNotificationMails": [
        "Security Compliance Notification Mails value"
      ],
      "securityComplianceNotificationPhones": [
        "Security Compliance Notification Phones value"
      ],
      "state": "State value",
      "street": "Street value",
      "technicalNotificationMails": [
        "Technical Notification Mails value"
      ],
      "verifiedDomains": [
        {
          "@odata.type": "microsoft.graph.verifiedDomain",
          "capabilities": "Capabilities value",
          "isDefault": true,
          "isInitial": true,
          "name": "Name value",
          "type": "Type value"
        }
      ],
      "mobileDeviceManagementAuthority": "String",
      "certificateConnectorSetting": {
        "@odata.type": "microsoft.graph.certificateConnectorSetting",
        "status": 6,
        "certExpiryTime": "2016-12-31T23:58:43.8192312+03:00",
        "enrollmentError": "Enrollment Error value",
        "lastConnectorConnectionTime": "2016-12-31T23:57:15.4728893+03:00",
        "connectorVersion": "Connector Version value",
        "lastUploadVersion": 1
      }
    }
  ]
}
```

