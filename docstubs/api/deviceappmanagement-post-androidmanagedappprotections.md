---
title: "Add androidManagedAppProtections"
description: "Add androidManagedAppProtections by posting to the androidManagedAppProtections collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add androidManagedAppProtections

Namespace: microsoft.graph

Add androidManagedAppProtections by posting to the androidManagedAppProtections collection.

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
POST /deviceAppManagement/androidManagedAppProtections/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [androidManagedAppProtection](../resources/androidmanagedappprotection.md) object.

The following table shows the properties that are required when you create the [androidManagedAppProtection](../resources/androidmanagedappprotection.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|description|String| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|createdDateTime|DateTimeOffset| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|roleScopeTagIds|String collection| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|version|String| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|periodOfflineBeforeAccessCheck|Duration| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|periodOnlineBeforeAccessCheck|Duration| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|allowedInboundDataTransferSources|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|allowedOutboundClipboardSharingLevel|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|deviceComplianceRequired|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|managedBrowserToOpenLinksRequired|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|saveAsBlocked|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|periodOfflineBeforeWipeIsEnforced|Duration| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|pinRequired|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|maximumPinRetries|Int32| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|simplePinBlocked|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumPinLength|Int32| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|pinCharacterSet|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Duration| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|allowedDataStorageLocations|Enumeration collection| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.|
|contactSyncBlocked|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|printBlocked|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|fingerprintBlocked|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|disableAppPinIfDevicePinIsSet|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumRequiredOsVersion|String| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumWarningOsVersion|String| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumRequiredAppVersion|String| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumWarningAppVersion|String| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumWipeOsVersion|String| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumWipeAppVersion|String| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|appActionIfDeviceComplianceRequired|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `block`, `wipe`, `warn`.|
|appActionIfMaximumPinRetriesExceeded|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `block`, `wipe`, `warn`.|
|pinRequiredInsteadOfBiometricTimeout|Duration| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|allowedOutboundClipboardSharingExceptionLength|Int32| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|notificationRestriction|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allow`, `blockOrganizationalData`, `block`.|
|previousPinBlockCount|Int32| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|managedBrowser|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `notConfigured`, `microsoftEdge`.|
|maximumAllowedDeviceThreatLevel|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `notConfigured`, `secured`, `low`, `medium`, `high`.|
|mobileThreatDefenseRemediationAction|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `block`, `wipe`, `warn`.|
|blockDataIngestionIntoOrganizationDocuments|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|allowedDataIngestionLocations|Enumeration collection| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `oneDriveForBusiness`, `sharePoint`, `camera`.|
|appActionIfUnableToAuthenticateUser|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `block`, `wipe`, `warn`.|
|isAssigned|Boolean| Inherited from [targetedManagedAppProtection](../resources/targetedmanagedappprotection.md)|
|targetedAppManagementLevels|Enumeration| Inherited from [targetedManagedAppProtection](../resources/targetedmanagedappprotection.md). Possible values are: `unspecified`, `unmanaged`, `mdm`, `androidEnterprise`.|
|screenCaptureBlocked|Boolean||
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Boolean||
|encryptAppData|Boolean||
|deployedAppCount|Int32||
|minimumRequiredPatchVersion|String||
|minimumWarningPatchVersion|String||
|exemptedAppPackages|[keyValuePair](../resources/keyvaluepair.md) collection||
|minimumWipePatchVersion|String||
|allowedAndroidDeviceManufacturers|String||
|appActionIfAndroidDeviceManufacturerNotAllowed|Enumeration| Possible values are: `block`, `wipe`, `warn`.|
|requiredAndroidSafetyNetDeviceAttestationType|Enumeration| Possible values are: `none`, `basicIntegrity`, `basicIntegrityAndDeviceCertification`.|
|appActionIfAndroidSafetyNetDeviceAttestationFailed|Enumeration| Possible values are: `block`, `wipe`, `warn`.|
|requiredAndroidSafetyNetAppsVerificationType|Enumeration| Possible values are: `none`, `enabled`.|
|appActionIfAndroidSafetyNetAppsVerificationFailed|Enumeration| Possible values are: `block`, `wipe`, `warn`.|
|customBrowserPackageId|String||
|customBrowserDisplayName|String||
|minimumRequiredCompanyPortalVersion|String||
|minimumWarningCompanyPortalVersion|String||
|minimumWipeCompanyPortalVersion|String||
|keyboardsRestricted|Boolean||
|approvedKeyboards|[keyValuePair](../resources/keyvaluepair.md) collection||
|allowedAndroidDeviceModels|String collection||
|appActionIfAndroidDeviceModelNotAllowed|Enumeration| Possible values are: `block`, `wipe`, `warn`.|



## Response
If successful, this method returns a `201 Created` response code and a [androidManagedAppProtection](../resources/androidmanagedappprotection.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_androidmanagedappprotection_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections
Content-type: application/json
Content-length: 3767

{
  "@odata.type": "#microsoft.graph.androidManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
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
  "isAssigned": true,
  "targetedAppManagementLevels": "String",
  "screenCaptureBlocked": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "encryptAppData": true,
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
  "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "String",
  "requiredAndroidSafetyNetDeviceAttestationType": "String",
  "appActionIfAndroidSafetyNetDeviceAttestationFailed": "String",
  "requiredAndroidSafetyNetAppsVerificationType": "String",
  "appActionIfAndroidSafetyNetAppsVerificationFailed": "String",
  "customBrowserPackageId": "Custom Browser Package Id value",
  "customBrowserDisplayName": "Custom Browser Display Name value",
  "minimumRequiredCompanyPortalVersion": "Minimum Required Company Portal Version value",
  "minimumWarningCompanyPortalVersion": "Minimum Warning Company Portal Version value",
  "minimumWipeCompanyPortalVersion": "Minimum Wipe Company Portal Version value",
  "keyboardsRestricted": true,
  "approvedKeyboards": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "allowedAndroidDeviceModels": [
    "Allowed Android Device Models value"
  ],
  "appActionIfAndroidDeviceModelNotAllowed": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.androidmanagedappprotection"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3939

{
  "@odata.type": "#microsoft.graph.androidManagedAppProtection",
  "id": "b99312fa-12fa-b993-fa12-93b9fa1293b9",
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
  "isAssigned": true,
  "targetedAppManagementLevels": "String",
  "screenCaptureBlocked": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "encryptAppData": true,
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
  "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "String",
  "requiredAndroidSafetyNetDeviceAttestationType": "String",
  "appActionIfAndroidSafetyNetDeviceAttestationFailed": "String",
  "requiredAndroidSafetyNetAppsVerificationType": "String",
  "appActionIfAndroidSafetyNetAppsVerificationFailed": "String",
  "customBrowserPackageId": "Custom Browser Package Id value",
  "customBrowserDisplayName": "Custom Browser Display Name value",
  "minimumRequiredCompanyPortalVersion": "Minimum Required Company Portal Version value",
  "minimumWarningCompanyPortalVersion": "Minimum Warning Company Portal Version value",
  "minimumWipeCompanyPortalVersion": "Minimum Wipe Company Portal Version value",
  "keyboardsRestricted": true,
  "approvedKeyboards": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "allowedAndroidDeviceModels": [
    "Allowed Android Device Models value"
  ],
  "appActionIfAndroidDeviceModelNotAllowed": "String"
}
```

