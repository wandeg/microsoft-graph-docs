---
title: "androidWorkProfileCustomConfiguration resource type"
description: "Android Work Profile custom configuration"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# androidWorkProfileCustomConfiguration resource type

Android Work Profile custom configuration


Inherits from [deviceConfiguration](../resources/deviceConfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List androidWorkProfileCustomConfigurations](../api/androidworkprofilecustomconfiguration-list.md)|[androidWorkProfileCustomConfiguration](../resources/androidWorkProfileCustomConfiguration.md) collection|List properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/androidworkprofilecustomconfiguration.md) objects.|
|[Get androidWorkProfileCustomConfiguration](../api/androidworkprofilecustomconfiguration-get.md)|[androidWorkProfileCustomConfiguration](../resources/androidWorkProfileCustomConfiguration.md)|Read properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/androidworkprofilecustomconfiguration.md) object.|
|[Create androidWorkProfileCustomConfiguration](../api/androidworkprofilecustomconfiguration-create.md)|[androidWorkProfileCustomConfiguration](../resources/androidWorkProfileCustomConfiguration.md)|Create a new [androidWorkProfileCustomConfiguration](../resources/androidworkprofilecustomconfiguration.md) object.|
|[Delete androidWorkProfileCustomConfiguration](../api/androidworkprofilecustomconfiguration-delete.md)|None|Deletes a [androidWorkProfileCustomConfiguration](../resources/androidworkprofilecustomconfiguration.md).|
|[Update androidWorkProfileCustomConfiguration](../api/androidworkprofilecustomconfiguration-update.md)|[androidWorkProfileCustomConfiguration](../resources/androidWorkProfileCustomConfiguration.md)|Update the properties of a [androidWorkProfileCustomConfiguration](../resources/androidworkprofilecustomconfiguration.md) object.|
|[assign](../api/androidworkprofilecustomconfiguration-assign.md)|[deviceConfigurationAssignment](../resources/deviceConfigurationAssignment.md) collection||
|[List assignments](../api/androidworkprofilecustomconfiguration-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceConfigurationAssignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/androidworkprofilecustomconfiguration-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceConfigurationAssignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/androidworkprofilecustomconfiguration-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceConfigurationDeviceStatus.md) collection|Get the deviceConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/androidworkprofilecustomconfiguration-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceConfigurationDeviceStatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/androidworkprofilecustomconfiguration-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceConfigurationUserStatus.md) collection|Get the deviceConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/androidworkprofilecustomconfiguration-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceConfigurationUserStatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceConfigurationDeviceOverview.md)|Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[Get deviceConfigurationUserOverview](../api/deviceconfigurationuseroverview-get.md)|[deviceConfigurationUserOverview](../resources/deviceConfigurationUserOverview.md)|Read properties and relationships of the [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/androidworkprofilecustomconfiguration-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/androidworkprofilecustomconfiguration-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|omaSettings|[omaSetting](../resources/omaSetting.md) collection|OMA settings. This collection can contain a maximum of 500 elements.|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/deviceConfigurationAssignment.md) collection|The list of assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md) collection|Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/deviceConfigurationDeviceStatus.md) collection|Device configuration installation status by device. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/deviceConfigurationDeviceOverview.md)|Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/deviceConfigurationUserStatus.md) collection|Device configuration installation status by user. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/deviceConfigurationUserOverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidWorkProfileCustomConfiguration",
  "baseType": "microsoft.graph.deviceConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "omaUri": "String",
      "value": 1024
    }
  ]
}
```

