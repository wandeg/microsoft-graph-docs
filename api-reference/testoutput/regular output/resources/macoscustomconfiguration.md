---
title: "macOSCustomConfiguration resource type"
description: "This topic provides descriptions of the declared methods, properties and relationships exposed by the macOSCustomConfiguration resource."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# macOSCustomConfiguration resource type

This topic provides descriptions of the declared methods, properties and relationships exposed by the macOSCustomConfiguration resource.


Inherits from [deviceConfiguration](../resources/deviceConfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List macOSCustomConfigurations](../api/macoscustomconfiguration-list.md)|[macOSCustomConfiguration](../resources/macOSCustomConfiguration.md) collection|List properties and relationships of the [macOSCustomConfiguration](../resources/macoscustomconfiguration.md) objects.|
|[Get macOSCustomConfiguration](../api/macoscustomconfiguration-get.md)|[macOSCustomConfiguration](../resources/macOSCustomConfiguration.md)|Read properties and relationships of the [macOSCustomConfiguration](../resources/macoscustomconfiguration.md) object.|
|[Create macOSCustomConfiguration](../api/macoscustomconfiguration-create.md)|[macOSCustomConfiguration](../resources/macOSCustomConfiguration.md)|Create a new [macOSCustomConfiguration](../resources/macoscustomconfiguration.md) object.|
|[Delete macOSCustomConfiguration](../api/macoscustomconfiguration-delete.md)|None|Deletes a [macOSCustomConfiguration](../resources/macoscustomconfiguration.md).|
|[Update macOSCustomConfiguration](../api/macoscustomconfiguration-update.md)|[macOSCustomConfiguration](../resources/macOSCustomConfiguration.md)|Update the properties of a [macOSCustomConfiguration](../resources/macoscustomconfiguration.md) object.|
|[assign](../api/macoscustomconfiguration-assign.md)|[deviceConfigurationAssignment](../resources/deviceConfigurationAssignment.md) collection||
|[List assignments](../api/macoscustomconfiguration-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceConfigurationAssignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/macoscustomconfiguration-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceConfigurationAssignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/macoscustomconfiguration-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceConfigurationDeviceStatus.md) collection|Get the deviceConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/macoscustomconfiguration-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceConfigurationDeviceStatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/macoscustomconfiguration-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceConfigurationUserStatus.md) collection|Get the deviceConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/macoscustomconfiguration-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceConfigurationUserStatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceConfigurationDeviceOverview.md)|Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[Get deviceConfigurationUserOverview](../api/deviceconfigurationuseroverview-get.md)|[deviceConfigurationUserOverview](../resources/deviceConfigurationUserOverview.md)|Read properties and relationships of the [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/macoscustomconfiguration-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/macoscustomconfiguration-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|payload|Binary|Payload. (UTF8 encoded byte array)|
|payloadFileName|String|Payload file name (*.mobileconfig | *.xml).|
|payloadName|String|Name that is displayed to the user.|
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
  "@odata.type": "microsoft.graph.macOSCustomConfiguration",
  "baseType": "microsoft.graph.deviceConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "payloadName": "String",
  "payloadFileName": "String",
  "payload": "binary"
}
```

