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
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_organization"
}
-->
``` http
GET https://graph.microsoft.com/beta/organization
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.organization)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2907

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.organization",
      "id": "3b5f4a86-4a86-3b5f-864a-5f3b864a5f3b",
      "deletedDateTime": "2017-01-01T00:02:56.4302403+03:00",
      "assignedPlans": [
        {
          "@odata.type": "microsoft.graph.assignedPlan",
          "assignedDateTime": "2017-01-01T00:00:15.9351772+03:00",
          "capabilityStatus": "Capability Status value",
          "service": "Service value",
          "servicePlanId": "976809b7-09b7-9768-b709-6897b7096897"
        }
      ],
      "businessPhones": [
        "Business Phones value"
      ],
      "city": "City value",
      "country": "Country value",
      "countryLetterCode": "Country Letter Code value",
      "createdDateTime": "2017-01-01T00:01:55.391884+03:00",
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
      "onPremisesLastSyncDateTime": "2016-12-31T23:59:29.9854725+03:00",
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
        "certExpiryTime": "2017-01-01T00:01:43.2836124+03:00",
        "enrollmentError": "Enrollment Error value",
        "lastConnectorConnectionTime": "2017-01-01T00:03:06.115054+03:00",
        "connectorVersion": "Connector Version value",
        "lastUploadVersion": 1
      }
    }
  ]
}
```

