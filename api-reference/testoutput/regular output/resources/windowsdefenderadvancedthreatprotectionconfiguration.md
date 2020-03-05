---
title: "windowsDefenderAdvancedThreatProtectionConfiguration resource type"
description: "Windows Defender AdvancedThreatProtection Configuration."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsDefenderAdvancedThreatProtectionConfiguration resource type


Namespace: microsoft.graph

Windows Defender AdvancedThreatProtection Configuration.


Inherits from [deviceConfiguration](../resources/deviceconfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windowsDefenderAdvancedThreatProtectionConfigurations](../api/windowsdefenderadvancedthreatprotectionconfiguration-list.md)|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/windowsdefenderadvancedthreatprotectionconfiguration.md) collection|List properties and relationships of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/windowsdefenderadvancedthreatprotectionconfiguration.md) objects.|
|[Get windowsDefenderAdvancedThreatProtectionConfiguration](../api/windowsdefenderadvancedthreatprotectionconfiguration-get.md)|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/windowsdefenderadvancedthreatprotectionconfiguration.md)|Read properties and relationships of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/windowsdefenderadvancedthreatprotectionconfiguration.md) object.|
|[Create windowsDefenderAdvancedThreatProtectionConfiguration](../api/windowsdefenderadvancedthreatprotectionconfiguration-create.md)|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/windowsdefenderadvancedthreatprotectionconfiguration.md)|Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/windowsdefenderadvancedthreatprotectionconfiguration.md) object.|
|[Delete windowsDefenderAdvancedThreatProtectionConfiguration](../api/windowsdefenderadvancedthreatprotectionconfiguration-delete.md)|None|Deletes a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/windowsdefenderadvancedthreatprotectionconfiguration.md).|
|[Update windowsDefenderAdvancedThreatProtectionConfiguration](../api/windowsdefenderadvancedthreatprotectionconfiguration-update.md)|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/windowsdefenderadvancedthreatprotectionconfiguration.md)|Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/windowsdefenderadvancedthreatprotectionconfiguration.md) object.|
|[assign](../api/windowsdefenderadvancedthreatprotectionconfiguration-assign.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection||
|[List assignments](../api/windowsdefenderadvancedthreatprotectionconfiguration-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/windowsdefenderadvancedthreatprotectionconfiguration-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/windowsdefenderadvancedthreatprotectionconfiguration-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Get the deviceConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/windowsdefenderadvancedthreatprotectionconfiguration-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/windowsdefenderadvancedthreatprotectionconfiguration-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Get the deviceConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/windowsdefenderadvancedthreatprotectionconfiguration-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[Get deviceConfigurationUserOverview](../api/deviceconfigurationuseroverview-get.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Read properties and relationships of the [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/windowsdefenderadvancedthreatprotectionconfiguration-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/windowsdefenderadvancedthreatprotectionconfiguration-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowSampleSharing|Boolean|Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|enableExpeditedTelemetryReporting|Boolean|Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
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
  "@odata.type": "microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "baseType": "microsoft.graph.deviceConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```

