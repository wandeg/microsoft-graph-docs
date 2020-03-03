---
title: "managedAppProtection resource type"
description: "Policy used to configure detailed management settings for a specified set of apps"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# managedAppProtection resource type

Policy used to configure detailed management settings for a specified set of apps


Inherits from [managedAppPolicy](../resources/managedAppPolicy.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List managedAppProtections](../api/managedappprotection-list.md)|[managedAppProtection](../resources/managedAppProtection.md) collection|List properties and relationships of the [managedAppProtection](../resources/managedappprotection.md) objects.|
|[Get managedAppProtection](../api/managedappprotection-get.md)|[managedAppProtection](../resources/managedAppProtection.md)|Read properties and relationships of the [managedAppProtection](../resources/managedappprotection.md) object.|
|[targetApps](../api/managedappprotection-targetapps.md)|None||
|[targetApps](../api/managedappprotection-targetapps.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedDataIngestionLocations|Enumeration collection|Data storage locations where a user may store managed data.|
|allowedDataStorageLocations|Enumeration collection|Data storage locations where a user may store managed data.|
|allowedInboundDataTransferSources|Enumeration|Sources from which data is allowed to be transferred. Possible values are: `allApps`, `managedApps`, `none`.|
|allowedOutboundClipboardSharingExceptionLength|Int32|Specify the number of characters that may be cut or copied from Org data and accounts to any application. This setting overrides the AllowedOutboundClipboardSharingLevel restriction. Default value of '0' means no exception is allowed.|
|allowedOutboundClipboardSharingLevel|Enumeration|The level to which the clipboard may be shared between apps on the managed device. Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|allowedOutboundDataTransferDestinations|Enumeration|Destinations to which data is allowed to be transferred. Possible values are: `allApps`, `managedApps`, `none`.|
|appActionIfDeviceComplianceRequired|Enumeration|Defines a managed app behavior, either block or wipe, when the device is either rooted or jailbroken, if DeviceComplianceRequired is set to true. Possible values are: `block`, `wipe`, `warn`.|
|appActionIfMaximumPinRetriesExceeded|Enumeration|Defines a managed app behavior, either block or wipe, based on maximum number of incorrect pin retry attempts. Possible values are: `block`, `wipe`, `warn`.|
|blockDataIngestionIntoOrganizationDocuments|Boolean|Indicates whether a user can bring data into org documents.|
|contactSyncBlocked|Boolean|Indicates whether contacts can be synced to the user's device.|
|createdDateTime|DateTimeOffset|The date and time the policy was created. Inherited from [managedAppPolicy](../resources/managedAppPolicy.md)|
|dataBackupBlocked|Boolean|Indicates whether the backup of a managed app's data is blocked.|
|description|String|The policy's description. Inherited from [managedAppPolicy](../resources/managedAppPolicy.md)|
|deviceComplianceRequired|Boolean|Indicates whether device compliance is required.|
|disableAppPinIfDevicePinIsSet|Boolean|Indicates whether use of the app pin is required if the device pin is set.|
|displayName|String|Policy display name. Inherited from [managedAppPolicy](../resources/managedAppPolicy.md)|
|fingerprintBlocked|Boolean|Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Last time the policy was modified. Inherited from [managedAppPolicy](../resources/managedAppPolicy.md)|
|managedBrowser|Enumeration|Indicates in which managed browser(s) that internet links should be opened. Possible values are: `notConfigured`, `microsoftEdge`.|
|managedBrowserToOpenLinksRequired|Boolean|Indicates whether internet links should be opened in the managed browser app.|
|maximumAllowedDeviceThreatLevel|Enumeration|Maximum allowed device threat level, as reported by the MTD app. Possible values are: `notConfigured`, `secured`, `low`, `medium`, `high`.|
|maximumPinRetries|Int32|Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.|
|minimumPinLength|Int32|Minimum pin length required for an app-level pin if PinRequired is set to True|
|minimumRequiredAppVersion|String|Versions less than the specified version will block the managed app from accessing company data.|
|minimumRequiredOsVersion|String|Versions less than the specified version will block the managed app from accessing company data.|
|minimumWarningAppVersion|String|Versions less than the specified version will result in warning message on the managed app.|
|minimumWarningOsVersion|String|Versions less than the specified version will result in warning message on the managed app from accessing company data.|
|minimumWipeAppVersion|String|Versions less than or equal to the specified version will wipe the managed app and the associated company data.|
|minimumWipeOsVersion|String|Versions less than or equal to the specified version will wipe the managed app and the associated company data.|
|mobileThreatDefenseRemediationAction|Enumeration|Determines what action to take if the mobile threat defense threat threshold isn't met. Warn isn't a supported value for this property. Possible values are: `block`, `wipe`, `warn`.|
|notificationRestriction|Enumeration|Specify app notification restriction. Possible values are: `allow`, `blockOrganizationalData`, `block`.|
|organizationalCredentialsRequired|Boolean|Indicates whether organizational credentials are required for app use.|
|periodBeforePinReset|Duration|TimePeriod before the all-level pin must be reset if PinRequired is set to True.|
|periodOfflineBeforeAccessCheck|Duration|The period after which access is checked when the device is not connected to the internet.|
|periodOfflineBeforeWipeIsEnforced|Duration|The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.|
|periodOnlineBeforeAccessCheck|Duration|The period after which access is checked when the device is connected to the internet.|
|pinCharacterSet|Enumeration|Character set which may be used for an app-level pin if PinRequired is set to True. Possible values are: `numeric`, `alphanumericAndSymbol`.|
|pinRequired|Boolean|Indicates whether an app-level pin is required.|
|pinRequiredInsteadOfBiometricTimeout|Duration|Timeout in minutes for an app pin instead of non biometrics passcode|
|previousPinBlockCount|Int32|Requires a pin to be unique from the number specified in this property.|
|printBlocked|Boolean|Indicates whether printing is allowed from managed apps.|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [managedAppPolicy](../resources/managedAppPolicy.md)|
|saveAsBlocked|Boolean|Indicates whether users may use the "Save As" menu item to save a copy of protected files.|
|simplePinBlocked|Boolean|Indicates whether simplePin is blocked.|
|version|String|Version of the entity. Inherited from [managedAppPolicy](../resources/managedAppPolicy.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppProtection",
  "baseType": "microsoft.graph.managedAppPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppProtection",
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
  ]
}
```

