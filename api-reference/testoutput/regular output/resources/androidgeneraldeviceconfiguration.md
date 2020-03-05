---
title: "androidGeneralDeviceConfiguration resource type"
description: "This topic provides descriptions of the declared methods, properties and relationships exposed by the androidGeneralDeviceConfiguration resource."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# androidGeneralDeviceConfiguration resource type


Namespace: microsoft.graph

This topic provides descriptions of the declared methods, properties and relationships exposed by the androidGeneralDeviceConfiguration resource.


Inherits from [deviceConfiguration](../resources/deviceconfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List androidGeneralDeviceConfigurations](../api/androidgeneraldeviceconfiguration-list.md)|[androidGeneralDeviceConfiguration](../resources/androidgeneraldeviceconfiguration.md) collection|List properties and relationships of the [androidGeneralDeviceConfiguration](../resources/androidgeneraldeviceconfiguration.md) objects.|
|[Get androidGeneralDeviceConfiguration](../api/androidgeneraldeviceconfiguration-get.md)|[androidGeneralDeviceConfiguration](../resources/androidgeneraldeviceconfiguration.md)|Read properties and relationships of the [androidGeneralDeviceConfiguration](../resources/androidgeneraldeviceconfiguration.md) object.|
|[Create androidGeneralDeviceConfiguration](../api/androidgeneraldeviceconfiguration-create.md)|[androidGeneralDeviceConfiguration](../resources/androidgeneraldeviceconfiguration.md)|Create a new [androidGeneralDeviceConfiguration](../resources/androidgeneraldeviceconfiguration.md) object.|
|[Delete androidGeneralDeviceConfiguration](../api/androidgeneraldeviceconfiguration-delete.md)|None|Deletes a [androidGeneralDeviceConfiguration](../resources/androidgeneraldeviceconfiguration.md).|
|[Update androidGeneralDeviceConfiguration](../api/androidgeneraldeviceconfiguration-update.md)|[androidGeneralDeviceConfiguration](../resources/androidgeneraldeviceconfiguration.md)|Update the properties of a [androidGeneralDeviceConfiguration](../resources/androidgeneraldeviceconfiguration.md) object.|
|[assign](../api/androidgeneraldeviceconfiguration-assign.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection||
|[List assignments](../api/androidgeneraldeviceconfiguration-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/androidgeneraldeviceconfiguration-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/androidgeneraldeviceconfiguration-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Get the deviceConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/androidgeneraldeviceconfiguration-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/androidgeneraldeviceconfiguration-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Get the deviceConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/androidgeneraldeviceconfiguration-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[Get deviceConfigurationUserOverview](../api/deviceconfigurationuseroverview-get.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Read properties and relationships of the [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/androidgeneraldeviceconfiguration-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/androidgeneraldeviceconfiguration-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appsBlockClipboardSharing|Boolean|Indicates whether or not to block clipboard sharing to copy and paste between applications.|
|appsBlockCopyPaste|Boolean|Indicates whether or not to block copy and paste within applications.|
|appsBlockYouTube|Boolean|Indicates whether or not to block the YouTube app.|
|appsHideList|[appListItem](../resources/applistitem.md) collection|List of apps to be hidden on the KNOX device. This collection can contain a maximum of 500 elements.|
|appsInstallAllowList|[appListItem](../resources/applistitem.md) collection|List of apps which can be installed on the KNOX device. This collection can contain a maximum of 500 elements.|
|appsLaunchBlockList|[appListItem](../resources/applistitem.md) collection|List of apps which are blocked from being launched on the KNOX device. This collection can contain a maximum of 500 elements.|
|bluetoothBlocked|Boolean|Indicates whether or not to block Bluetooth.|
|cameraBlocked|Boolean|Indicates whether or not to block the use of the camera.|
|cellularBlockDataRoaming|Boolean|Indicates whether or not to block data roaming.|
|cellularBlockMessaging|Boolean|Indicates whether or not to block SMS/MMS messaging.|
|cellularBlockVoiceRoaming|Boolean|Indicates whether or not to block voice roaming.|
|cellularBlockWiFiTethering|Boolean|Indicates whether or not to block syncing Wi-Fi tethering.|
|compliantAppListType|Enumeration|Type of list that is in the CompliantAppsList. Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|compliantAppsList|[appListItem](../resources/applistitem.md) collection|List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType). This collection can contain a maximum of 10000 elements.|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceSharingAllowed|Boolean|Indicates whether or not to allow device sharing mode.|
|diagnosticDataBlockSubmission|Boolean|Indicates whether or not to block diagnostic data submission.|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|factoryResetBlocked|Boolean|Indicates whether or not to block user performing a factory reset.|
|googleAccountBlockAutoSync|Boolean|Indicates whether or not to block Google account auto sync.|
|googlePlayStoreBlocked|Boolean|Indicates whether or not to block the Google Play store.|
|id|String| Inherited from [entity](../resources/entity.md)|
|kioskModeApps|[appListItem](../resources/applistitem.md) collection|A list of apps that will be allowed to run when the device is in Kiosk Mode. This collection can contain a maximum of 500 elements.|
|kioskModeBlockSleepButton|Boolean|Indicates whether or not to block the screen sleep button while in Kiosk Mode.|
|kioskModeBlockVolumeButtons|Boolean|Indicates whether or not to block the volume buttons while in Kiosk Mode.|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|locationServicesBlocked|Boolean|Indicates whether or not to block location services.|
|nfcBlocked|Boolean|Indicates whether or not to block Near-Field Communication.|
|passwordBlockFingerprintUnlock|Boolean|Indicates whether or not to block fingerprint unlock.|
|passwordBlockTrustAgents|Boolean|Indicates whether or not to block Smart Lock and other trust agents.|
|passwordExpirationDays|Int32|Number of days before the password expires. Valid values 1 to 365|
|passwordMinimumLength|Int32|Minimum length of passwords. Valid values 4 to 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Minutes of inactivity before the screen times out.|
|passwordPreviousPasswordBlockCount|Int32|Number of previous passwords to block. Valid values 0 to 24|
|passwordRequired|Boolean|Indicates whether or not to require a password.|
|passwordRequiredType|Enumeration|Type of password that is required. Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Number of sign in failures allowed before factory reset. Valid values 1 to 16|
|powerOffBlocked|Boolean|Indicates whether or not to block powering off the device.|
|screenCaptureBlocked|Boolean|Indicates whether or not to block screenshots.|
|securityRequireVerifyApps|Boolean|Require the Android Verify apps feature is turned on.|
|storageBlockGoogleBackup|Boolean|Indicates whether or not to block Google Backup.|
|storageBlockRemovableStorage|Boolean|Indicates whether or not to block removable storage usage.|
|storageRequireDeviceEncryption|Boolean|Indicates whether or not to require device encryption.|
|storageRequireRemovableStorageEncryption|Boolean|Indicates whether or not to require removable storage encryption.|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|voiceAssistantBlocked|Boolean|Indicates whether or not to block the use of the Voice Assistant.|
|voiceDialingBlocked|Boolean|Indicates whether or not to block voice dialing.|
|webBrowserBlockAutofill|Boolean|Indicates whether or not to block the web browser's auto fill feature.|
|webBrowserBlocked|Boolean|Indicates whether or not to block the web browser.|
|webBrowserBlockJavaScript|Boolean|Indicates whether or not to block JavaScript within the web browser.|
|webBrowserBlockPopups|Boolean|Indicates whether or not to block popups within the web browser.|
|webBrowserCookieSettings|Enumeration|Cookie settings within the web browser. Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.|
|wiFiBlocked|Boolean|Indicates whether or not to block syncing Wi-Fi.|

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
  "@odata.type": "microsoft.graph.androidGeneralDeviceConfiguration",
  "baseType": "microsoft.graph.deviceConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
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
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "passwordRequiredType": "String",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "String",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem"
    }
  ],
  "securityRequireVerifyApps": true
}
```

