---
title: "List defaultManagedAppProtections"
description: "Get the defaultManagedAppProtections from the defaultManagedAppProtections navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List defaultManagedAppProtections

Namespace: microsoft.graph

Get the defaultManagedAppProtections from the defaultManagedAppProtections navigation property.

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
GET /deviceAppManagement/defaultManagedAppProtections
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
If successful, this method returns a `200 OK` response code and a collection of [defaultManagedAppProtection](../resources/defaultmanagedappprotection.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_defaultmanagedappprotection"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.defaultmanagedappprotection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4948

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
      "id": "f7ed0b16-0b16-f7ed-160b-edf7160bedf7",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
      "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "version": "Version value",
      "periodOfflineBeforeAccessCheck": "-PT51.1004519S",
      "periodOnlineBeforeAccessCheck": "PT1M59.4455281S",
      "allowedInboundDataTransferSources": "String",
      "allowedOutboundDataTransferDestinations": "String",
      "organizationalCredentialsRequired": true,
      "allowedOutboundClipboardSharingLevel": "String",
      "dataBackupBlocked": true,
      "deviceComplianceRequired": true,
      "managedBrowserToOpenLinksRequired": true,
      "saveAsBlocked": true,
      "periodOfflineBeforeWipeIsEnforced": "-PT1M14.4005247S",
      "pinRequired": true,
      "maximumPinRetries": 1,
      "simplePinBlocked": true,
      "minimumPinLength": 0,
      "pinCharacterSet": "String",
      "periodBeforePinReset": "-PT2M41.5840184S",
      "allowedDataStorageLocations": [
        "String"
      ],
      "contactSyncBlocked": true,
      "printBlocked": true,
      "fingerprintBlocked": true,
      "disableAppPinIfDevicePinIsSet": true,
      "minimumRequiredOsVersion": "Minimum Required Os Version value",
      "minimumWarningOsVersion": "Minimum Warning Os Version value",
      "minimumRequiredAppVersion": "Minimum Required App Version value",
      "minimumWarningAppVersion": "Minimum Warning App Version value",
      "minimumWipeOsVersion": "Minimum Wipe Os Version value",
      "minimumWipeAppVersion": "Minimum Wipe App Version value",
      "appActionIfDeviceComplianceRequired": "String",
      "appActionIfMaximumPinRetriesExceeded": "String",
      "pinRequiredInsteadOfBiometricTimeout": "-PT2.5164496S",
      "allowedOutboundClipboardSharingExceptionLength": 14,
      "notificationRestriction": "String",
      "previousPinBlockCount": 5,
      "managedBrowser": "String",
      "maximumAllowedDeviceThreatLevel": "String",
      "mobileThreatDefenseRemediationAction": "String",
      "blockDataIngestionIntoOrganizationDocuments": true,
      "allowedDataIngestionLocations": [
        "String"
      ],
      "appActionIfUnableToAuthenticateUser": "String",
      "appDataEncryptionType": "String",
      "screenCaptureBlocked": true,
      "encryptAppData": true,
      "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
      "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
      "customSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "deployedAppCount": 0,
      "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
      "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
      "exemptedAppProtocols": [
        {
          "@odata.type": "microsoft.graph.keyValuePair"
        }
      ],
      "exemptedAppPackages": [
        {
          "@odata.type": "microsoft.graph.keyValuePair"
        }
      ],
      "faceIdBlocked": true,
      "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
      "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
      "allowedIosDeviceModels": "Allowed Ios Device Models value",
      "appActionIfIosDeviceModelNotAllowed": "String",
      "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
      "appActionIfAndroidDeviceManufacturerNotAllowed": "String",
      "thirdPartyKeyboardsBlocked": true,
      "filterOpenInToOnlyManagedApps": true,
      "disableProtectionOfManagedOutboundOpenInData": true,
      "protectInboundDataFromUnknownSources": true,
      "requiredAndroidSafetyNetDeviceAttestationType": "String",
      "appActionIfAndroidSafetyNetDeviceAttestationFailed": "String",
      "requiredAndroidSafetyNetAppsVerificationType": "String",
      "appActionIfAndroidSafetyNetAppsVerificationFailed": "String",
      "customBrowserProtocol": "Custom Browser Protocol value",
      "customBrowserPackageId": "Custom Browser Package Id value",
      "customBrowserDisplayName": "Custom Browser Display Name value",
      "minimumRequiredCompanyPortalVersion": "Minimum Required Company Portal Version value",
      "minimumWarningCompanyPortalVersion": "Minimum Warning Company Portal Version value",
      "minimumWipeCompanyPortalVersion": "Minimum Wipe Company Portal Version value",
      "allowedAndroidDeviceModels": [
        "Allowed Android Device Models value"
      ],
      "appActionIfAndroidDeviceModelNotAllowed": "String"
    }
  ]
}
```

