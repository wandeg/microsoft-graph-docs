---
title: "Update deviceManagement"
description: "Update the properties of a deviceManagement object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deviceManagement

Namespace: microsoft.graph

Update the properties of a [deviceManagement](../resources/devicemanagement.md) object.

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
PATCH /deviceManagement
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [deviceManagement](../resources/devicemanagement.md) object.

The following table shows the properties that are required when you create the [deviceManagement](../resources/devicemanagement.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|settings|[deviceManagementSettings](../resources/devicemanagementsettings.md)|Account level settings.|
|maximumDepTokens|Int32|Maximum number of dep tokens allowed per-tenant.|
|intuneAccountId|Guid|Intune Account Id for given tenant|
|lastReportAggregationDateTime|DateTimeOffset|The last modified time of reporting for this account. This property is read-only.|
|deviceComplianceReportSummarizationDateTime|DateTimeOffset|The last requested time of device compliance reporting for this account. This property is read-only.|
|legacyPcManangementEnabled|Boolean|The property to enable Non-MDM managed legacy PC management for this account. This property is read-only.|
|intuneBrand|[intuneBrand](../resources/intunebrand.md)|intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.|
|subscriptionState|deviceManagementSubscriptionState|Tenant mobile device management subscription state. Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|subscriptions|deviceManagementSubscriptions|Tenant's Subscription. Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.|
|managedDeviceCleanupSettings|[managedDeviceCleanupSettings](../resources/manageddevicecleanupsettings.md)|Device cleanup rule|
|adminConsent|[adminConsent](../resources/adminconsent.md)|Admin consent information.|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/deviceprotectionoverview.md)|Device protection overview.|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/windowsmalwareoverview.md)|Malware overview for windows devices.|
|accountMoveCompletionDateTime|DateTimeOffset|The date & time when tenant data moved between scaleunits.|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/devicemanagement.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_devicemanagement"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-Type: application/json
Content-length: 4631

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 4,
    "isScheduledActionEnabled": true,
    "secureByDefault": true,
    "enhancedJailBreak": true,
    "deviceInactivityBeforeRetirementInDay": 5,
    "derivedCredentialProvider": "String",
    "derivedCredentialUrl": "https://example.com/derivedCredentialUrl/",
    "androidDeviceAdministratorEnrollmentEnabled": true,
    "ignoreDevicesForUnsupportedSettingsEnabled": true
  },
  "maximumDepTokens": 0,
  "intuneAccountId": "c214ad1a-ad1a-c214-1aad-14c21aad14c2",
  "lastReportAggregationDateTime": "2017-01-01T00:01:49.969283+03:00",
  "deviceComplianceReportSummarizationDateTime": "2017-01-01T00:00:42.0758155+03:00",
  "legacyPcManangementEnabled": true,
  "intuneBrand": {
    "@odata.type": "microsoft.graph.intuneBrand",
    "displayName": "Display Name value",
    "themeColor": {
      "@odata.type": "microsoft.graph.rgbColor",
      "r": 1,
      "g": 1,
      "b": 1
    },
    "showLogo": true,
    "lightBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "darkBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent"
    },
    "showNameNextToLogo": true,
    "landingPageCustomizedImage": {
      "@odata.type": "microsoft.graph.mimeContent"
    },
    "showDisplayNameNextToLogo": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "contactITName": "Contact ITName value",
    "contactITPhoneNumber": "Contact ITPhone Number value",
    "contactITEmailAddress": "Contact ITEmail Address value",
    "contactITNotes": "Contact ITNotes value",
    "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
    "onlineSupportSiteName": "Online Support Site Name value",
    "privacyUrl": "https://example.com/privacyUrl/",
    "customPrivacyMessage": "Custom Privacy Message value",
    "isRemoveDeviceDisabled": true,
    "isFactoryResetDisabled": true,
    "companyPortalBlockedActions": [
      {
        "@odata.type": "microsoft.graph.companyPortalBlockedAction",
        "platform": "String",
        "ownerType": "String",
        "action": "String"
      }
    ],
    "showAzureADEnterpriseApps": true,
    "showOfficeWebApps": true,
    "sendDeviceOwnershipChangePushNotification": true,
    "enrollmentAvailability": "String"
  },
  "subscriptionState": "String",
  "subscriptions": "String",
  "managedDeviceCleanupSettings": {
    "@odata.type": "microsoft.graph.managedDeviceCleanupSettings",
    "deviceInactivityBeforeRetirementInDays": "Device Inactivity Before Retirement In Days value"
  },
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "String",
    "shareUserExperienceAnalyticsData": "String"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "windowsMalwareOverview": {
    "@odata.type": "microsoft.graph.windowsMalwareOverview",
    "malwareDetectedDeviceCount": 10,
    "malwareStateSummary": [
      {
        "@odata.type": "microsoft.graph.windowsMalwareStateCount",
        "state": "String",
        "deviceCount": 11,
        "lastUpdateDateTime": "2017-01-01T00:03:05.9143895+03:00"
      }
    ],
    "malwareExecutionStateSummary": [
      {
        "@odata.type": "microsoft.graph.windowsMalwareExecutionStateCount",
        "executionState": "String"
      }
    ],
    "malwareCategorySummary": [
      {
        "@odata.type": "microsoft.graph.windowsMalwareCategoryCount",
        "category": "String"
      }
    ],
    "malwareNameSummary": [
      {
        "@odata.type": "microsoft.graph.windowsMalwareNameCount",
        "malwareIdentifier": "Malware Identifier value",
        "name": "Name value"
      }
    ],
    "osVersionsSummary": [
      {
        "@odata.type": "microsoft.graph.osVersionCount",
        "osVersion": "Os Version value"
      }
    ]
  },
  "accountMoveCompletionDateTime": "2016-12-31T23:58:14.3370898+03:00"
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
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "6b97fc7a-fc7a-6b97-7afc-976b7afc976b",
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 4,
    "isScheduledActionEnabled": true,
    "secureByDefault": true,
    "enhancedJailBreak": true,
    "deviceInactivityBeforeRetirementInDay": 5,
    "derivedCredentialProvider": "String",
    "derivedCredentialUrl": "https://example.com/derivedCredentialUrl/",
    "androidDeviceAdministratorEnrollmentEnabled": true,
    "ignoreDevicesForUnsupportedSettingsEnabled": true
  },
  "maximumDepTokens": 0,
  "intuneAccountId": "c214ad1a-ad1a-c214-1aad-14c21aad14c2",
  "lastReportAggregationDateTime": "2017-01-01T00:01:49.969283+03:00",
  "deviceComplianceReportSummarizationDateTime": "2017-01-01T00:00:42.0758155+03:00",
  "legacyPcManangementEnabled": true,
  "intuneBrand": {
    "@odata.type": "microsoft.graph.intuneBrand",
    "displayName": "Display Name value",
    "themeColor": {
      "@odata.type": "microsoft.graph.rgbColor",
      "r": 1,
      "g": 1,
      "b": 1
    },
    "showLogo": true,
    "lightBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "darkBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent"
    },
    "showNameNextToLogo": true,
    "landingPageCustomizedImage": {
      "@odata.type": "microsoft.graph.mimeContent"
    },
    "showDisplayNameNextToLogo": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "contactITName": "Contact ITName value",
    "contactITPhoneNumber": "Contact ITPhone Number value",
    "contactITEmailAddress": "Contact ITEmail Address value",
    "contactITNotes": "Contact ITNotes value",
    "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
    "onlineSupportSiteName": "Online Support Site Name value",
    "privacyUrl": "https://example.com/privacyUrl/",
    "customPrivacyMessage": "Custom Privacy Message value",
    "isRemoveDeviceDisabled": true,
    "isFactoryResetDisabled": true,
    "companyPortalBlockedActions": [
      {
        "@odata.type": "microsoft.graph.companyPortalBlockedAction",
        "platform": "String",
        "ownerType": "String",
        "action": "String"
      }
    ],
    "showAzureADEnterpriseApps": true,
    "showOfficeWebApps": true,
    "sendDeviceOwnershipChangePushNotification": true,
    "enrollmentAvailability": "String"
  },
  "subscriptionState": "String",
  "subscriptions": "String",
  "managedDeviceCleanupSettings": {
    "@odata.type": "microsoft.graph.managedDeviceCleanupSettings",
    "deviceInactivityBeforeRetirementInDays": "Device Inactivity Before Retirement In Days value"
  },
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "String",
    "shareUserExperienceAnalyticsData": "String"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "windowsMalwareOverview": {
    "@odata.type": "microsoft.graph.windowsMalwareOverview",
    "malwareDetectedDeviceCount": 10,
    "malwareStateSummary": [
      {
        "@odata.type": "microsoft.graph.windowsMalwareStateCount",
        "state": "String",
        "deviceCount": 11,
        "lastUpdateDateTime": "2017-01-01T00:03:05.9143895+03:00"
      }
    ],
    "malwareExecutionStateSummary": [
      {
        "@odata.type": "microsoft.graph.windowsMalwareExecutionStateCount",
        "executionState": "String"
      }
    ],
    "malwareCategorySummary": [
      {
        "@odata.type": "microsoft.graph.windowsMalwareCategoryCount",
        "category": "String"
      }
    ],
    "malwareNameSummary": [
      {
        "@odata.type": "microsoft.graph.windowsMalwareNameCount",
        "malwareIdentifier": "Malware Identifier value",
        "name": "Name value"
      }
    ],
    "osVersionsSummary": [
      {
        "@odata.type": "microsoft.graph.osVersionCount",
        "osVersion": "Os Version value"
      }
    ]
  },
  "accountMoveCompletionDateTime": "2016-12-31T23:58:14.3370898+03:00"
}
```

