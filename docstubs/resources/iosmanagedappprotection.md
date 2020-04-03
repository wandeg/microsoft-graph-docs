---
title: "iosManagedAppProtection resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosManagedAppProtection resource type


Namespace: microsoft.graph




Inherits from [targetedManagedAppProtection](../resources/targetedmanagedappprotection.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get iosManagedAppProtection](../api/iosmanagedappprotection-get.md)|[iosManagedAppProtection](../resources/iosmanagedappprotection.md)|Read properties and relationships of the [iosManagedAppProtection](../resources/iosmanagedappprotection.md) object.|
|[Update iosManagedAppProtection](../api/iosmanagedappprotection-update.md)|[iosManagedAppProtection](../resources/iosmanagedappprotection.md)|Update the properties of a [iosManagedAppProtection](../resources/iosmanagedappprotection.md) object.|
|[hasPayloadLinks](../api/iosmanagedappprotection-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/haspayloadlinkresultitem.md) collection||
|[assign](../api/iosmanagedappprotection-assign.md)|None||
|[List assignments](../api/iosmanagedappprotection-list-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) collection|Get the targetedManagedAppPolicyAssignments from the assignments navigation property.|
|[Add assignments](../api/iosmanagedappprotection-post-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md)|Add assignments by posting to the assignments collection.|
|[List apps](../api/iosmanagedappprotection-list-apps.md)|[managedMobileApp](../resources/managedmobileapp.md) collection|Get the managedMobileApps from the apps navigation property.|
|[Add apps](../api/iosmanagedappprotection-post-apps.md)|[managedMobileApp](../resources/managedmobileapp.md)|Add apps by posting to the apps collection.|
|[Get managedAppPolicyDeploymentSummary](../api/managedapppolicydeploymentsummary-get.md)|[managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md)|Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedDataIngestionLocations|Enumeration collection| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|allowedDataStorageLocations|Enumeration collection| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|allowedInboundDataTransferSources|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allApps`, `managedApps`, `none`.|
|allowedIosDeviceModels|String||
|allowedOutboundClipboardSharingExceptionLength|Int32| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|allowedOutboundClipboardSharingLevel|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|allowedOutboundDataTransferDestinations|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allApps`, `managedApps`, `none`.|
|appActionIfDeviceComplianceRequired|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `block`, `wipe`, `warn`.|
|appActionIfIosDeviceModelNotAllowed|Enumeration| Possible values are: `block`, `wipe`, `warn`.|
|appActionIfMaximumPinRetriesExceeded|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `block`, `wipe`, `warn`.|
|appActionIfUnableToAuthenticateUser|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `block`, `wipe`, `warn`.|
|appDataEncryptionType|Enumeration| Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.|
|blockDataIngestionIntoOrganizationDocuments|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|contactSyncBlocked|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|createdDateTime|DateTimeOffset| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|customBrowserProtocol|String||
|dataBackupBlocked|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|deployedAppCount|Int32||
|description|String| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|deviceComplianceRequired|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|disableAppPinIfDevicePinIsSet|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|disableProtectionOfManagedOutboundOpenInData|Boolean||
|displayName|String| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|exemptedAppProtocols|[keyValuePair](../resources/keyvaluepair.md) collection||
|faceIdBlocked|Boolean||
|filterOpenInToOnlyManagedApps|Boolean||
|fingerprintBlocked|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isAssigned|Boolean| Inherited from [targetedManagedAppProtection](../resources/targetedmanagedappprotection.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|managedBrowser|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `notConfigured`, `microsoftEdge`.|
|managedBrowserToOpenLinksRequired|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|maximumAllowedDeviceThreatLevel|Enumeration| Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `notConfigured`, `secured`, `low`, `medium`, `high`.|
|maximumPinRetries|Int32| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumPinLength|Int32| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumRequiredAppVersion|String| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumRequiredOsVersion|String| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumRequiredSdkVersion|String||
|minimumWarningAppVersion|String| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumWarningOsVersion|String| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumWipeAppVersion|String| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumWipeOsVersion|String| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
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
|roleScopeTagIds|String collection| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|saveAsBlocked|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|simplePinBlocked|Boolean| Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|targetedAppManagementLevels|Enumeration| Inherited from [targetedManagedAppProtection](../resources/targetedmanagedappprotection.md). Possible values are: `unspecified`, `unmanaged`, `mdm`, `androidEnterprise`.|
|thirdPartyKeyboardsBlocked|Boolean||
|version|String| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|apps|[managedMobileApp](../resources/managedmobileapp.md) collection||
|assignments|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) collection| Inherited from [targetedManagedAppProtection](../resources/targetedmanagedappprotection.md)|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosManagedAppProtection",
  "baseType": "microsoft.graph.targetedManagedAppProtection",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosManagedAppProtection",
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
  "isAssigned": true,
  "targetedAppManagementLevels": "String",
  "appDataEncryptionType": "String",
  "minimumRequiredSdkVersion": "String",
  "deployedAppCount": 1024,
  "faceIdBlocked": true,
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "minimumWipeSdkVersion": "String",
  "allowedIosDeviceModels": "String",
  "appActionIfIosDeviceModelNotAllowed": "String",
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true,
  "customBrowserProtocol": "String"
}
```

