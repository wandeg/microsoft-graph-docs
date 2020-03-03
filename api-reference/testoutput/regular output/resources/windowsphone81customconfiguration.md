---
title: "windowsPhone81CustomConfiguration resource type"
description: "This topic provides descriptions of the declared methods, properties and relationships exposed by the windowsPhone81CustomConfiguration resource."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# windowsPhone81CustomConfiguration resource type

This topic provides descriptions of the declared methods, properties and relationships exposed by the windowsPhone81CustomConfiguration resource.


Inherits from [deviceConfiguration](../resources/deviceConfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windowsPhone81CustomConfigurations](../api/windowsphone81customconfiguration-list.md)|[windowsPhone81CustomConfiguration](../resources/windowsPhone81CustomConfiguration.md) collection|List properties and relationships of the [windowsPhone81CustomConfiguration](../resources/windowsphone81customconfiguration.md) objects.|
|[Get windowsPhone81CustomConfiguration](../api/windowsphone81customconfiguration-get.md)|[windowsPhone81CustomConfiguration](../resources/windowsPhone81CustomConfiguration.md)|Read properties and relationships of the [windowsPhone81CustomConfiguration](../resources/windowsphone81customconfiguration.md) object.|
|[Create windowsPhone81CustomConfiguration](../api/windowsphone81customconfiguration-create.md)|[windowsPhone81CustomConfiguration](../resources/windowsPhone81CustomConfiguration.md)|Create a new [windowsPhone81CustomConfiguration](../resources/windowsphone81customconfiguration.md) object.|
|[Delete windowsPhone81CustomConfiguration](../api/windowsphone81customconfiguration-delete.md)|None|Deletes a [windowsPhone81CustomConfiguration](../resources/windowsphone81customconfiguration.md).|
|[Update windowsPhone81CustomConfiguration](../api/windowsphone81customconfiguration-update.md)|[windowsPhone81CustomConfiguration](../resources/windowsPhone81CustomConfiguration.md)|Update the properties of a [windowsPhone81CustomConfiguration](../resources/windowsphone81customconfiguration.md) object.|
|[assign](../api/windowsphone81customconfiguration-assign.md)|[deviceConfigurationAssignment](../resources/deviceConfigurationAssignment.md) collection||
|[List assignments](../api/windowsphone81customconfiguration-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceConfigurationAssignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/windowsphone81customconfiguration-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceConfigurationAssignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/windowsphone81customconfiguration-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceConfigurationDeviceStatus.md) collection|Get the deviceConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/windowsphone81customconfiguration-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceConfigurationDeviceStatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/windowsphone81customconfiguration-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceConfigurationUserStatus.md) collection|Get the deviceConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/windowsphone81customconfiguration-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceConfigurationUserStatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceConfigurationDeviceOverview.md)|Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[Get deviceConfigurationUserOverview](../api/deviceconfigurationuseroverview-get.md)|[deviceConfigurationUserOverview](../resources/deviceConfigurationUserOverview.md)|Read properties and relationships of the [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/windowsphone81customconfiguration-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/windowsphone81customconfiguration-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|omaSettings|[omaSetting](../resources/omaSetting.md) collection|OMA settings. This collection can contain a maximum of 1000 elements.|
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
  "@odata.type": "microsoft.graph.windowsPhone81CustomConfiguration",
  "baseType": "microsoft.graph.deviceConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
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

