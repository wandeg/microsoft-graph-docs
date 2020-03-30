---
title: "Get organization"
description: "Read properties and relationships of the organization object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get organization

Namespace: microsoft.graph

Read properties and relationships of the [organization](../resources/organization.md) object.

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
GET /organization/{organizationId}
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
If successful, this method returns a `200 OK` response code and [organization](../resources/organization.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_organization"
}
-->
``` http
GET https://graph.microsoft.com/beta/organization/{organizationId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2745

{
  "value": {
    "@odata.type": "#microsoft.graph.organization",
    "id": "0812590e-590e-0812-0e59-12080e591208",
    "deletedDateTime": "2016-12-31T23:57:00.1067265+03:00",
    "assignedPlans": [
      {
        "@odata.type": "microsoft.graph.assignedPlan",
        "assignedDateTime": "2017-01-01T00:03:00.2256577+03:00",
        "capabilityStatus": "Capability Status value",
        "service": "Service value",
        "servicePlanId": "c7e63634-3634-c7e6-3436-e6c73436e6c7"
      }
    ],
    "businessPhones": [
      "Business Phones value"
    ],
    "city": "City value",
    "country": "Country value",
    "countryLetterCode": "Country Letter Code value",
    "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
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
    "onPremisesLastSyncDateTime": "2016-12-31T23:59:58.9687424+03:00",
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
      "certExpiryTime": "2016-12-31T23:57:38.1999154+03:00",
      "enrollmentError": "Enrollment Error value",
      "lastConnectorConnectionTime": "2017-01-01T00:01:49.5804926+03:00",
      "connectorVersion": "Connector Version value",
      "lastUploadVersion": 1
    }
  }
}
```

