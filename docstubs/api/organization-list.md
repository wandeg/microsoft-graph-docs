---
title: "List organizations"
description: "List properties and relationships of the organization objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List organizations

Namespace: microsoft.graph

List properties and relationships of the [organization](../resources/organization.md) objects.

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
GET /organization
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.organization)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2909

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.organization",
      "id": "3e47a32c-a32c-3e47-2ca3-473e2ca3473e",
      "deletedDateTime": "2017-01-01T00:01:42.7296606+00:00",
      "assignedPlans": [
        {
          "@odata.type": "microsoft.graph.assignedPlan",
          "assignedDateTime": "2017-01-01T00:02:08.3128832+00:00",
          "capabilityStatus": "Capability Status value",
          "service": "Service value",
          "servicePlanId": "439cd6b6-d6b6-439c-b6d6-9c43b6d69c43"
        }
      ],
      "businessPhones": [
        "Business Phones value"
      ],
      "city": "City value",
      "country": "Country value",
      "countryLetterCode": "Country Letter Code value",
      "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
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
      "onPremisesLastSyncDateTime": "2017-01-01T00:02:42.7451887+00:00",
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
        "certExpiryTime": "2016-12-31T23:56:57.8873098+00:00",
        "enrollmentError": "Enrollment Error value",
        "lastConnectorConnectionTime": "2016-12-31T23:56:47.2374224+00:00",
        "connectorVersion": "Connector Version value",
        "lastUploadVersion": 1
      }
    }
  ]
}
```

