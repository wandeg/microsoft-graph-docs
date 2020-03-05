---
title: "iosDeviceFeaturesConfiguration resource type"
description: "iOS Device Features Configuration Profile."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosDeviceFeaturesConfiguration resource type


Namespace: microsoft.graph

iOS Device Features Configuration Profile.


Inherits from [appleDeviceFeaturesConfigurationBase](../resources/appledevicefeaturesconfigurationbase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List iosDeviceFeaturesConfigurations](../api/iosdevicefeaturesconfiguration-list.md)|[iosDeviceFeaturesConfiguration](../resources/iosdevicefeaturesconfiguration.md) collection|List properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/iosdevicefeaturesconfiguration.md) objects.|
|[Get iosDeviceFeaturesConfiguration](../api/iosdevicefeaturesconfiguration-get.md)|[iosDeviceFeaturesConfiguration](../resources/iosdevicefeaturesconfiguration.md)|Read properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/iosdevicefeaturesconfiguration.md) object.|
|[Create iosDeviceFeaturesConfiguration](../api/iosdevicefeaturesconfiguration-create.md)|[iosDeviceFeaturesConfiguration](../resources/iosdevicefeaturesconfiguration.md)|Create a new [iosDeviceFeaturesConfiguration](../resources/iosdevicefeaturesconfiguration.md) object.|
|[Delete iosDeviceFeaturesConfiguration](../api/iosdevicefeaturesconfiguration-delete.md)|None|Deletes a [iosDeviceFeaturesConfiguration](../resources/iosdevicefeaturesconfiguration.md).|
|[Update iosDeviceFeaturesConfiguration](../api/iosdevicefeaturesconfiguration-update.md)|[iosDeviceFeaturesConfiguration](../resources/iosdevicefeaturesconfiguration.md)|Update the properties of a [iosDeviceFeaturesConfiguration](../resources/iosdevicefeaturesconfiguration.md) object.|
|[List assignments](../api/iosdevicefeaturesconfiguration-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/iosdevicefeaturesconfiguration-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/iosdevicefeaturesconfiguration-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Get the deviceConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/iosdevicefeaturesconfiguration-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/iosdevicefeaturesconfiguration-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Get the deviceConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/iosdevicefeaturesconfiguration-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[Get deviceConfigurationUserOverview](../api/deviceconfigurationuseroverview-get.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Read properties and relationships of the [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/iosdevicefeaturesconfiguration-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/iosdevicefeaturesconfiguration-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assetTagTemplate|String|Asset tag information for the device, displayed on the login window and lock screen.|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|homeScreenDockIcons|[iosHomeScreenItem](../resources/ioshomescreenitem.md) collection|A list of app and folders to appear on the Home Screen Dock. This collection can contain a maximum of 500 elements.|
|homeScreenPages|[iosHomeScreenPage](../resources/ioshomescreenpage.md) collection|A list of pages on the Home Screen. This collection can contain a maximum of 500 elements.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|lockScreenFootnote|String|A footnote displayed on the login window and lock screen. Available in iOS 9.3.1 and later.|
|notificationSettings|[iosNotificationSettings](../resources/iosnotificationsettings.md) collection|Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later). This collection can contain a maximum of 500 elements.|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|

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
  "@odata.type": "microsoft.graph.iosDeviceFeaturesConfiguration",
  "baseType": "microsoft.graph.appleDeviceFeaturesConfigurationBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "assetTagTemplate": "String",
  "lockScreenFootnote": "String",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "bundleID": "String"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder"
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "appName": "String",
      "publisher": "String",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "String",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ]
}
```

