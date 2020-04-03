---
title: "Get deviceManagement"
description: "Read properties and relationships of the deviceManagement object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get deviceManagement

Namespace: microsoft.graph

Read properties and relationships of the [deviceManagement](../resources/devicemanagement.md) object.

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
GET /deviceManagement
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
If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/devicemanagement.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagement"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4960

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "9d1ddc2e-dc2e-9d1d-2edc-1d9d2edc1d9d",
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
    "intuneAccountId": "5da0cf4a-cf4a-5da0-4acf-a05d4acfa05d",
    "lastReportAggregationDateTime": "2016-12-31T23:57:39.3435134+00:00",
    "deviceComplianceReportSummarizationDateTime": "2016-12-31T23:59:12.6903252+00:00",
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
          "lastUpdateDateTime": "2016-12-31T23:58:44.7733763+00:00"
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
    "accountMoveCompletionDateTime": "2017-01-01T00:02:37.7345639+00:00"
  }
}
```

