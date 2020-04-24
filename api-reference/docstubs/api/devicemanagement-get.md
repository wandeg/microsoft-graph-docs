---
title: "Get deviceManagement"
description: "Read the properties and relationships of a deviceManagement object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get deviceManagement

Namespace: microsoft.graph

Read the properties and relationships of a [deviceManagement](../resources/devicemanagement.md) object.

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
GET /deviceManagement
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
If successful, this method returns a `200 OK` response code and a [deviceManagement](../resources/devicemanagement.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_devicemanagement"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
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
}
```

