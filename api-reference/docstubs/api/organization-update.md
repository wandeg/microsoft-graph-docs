---
title: "Update organization"
description: "Update the properties of an organization object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update organization

Namespace: microsoft.graph

Update the properties of an [organization](../resources/organization.md) object.

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
PATCH /organization/{organizationId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [organization](../resources/organization.md) object.

The following table shows the properties that are required when you create the [organization](../resources/organization.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|assignedPlans|[assignedPlan](../resources/assignedplan.md) collection|**TODO: Add Description**|
|businessPhones|String collection|**TODO: Add Description**|
|city|String|**TODO: Add Description**|
|country|String|**TODO: Add Description**|
|countryLetterCode|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|directorySizeQuota|[directorySizeQuota](../resources/directorysizequota.md)|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|isMultipleDataLocationsForServicesEnabled|Boolean|**TODO: Add Description**|
|marketingNotificationEmails|String collection|**TODO: Add Description**|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|onPremisesSyncEnabled|Boolean|**TODO: Add Description**|
|postalCode|String|**TODO: Add Description**|
|preferredLanguage|String|**TODO: Add Description**|
|privacyProfile|[privacyProfile](../resources/privacyprofile.md)|**TODO: Add Description**|
|provisionedPlans|[provisionedPlan](../resources/provisionedplan.md) collection|**TODO: Add Description**|
|securityComplianceNotificationMails|String collection|**TODO: Add Description**|
|securityComplianceNotificationPhones|String collection|**TODO: Add Description**|
|state|String|**TODO: Add Description**|
|street|String|**TODO: Add Description**|
|technicalNotificationMails|String collection|**TODO: Add Description**|
|verifiedDomains|[verifiedDomain](../resources/verifieddomain.md) collection|**TODO: Add Description**|
|mobileDeviceManagementAuthority|mdmAuthority|Mobile device management authority. Possible values are: `unknown`, `intune`, `sccm`, `office365`.|
|certificateConnectorSetting|[certificateConnectorSetting](../resources/certificateconnectorsetting.md)|Certificate connector setting.|



## Response
If successful, this method returns a `200 OK` response code and an updated [organization](../resources/organization.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_organization"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}
Content-Type: application/json
Content-length: 2468

{
  "@odata.type": "#microsoft.graph.organization",
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
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
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
```

