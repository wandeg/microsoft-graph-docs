---
title: "iosCustomConfiguration resource type"
description: "This topic provides descriptions of the declared methods, properties and relationships exposed by the iosCustomConfiguration resource."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosCustomConfiguration resource type


Namespace: microsoft.graph

This topic provides descriptions of the declared methods, properties and relationships exposed by the iosCustomConfiguration resource.


Inherits from [deviceConfiguration](../resources/deviceconfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List iosCustomConfigurations](../api/ioscustomconfiguration-list.md)|[iosCustomConfiguration](../resources/ioscustomconfiguration.md) collection|List properties and relationships of the [iosCustomConfiguration](../resources/ioscustomconfiguration.md) objects.|
|[Get iosCustomConfiguration](../api/ioscustomconfiguration-get.md)|[iosCustomConfiguration](../resources/ioscustomconfiguration.md)|Read properties and relationships of the [iosCustomConfiguration](../resources/ioscustomconfiguration.md) object.|
|[Create iosCustomConfiguration](../api/ioscustomconfiguration-create.md)|[iosCustomConfiguration](../resources/ioscustomconfiguration.md)|Create a new [iosCustomConfiguration](../resources/ioscustomconfiguration.md) object.|
|[Delete iosCustomConfiguration](../api/ioscustomconfiguration-delete.md)|None|Deletes a [iosCustomConfiguration](../resources/ioscustomconfiguration.md).|
|[Update iosCustomConfiguration](../api/ioscustomconfiguration-update.md)|[iosCustomConfiguration](../resources/ioscustomconfiguration.md)|Update the properties of a [iosCustomConfiguration](../resources/ioscustomconfiguration.md) object.|
|[assign](../api/ioscustomconfiguration-assign.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection||
|[List assignments](../api/ioscustomconfiguration-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/ioscustomconfiguration-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/ioscustomconfiguration-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Get the deviceConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/ioscustomconfiguration-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/ioscustomconfiguration-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Get the deviceConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/ioscustomconfiguration-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[Get deviceConfigurationUserOverview](../api/deviceconfigurationuseroverview-get.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Read properties and relationships of the [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/ioscustomconfiguration-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/ioscustomconfiguration-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|payload|Binary|Payload. (UTF8 encoded byte array)|
|payloadFileName|String|Payload file name (*.mobileconfig | *.xml).|
|payloadName|String|Name that is displayed to the user.|
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
  "@odata.type": "microsoft.graph.iosCustomConfiguration",
  "baseType": "microsoft.graph.deviceConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
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

