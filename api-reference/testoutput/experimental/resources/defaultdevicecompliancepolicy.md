---
title: "defaultDeviceCompliancePolicy resource type"
description: "Default device compliance policy rules that are enforced account wide."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# defaultDeviceCompliancePolicy resource type

Default device compliance policy rules that are enforced account wide.


Inherits from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List defaultDeviceCompliancePolicies](../api/defaultdevicecompliancepolicy-list.md)|[defaultDeviceCompliancePolicy](../resources/defaultDeviceCompliancePolicy.md) collection|List properties and relationships of the [defaultDeviceCompliancePolicy](../resources/defaultdevicecompliancepolicy.md) objects.|
|[Get defaultDeviceCompliancePolicy](../api/defaultdevicecompliancepolicy-get.md)|[defaultDeviceCompliancePolicy](../resources/defaultDeviceCompliancePolicy.md)|Read properties and relationships of the [defaultDeviceCompliancePolicy](../resources/defaultdevicecompliancepolicy.md) object.|
|[Create defaultDeviceCompliancePolicy](../api/defaultdevicecompliancepolicy-create.md)|[defaultDeviceCompliancePolicy](../resources/defaultDeviceCompliancePolicy.md)|Create a new [defaultDeviceCompliancePolicy](../resources/defaultdevicecompliancepolicy.md) object.|
|[Delete defaultDeviceCompliancePolicy](../api/defaultdevicecompliancepolicy-delete.md)|None|Deletes a [defaultDeviceCompliancePolicy](../resources/defaultdevicecompliancepolicy.md).|
|[Update defaultDeviceCompliancePolicy](../api/defaultdevicecompliancepolicy-update.md)|[defaultDeviceCompliancePolicy](../resources/defaultDeviceCompliancePolicy.md)|Update the properties of a [defaultDeviceCompliancePolicy](../resources/defaultdevicecompliancepolicy.md) object.|
|[assign](../api/defaultdevicecompliancepolicy-assign.md)|[deviceCompliancePolicyAssignment](../resources/deviceCompliancePolicyAssignment.md) collection||
|[scheduleActionsForRules](../api/defaultdevicecompliancepolicy-scheduleactionsforrules.md)|None||
|[List scheduledActionsForRule](../api/defaultdevicecompliancepolicy-list-scheduledactionsforrule.md)|[deviceComplianceScheduledActionForRule](../resources/deviceComplianceScheduledActionForRule.md) collection|Get the deviceComplianceScheduledActionForRules from the scheduledActionsForRule navigation property.|
|[Add scheduledActionsForRule](../api/defaultdevicecompliancepolicy-post-scheduledactionsforrule.md)|[deviceComplianceScheduledActionForRule](../resources/deviceComplianceScheduledActionForRule.md)|Add scheduledActionsForRule by posting to the scheduledActionsForRule collection.|
|[List deviceStatuses](../api/defaultdevicecompliancepolicy-list-devicestatuses.md)|[deviceComplianceDeviceStatus](../resources/deviceComplianceDeviceStatus.md) collection|Get the deviceComplianceDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/defaultdevicecompliancepolicy-post-devicestatuses.md)|[deviceComplianceDeviceStatus](../resources/deviceComplianceDeviceStatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/defaultdevicecompliancepolicy-list-userstatuses.md)|[deviceComplianceUserStatus](../resources/deviceComplianceUserStatus.md) collection|Get the deviceComplianceUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/defaultdevicecompliancepolicy-post-userstatuses.md)|[deviceComplianceUserStatus](../resources/deviceComplianceUserStatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceComplianceDeviceOverview](../api/devicecompliancedeviceoverview-get.md)|[deviceComplianceDeviceOverview](../resources/deviceComplianceDeviceOverview.md)|Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md) object.|
|[Get deviceComplianceUserOverview](../api/devicecomplianceuseroverview-get.md)|[deviceComplianceUserOverview](../resources/deviceComplianceUserOverview.md)|Read properties and relationships of the [deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/defaultdevicecompliancepolicy-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/defaultdevicecompliancepolicy-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|
|[List assignments](../api/defaultdevicecompliancepolicy-list-assignments.md)|[deviceCompliancePolicyAssignment](../resources/deviceCompliancePolicyAssignment.md) collection|Get the deviceCompliancePolicyAssignments from the assignments navigation property.|
|[Add assignments](../api/defaultdevicecompliancepolicy-post-assignments.md)|[deviceCompliancePolicyAssignment](../resources/deviceCompliancePolicyAssignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|
|version|Int32|Version of the device configuration. Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceCompliancePolicyAssignment](../resources/deviceCompliancePolicyAssignment.md) collection|The collection of assignments for this compliance policy. Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md) collection|Compliance Setting State Device Summary Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|
|deviceStatuses|[deviceComplianceDeviceStatus](../resources/deviceComplianceDeviceStatus.md) collection|List of DeviceComplianceDeviceStatus. Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/deviceComplianceDeviceOverview.md)|Device compliance devices status overview Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|
|scheduledActionsForRule|[deviceComplianceScheduledActionForRule](../resources/deviceComplianceScheduledActionForRule.md) collection|The list of scheduled action for this rule Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|
|userStatuses|[deviceComplianceUserStatus](../resources/deviceComplianceUserStatus.md) collection|List of DeviceComplianceUserStatus. Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|
|userStatusOverview|[deviceComplianceUserOverview](../resources/deviceComplianceUserOverview.md)|Device compliance users status overview Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultDeviceCompliancePolicy",
  "baseType": "microsoft.graph.deviceCompliancePolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "id": "String (identifier)",
  "roleScopeTagIds": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```

