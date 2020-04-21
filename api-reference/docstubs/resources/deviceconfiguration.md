---
title: "deviceConfiguration resource type"
description: "Device Configuration."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# deviceConfiguration resource type


Namespace: microsoft.graph

Device Configuration.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceConfiguration](../api/deviceconfiguration-get.md)|[deviceConfiguration](../resources/deviceconfiguration.md)|Read properties and relationships of a [deviceConfiguration](../resources/deviceconfiguration.md) object.|
|[assign](../api/deviceconfiguration-assign.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|**TODO: Add Description**|
|[List assignments](../api/deviceconfiguration-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Create assignments](../api/deviceconfiguration-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/deviceconfiguration-delete-assignments.md)|None|Delete an assignments object.|
|[Update assignments](../api/deviceconfiguration-update-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Update the properties of an assignments object.|
|[Get deviceConfigurationAssignment](../api/deviceconfigurationassignment-get.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Read properties and relationships of a [deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) object.|
|[List deviceStatuses](../api/deviceconfiguration-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Get the deviceConfigurationDeviceStatus from the deviceStatuses navigation property.|
|[Create deviceStatuses](../api/deviceconfiguration-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Create a new deviceStatuses object.|
|[Delete deviceStatuses](../api/deviceconfiguration-delete-devicestatuses.md)|None|Delete a deviceStatuses object.|
|[Update deviceStatuses](../api/deviceconfiguration-update-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Update the properties of a deviceStatuses object.|
|[Get deviceConfigurationDeviceStatus](../api/deviceconfigurationdevicestatus-get.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Read properties and relationships of a [deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) object.|
|[List userStatuses](../api/deviceconfiguration-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Get the deviceConfigurationUserStatus from the userStatuses navigation property.|
|[Create userStatuses](../api/deviceconfiguration-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Create a new userStatuses object.|
|[Delete userStatuses](../api/deviceconfiguration-delete-userstatuses.md)|None|Delete an userStatuses object.|
|[Update userStatuses](../api/deviceconfiguration-update-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Update the properties of an userStatuses object.|
|[Get deviceConfigurationUserStatus](../api/deviceconfigurationuserstatus-get.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Read properties and relationships of a [deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) object.|
|[List deviceStatusOverview](../api/deviceconfiguration-list-devicestatusoverview.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) collection|Get the deviceConfigurationDeviceOverviews from the deviceStatusOverview navigation property.|
|[Create deviceStatusOverview](../api/deviceconfiguration-post-devicestatusoverview.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Create a new deviceStatusOverview object.|
|[Delete deviceStatusOverview](../api/deviceconfiguration-delete-devicestatusoverview.md)|None|Delete a deviceStatusOverview object.|
|[Update deviceStatusOverview](../api/deviceconfiguration-update-devicestatusoverview.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Update the properties of a deviceStatusOverview object.|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Read properties and relationships of a [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[List userStatusOverview](../api/deviceconfiguration-list-userstatusoverview.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) collection|Get the deviceConfigurationUserOverviews from the userStatusOverview navigation property.|
|[Create userStatusOverview](../api/deviceconfiguration-post-userstatusoverview.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Create a new userStatusOverview object.|
|[Delete userStatusOverview](../api/deviceconfiguration-delete-userstatusoverview.md)|None|Delete an userStatusOverview object.|
|[Update userStatusOverview](../api/deviceconfiguration-update-userstatusoverview.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Update the properties of an userStatusOverview object.|
|[Get deviceConfigurationUserOverview](../api/deviceconfigurationuseroverview-get.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Read properties and relationships of a [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/deviceconfiguration-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Create deviceSettingStateSummaries](../api/deviceconfiguration-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Create a new deviceSettingStateSummaries object.|
|[Delete deviceSettingStateSummaries](../api/deviceconfiguration-delete-devicesettingstatesummaries.md)|None|Delete a deviceSettingStateSummaries object.|
|[Update deviceSettingStateSummaries](../api/deviceconfiguration-update-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Update the properties of a deviceSettingStateSummaries object.|
|[Get settingStateDeviceSummary](../api/settingstatedevicesummary-get.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Read properties and relationships of a [settingStateDeviceSummary](../resources/settingstatedevicesummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|DateTime the object was created.|
|description|String|Admin provided description of the Device Configuration.|
|displayName|String|Admin provided name of the device configuration.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|version|Int32|Version of the device configuration.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|The list of assignments for the device configuration profile.|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Device Configuration Setting State Device Summary|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Device configuration installation status by device.|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Device Configuration devices status overview|
|userStatuses|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Device configuration installation status by user.|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Device Configuration users status overview|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfiguration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024
}
```

