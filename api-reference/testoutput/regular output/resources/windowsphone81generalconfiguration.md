---
title: "windowsPhone81GeneralConfiguration resource type"
description: "This topic provides descriptions of the declared methods, properties and relationships exposed by the windowsPhone81GeneralConfiguration resource."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsPhone81GeneralConfiguration resource type


Namespace: microsoft.graph

This topic provides descriptions of the declared methods, properties and relationships exposed by the windowsPhone81GeneralConfiguration resource.


Inherits from [deviceConfiguration](../resources/deviceconfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windowsPhone81GeneralConfigurations](../api/windowsphone81generalconfiguration-list.md)|[windowsPhone81GeneralConfiguration](../resources/windowsphone81generalconfiguration.md) collection|List properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/windowsphone81generalconfiguration.md) objects.|
|[Get windowsPhone81GeneralConfiguration](../api/windowsphone81generalconfiguration-get.md)|[windowsPhone81GeneralConfiguration](../resources/windowsphone81generalconfiguration.md)|Read properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/windowsphone81generalconfiguration.md) object.|
|[Create windowsPhone81GeneralConfiguration](../api/windowsphone81generalconfiguration-create.md)|[windowsPhone81GeneralConfiguration](../resources/windowsphone81generalconfiguration.md)|Create a new [windowsPhone81GeneralConfiguration](../resources/windowsphone81generalconfiguration.md) object.|
|[Delete windowsPhone81GeneralConfiguration](../api/windowsphone81generalconfiguration-delete.md)|None|Deletes a [windowsPhone81GeneralConfiguration](../resources/windowsphone81generalconfiguration.md).|
|[Update windowsPhone81GeneralConfiguration](../api/windowsphone81generalconfiguration-update.md)|[windowsPhone81GeneralConfiguration](../resources/windowsphone81generalconfiguration.md)|Update the properties of a [windowsPhone81GeneralConfiguration](../resources/windowsphone81generalconfiguration.md) object.|
|[assign](../api/windowsphone81generalconfiguration-assign.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection||
|[List assignments](../api/windowsphone81generalconfiguration-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/windowsphone81generalconfiguration-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/windowsphone81generalconfiguration-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Get the deviceConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/windowsphone81generalconfiguration-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/windowsphone81generalconfiguration-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Get the deviceConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/windowsphone81generalconfiguration-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[Get deviceConfigurationUserOverview](../api/deviceconfigurationuseroverview-get.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Read properties and relationships of the [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/windowsphone81generalconfiguration-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/windowsphone81generalconfiguration-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applyOnlyToWindowsPhone81|Boolean|Value indicating whether this policy only applies to Windows Phone 8.1. This property is read-only.|
|appsBlockCopyPaste|Boolean|Indicates whether or not to block copy paste.|
|bluetoothBlocked|Boolean|Indicates whether or not to block bluetooth.|
|cameraBlocked|Boolean|Indicates whether or not to block camera.|
|cellularBlockWifiTethering|Boolean|Indicates whether or not to block Wi-Fi tethering. Has no impact if Wi-Fi is blocked.|
|compliantAppListType|Enumeration|List that is in the AppComplianceList. Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|compliantAppsList|[appListItem](../resources/applistitem.md) collection|List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType). This collection can contain a maximum of 10000 elements.|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|diagnosticDataBlockSubmission|Boolean|Indicates whether or not to block diagnostic data submission.|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|emailBlockAddingAccounts|Boolean|Indicates whether or not to block custom email accounts.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|locationServicesBlocked|Boolean|Indicates whether or not to block location services.|
|microsoftAccountBlocked|Boolean|Indicates whether or not to block using a Microsoft Account.|
|nfcBlocked|Boolean|Indicates whether or not to block Near-Field Communication.|
|passwordBlockSimple|Boolean|Indicates whether or not to block syncing the calendar.|
|passwordExpirationDays|Int32|Number of days before the password expires.|
|passwordMinimumCharacterSetCount|Int32|Number of character sets a password must contain.|
|passwordMinimumLength|Int32|Minimum length of passwords.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Minutes of inactivity before screen timeout.|
|passwordPreviousPasswordBlockCount|Int32|Number of previous passwords to block. Valid values 0 to 24|
|passwordRequired|Boolean|Indicates whether or not to require a password.|
|passwordRequiredType|Enumeration|Password type that is required. Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Number of sign in failures allowed before factory reset.|
|screenCaptureBlocked|Boolean|Indicates whether or not to block screenshots.|
|storageBlockRemovableStorage|Boolean|Indicates whether or not to block removable storage.|
|storageRequireEncryption|Boolean|Indicates whether or not to require encryption.|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|webBrowserBlocked|Boolean|Indicates whether or not to block the web browser.|
|wifiBlockAutomaticConnectHotspots|Boolean|Indicates whether or not to block automatically connecting to Wi-Fi hotspots. Has no impact if Wi-Fi is blocked.|
|wifiBlocked|Boolean|Indicates whether or not to block Wi-Fi.|
|wifiBlockHotspotReporting|Boolean|Indicates whether or not to block Wi-Fi hotspot reporting. Has no impact if Wi-Fi is blocked.|
|windowsStoreBlocked|Boolean|Indicates whether or not to block the Windows Store.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|The list of assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Device configuration installation status by device. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Device configuration installation status by user. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPhone81GeneralConfiguration",
  "baseType": "microsoft.graph.deviceConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "compliantAppListType": "String",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "passwordRequiredType": "String",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```

