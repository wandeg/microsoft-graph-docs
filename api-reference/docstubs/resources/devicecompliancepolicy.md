---
title: "deviceCompliancePolicy resource type"
description: "This is the base class for Compliance policy. Compliance policies are platform specific and individual per-platform compliance policies inherit from here. "
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# deviceCompliancePolicy resource type


Namespace: microsoft.graph

This is the base class for Compliance policy. Compliance policies are platform specific and individual per-platform compliance policies inherit from here. 


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceCompliancePolicy](../api/devicecompliancepolicy-get.md)|[deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|Read properties and relationships of a [deviceCompliancePolicy](../resources/devicecompliancepolicy.md) object.|
|[assign](../api/devicecompliancepolicy-assign.md)|[deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md) collection|**TODO: Add Description**|
|[scheduleActionsForRules](../api/devicecompliancepolicy-scheduleactionsforrules.md)|None|**TODO: Add Description**|
|[List scheduledActionsForRule](../api/devicecompliancepolicy-list-scheduledactionsforrule.md)|[deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md) collection|Get the deviceComplianceScheduledActionForRules from the scheduledActionsForRule navigation property.|
|[Create scheduledActionsForRule](../api/devicecompliancepolicy-post-scheduledactionsforrule.md)|[deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md)|Create a new scheduledActionsForRule object.|
|[Delete scheduledActionsForRule](../api/devicecompliancepolicy-delete-scheduledactionsforrule.md)|None|Delete a scheduledActionsForRule object.|
|[Update scheduledActionsForRule](../api/devicecompliancepolicy-update-scheduledactionsforrule.md)|[deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md)|Update the properties of a scheduledActionsForRule object.|
|[Get deviceComplianceScheduledActionForRule](../api/devicecompliancescheduledactionforrule-get.md)|[deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md)|Read properties and relationships of a [deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md) object.|
|[List deviceStatuses](../api/devicecompliancepolicy-list-devicestatuses.md)|[deviceComplianceDeviceStatus](../resources/devicecompliancedevicestatus.md) collection|Get the deviceComplianceDeviceStatus from the deviceStatuses navigation property.|
|[Create deviceStatuses](../api/devicecompliancepolicy-post-devicestatuses.md)|[deviceComplianceDeviceStatus](../resources/devicecompliancedevicestatus.md)|Create a new deviceStatuses object.|
|[Delete deviceStatuses](../api/devicecompliancepolicy-delete-devicestatuses.md)|None|Delete a deviceStatuses object.|
|[Update deviceStatuses](../api/devicecompliancepolicy-update-devicestatuses.md)|[deviceComplianceDeviceStatus](../resources/devicecompliancedevicestatus.md)|Update the properties of a deviceStatuses object.|
|[Get deviceComplianceDeviceStatus](../api/devicecompliancedevicestatus-get.md)|[deviceComplianceDeviceStatus](../resources/devicecompliancedevicestatus.md)|Read properties and relationships of a [deviceComplianceDeviceStatus](../resources/devicecompliancedevicestatus.md) object.|
|[List userStatuses](../api/devicecompliancepolicy-list-userstatuses.md)|[deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md) collection|Get the deviceComplianceUserStatus from the userStatuses navigation property.|
|[Create userStatuses](../api/devicecompliancepolicy-post-userstatuses.md)|[deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md)|Create a new userStatuses object.|
|[Delete userStatuses](../api/devicecompliancepolicy-delete-userstatuses.md)|None|Delete an userStatuses object.|
|[Update userStatuses](../api/devicecompliancepolicy-update-userstatuses.md)|[deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md)|Update the properties of an userStatuses object.|
|[Get deviceComplianceUserStatus](../api/devicecomplianceuserstatus-get.md)|[deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md)|Read properties and relationships of a [deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md) object.|
|[List deviceStatusOverview](../api/devicecompliancepolicy-list-devicestatusoverview.md)|[deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md) collection|Get the deviceComplianceDeviceOverviews from the deviceStatusOverview navigation property.|
|[Create deviceStatusOverview](../api/devicecompliancepolicy-post-devicestatusoverview.md)|[deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md)|Create a new deviceStatusOverview object.|
|[Delete deviceStatusOverview](../api/devicecompliancepolicy-delete-devicestatusoverview.md)|None|Delete a deviceStatusOverview object.|
|[Update deviceStatusOverview](../api/devicecompliancepolicy-update-devicestatusoverview.md)|[deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md)|Update the properties of a deviceStatusOverview object.|
|[Get deviceComplianceDeviceOverview](../api/devicecompliancedeviceoverview-get.md)|[deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md)|Read properties and relationships of a [deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md) object.|
|[List userStatusOverview](../api/devicecompliancepolicy-list-userstatusoverview.md)|[deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md) collection|Get the deviceComplianceUserOverviews from the userStatusOverview navigation property.|
|[Create userStatusOverview](../api/devicecompliancepolicy-post-userstatusoverview.md)|[deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md)|Create a new userStatusOverview object.|
|[Delete userStatusOverview](../api/devicecompliancepolicy-delete-userstatusoverview.md)|None|Delete an userStatusOverview object.|
|[Update userStatusOverview](../api/devicecompliancepolicy-update-userstatusoverview.md)|[deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md)|Update the properties of an userStatusOverview object.|
|[Get deviceComplianceUserOverview](../api/devicecomplianceuseroverview-get.md)|[deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md)|Read properties and relationships of a [deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/devicecompliancepolicy-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Create deviceSettingStateSummaries](../api/devicecompliancepolicy-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Create a new deviceSettingStateSummaries object.|
|[Delete deviceSettingStateSummaries](../api/devicecompliancepolicy-delete-devicesettingstatesummaries.md)|None|Delete a deviceSettingStateSummaries object.|
|[Update deviceSettingStateSummaries](../api/devicecompliancepolicy-update-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Update the properties of a deviceSettingStateSummaries object.|
|[Get settingStateDeviceSummary](../api/settingstatedevicesummary-get.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Read properties and relationships of a [settingStateDeviceSummary](../resources/settingstatedevicesummary.md) object.|
|[List assignments](../api/devicecompliancepolicy-list-assignments.md)|[deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md) collection|Get the deviceCompliancePolicyAssignments from the assignments navigation property.|
|[Create assignments](../api/devicecompliancepolicy-post-assignments.md)|[deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/devicecompliancepolicy-delete-assignments.md)|None|Delete an assignments object.|
|[Update assignments](../api/devicecompliancepolicy-update-assignments.md)|[deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md)|Update the properties of an assignments object.|
|[Get deviceCompliancePolicyAssignment](../api/devicecompliancepolicyassignment-get.md)|[deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md)|Read properties and relationships of a [deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md) object.|

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
|assignments|[deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md) collection|The collection of assignments for this compliance policy.|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Compliance Setting State Device Summary|
|deviceStatuses|[deviceComplianceDeviceStatus](../resources/devicecompliancedevicestatus.md) collection|List of DeviceComplianceDeviceStatus.|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md)|Device compliance devices status overview|
|scheduledActionsForRule|[deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md) collection|The list of scheduled action for this rule|
|userStatuses|[deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md) collection|List of DeviceComplianceUserStatus.|
|userStatusOverview|[deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md)|Device compliance users status overview|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```

