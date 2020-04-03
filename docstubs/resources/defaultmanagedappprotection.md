---
title: "defaultManagedAppProtection resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# defaultManagedAppProtection resource type


Namespace: microsoft.graph




Inherits from [managedAppProtection](../resources/managedappprotection.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get defaultManagedAppProtection](../api/defaultmanagedappprotection-get.md)|[defaultManagedAppProtection](../resources/defaultmanagedappprotection.md)|Read properties and relationships of the [defaultManagedAppProtection](../resources/defaultmanagedappprotection.md) object.|
|[Update defaultManagedAppProtection](../api/defaultmanagedappprotection-update.md)|[defaultManagedAppProtection](../resources/defaultmanagedappprotection.md)|Update the properties of a [defaultManagedAppProtection](../resources/defaultmanagedappprotection.md) object.|
|[targetApps](../api/defaultmanagedappprotection-targetapps.md)|None||
|[List apps](../api/defaultmanagedappprotection-list-apps.md)|[managedMobileApp](../resources/managedmobileapp.md) collection|Get the managedMobileApps from the apps navigation property.|
|[Add apps](../api/defaultmanagedappprotection-post-apps.md)|[managedMobileApp](../resources/managedmobileapp.md)|Add apps by posting to the apps collection.|
|[Get managedAppPolicyDeploymentSummary](../api/managedapppolicydeploymentsummary-get.md)|[managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md)|Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedAndroidDeviceManufacturers|String||
|allowedAndroidDeviceModels|String collection||
|allowedDataIngestionLocations|Enumeration collection| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|allowedDataStorageLocations|Enumeration collection| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|allowedInboundDataTransferSources|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allApps`, `managedApps`, `none`.|
|allowedIosDeviceModels|String||
|allowedOutboundClipboardSharingExceptionLength|Int32| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|allowedOutboundClipboardSharingLevel|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|allowedOutboundDataTransferDestinations|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allApps`, `managedApps`, `none`.|
|appActionIfAndroidDeviceManufacturerNotAllowed|Enumeration| Possible values are: `block`, `wipe`, `warn`.|
|appActionIfAndroidDeviceModelNotAllowed|Enumeration| Possible values are: `block`, `wipe`, `warn`.|
|appActionIfAndroidSafetyNetAppsVerificationFailed|Enumeration| Possible values are: `block`, `wipe`, `warn`.|
|appActionIfAndroidSafetyNetDeviceAttestationFailed|Enumeration| Possible values are: `block`, `wipe`, `warn`.|
|appActionIfDeviceComplianceRequired|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `block`, `wipe`, `warn`.|
|appActionIfIosDeviceModelNotAllowed|Enumeration| Possible values are: `block`, `wipe`, `warn`.|
|appActionIfMaximumPinRetriesExceeded|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `block`, `wipe`, `warn`.|
|appActionIfUnableToAuthenticateUser|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `block`, `wipe`, `warn`.|
|appDataEncryptionType|Enumeration| Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.|
|blockDataIngestionIntoOrganizationDocuments|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|contactSyncBlocked|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|createdDateTime|DateTimeOffset| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|customBrowserDisplayName|String||
|customBrowserPackageId|String||
|customBrowserProtocol|String||
|customSettings|[keyValuePair](../resources/keyvaluepair.md) collection||
|dataBackupBlocked|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|deployedAppCount|Int32||
|description|String| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|deviceComplianceRequired|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Boolean||
|disableAppPinIfDevicePinIsSet|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|disableProtectionOfManagedOutboundOpenInData|Boolean||
|displayName|String| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|encryptAppData|Boolean||
|exemptedAppPackages|[keyValuePair](../resources/keyvaluepair.md) collection||
|exemptedAppProtocols|[keyValuePair](../resources/keyvaluepair.md) collection||
|faceIdBlocked|Boolean||
|filterOpenInToOnlyManagedApps|Boolean||
|fingerprintBlocked|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|managedBrowser|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `notConfigured`, `microsoftEdge`.|
|managedBrowserToOpenLinksRequired|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|maximumAllowedDeviceThreatLevel|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `notConfigured`, `secured`, `low`, `medium`, `high`.|
|maximumPinRetries|Int32| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumPinLength|Int32| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumRequiredAppVersion|String| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumRequiredCompanyPortalVersion|String||
|minimumRequiredOsVersion|String| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumRequiredPatchVersion|String||
|minimumRequiredSdkVersion|String||
|minimumWarningAppVersion|String| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumWarningCompanyPortalVersion|String||
|minimumWarningOsVersion|String| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumWarningPatchVersion|String||
|minimumWipeAppVersion|String| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumWipeCompanyPortalVersion|String||
|minimumWipeOsVersion|String| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumWipePatchVersion|String||
|minimumWipeSdkVersion|String||
|mobileThreatDefenseRemediationAction|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `block`, `wipe`, `warn`.|
|notificationRestriction|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allow`, `blockOrganizationalData`, `block`.|
|organizationalCredentialsRequired|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|periodBeforePinReset|Duration| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|periodOfflineBeforeAccessCheck|Duration| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|periodOfflineBeforeWipeIsEnforced|Duration| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|periodOnlineBeforeAccessCheck|Duration| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|pinCharacterSet|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `numeric`, `alphanumericAndSymbol`.|
|pinRequired|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|pinRequiredInsteadOfBiometricTimeout|Duration| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|previousPinBlockCount|Int32| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|printBlocked|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|protectInboundDataFromUnknownSources|Boolean||
|requiredAndroidSafetyNetAppsVerificationType|Enumeration| Possible values are: `none`, `enabled`.|
|requiredAndroidSafetyNetDeviceAttestationType|Enumeration| Possible values are: `none`, `basicIntegrity`, `basicIntegrityAndDeviceCertification`.|
|roleScopeTagIds|String collection| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|saveAsBlocked|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|screenCaptureBlocked|Boolean||
|simplePinBlocked|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|thirdPartyKeyboardsBlocked|Boolean||
|version|String| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|apps|[managedMobileApp](../resources/managedmobileapp.md) collection||
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultManagedAppProtection",
  "baseType": "microsoft.graph.managedAppProtection",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "version": "String",
  "periodOfflineBeforeAccessCheck": "String (duration)",
  "periodOnlineBeforeAccessCheck": "String (duration)",
  "allowedInboundDataTransferSources": "String",
  "allowedOutboundDataTransferDestinations": "String",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "String",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "String (duration)",
  "pinRequired": true,
  "maximumPinRetries": 1024,
  "simplePinBlocked": true,
  "minimumPinLength": 1024,
  "pinCharacterSet": "String",
  "periodBeforePinReset": "String (duration)",
  "allowedDataStorageLocations": [
    "String"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "String",
  "minimumWarningOsVersion": "String",
  "minimumRequiredAppVersion": "String",
  "minimumWarningAppVersion": "String",
  "minimumWipeOsVersion": "String",
  "minimumWipeAppVersion": "String",
  "appActionIfDeviceComplianceRequired": "String",
  "appActionIfMaximumPinRetriesExceeded": "String",
  "pinRequiredInsteadOfBiometricTimeout": "String (duration)",
  "allowedOutboundClipboardSharingExceptionLength": 1024,
  "notificationRestriction": "String",
  "previousPinBlockCount": 1024,
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
  "minimumRequiredSdkVersion": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "deployedAppCount": 1024,
  "minimumRequiredPatchVersion": "String",
  "minimumWarningPatchVersion": "String",
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
  "minimumWipeSdkVersion": "String",
  "minimumWipePatchVersion": "String",
  "allowedIosDeviceModels": "String",
  "appActionIfIosDeviceModelNotAllowed": "String",
  "allowedAndroidDeviceManufacturers": "String",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "String",
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true,
  "requiredAndroidSafetyNetDeviceAttestationType": "String",
  "appActionIfAndroidSafetyNetDeviceAttestationFailed": "String",
  "requiredAndroidSafetyNetAppsVerificationType": "String",
  "appActionIfAndroidSafetyNetAppsVerificationFailed": "String",
  "customBrowserProtocol": "String",
  "customBrowserPackageId": "String",
  "customBrowserDisplayName": "String",
  "minimumRequiredCompanyPortalVersion": "String",
  "minimumWarningCompanyPortalVersion": "String",
  "minimumWipeCompanyPortalVersion": "String",
  "allowedAndroidDeviceModels": [
    "String"
  ],
  "appActionIfAndroidDeviceModelNotAllowed": "String"
}
```

