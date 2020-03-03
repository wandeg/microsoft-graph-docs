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
|allowedDataStorageLocations|Enumeration collection|Data storage locations where a user may store managed data.|
|allowedInboundDataTransferSources|Enumeration|Sources from which data is allowed to be transferred. Possible values are: `allApps`, `managedApps`, `none`.|
|allowedOutboundClipboardSharingLevel|Enumeration|The level to which the clipboard may be shared between apps on the managed device. Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|allowedOutboundDataTransferDestinations|Enumeration|Destinations to which data is allowed to be transferred. Possible values are: `allApps`, `managedApps`, `none`.|
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
|managedBrowserToOpenLinksRequired|Boolean|Indicates whether internet links should be opened in the managed browser app.|
|maximumPinRetries|Int32|Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.|
|minimumPinLength|Int32|Minimum pin length required for an app-level pin if PinRequired is set to True|
|minimumRequiredAppVersion|String|Versions less than the specified version will block the managed app from accessing company data.|
|minimumRequiredOsVersion|String|Versions less than the specified version will block the managed app from accessing company data.|
|minimumWarningAppVersion|String|Versions less than the specified version will result in warning message on the managed app.|
|minimumWarningOsVersion|String|Versions less than the specified version will result in warning message on the managed app from accessing company data.|
|organizationalCredentialsRequired|Boolean|Indicates whether organizational credentials are required for app use.|
|periodBeforePinReset|Duration|TimePeriod before the all-level pin must be reset if PinRequired is set to True.|
|periodOfflineBeforeAccessCheck|Duration|The period after which access is checked when the device is not connected to the internet.|
|periodOfflineBeforeWipeIsEnforced|Duration|The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.|
|periodOnlineBeforeAccessCheck|Duration|The period after which access is checked when the device is connected to the internet.|
|pinCharacterSet|Enumeration|Character set which may be used for an app-level pin if PinRequired is set to True. Possible values are: `numeric`, `alphanumericAndSymbol`.|
|pinRequired|Boolean|Indicates whether an app-level pin is required.|
|printBlocked|Boolean|Indicates whether printing is allowed from managed apps.|
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
  "minimumWarningAppVersion": "String"
}
```

