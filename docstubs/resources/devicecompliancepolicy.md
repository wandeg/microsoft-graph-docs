---
title: "deviceCompliancePolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceCompliancePolicy resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceCompliancePolicy](../api/devicecompliancepolicy-get.md)|[deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|Read properties and relationships of the [deviceCompliancePolicy](../resources/devicecompliancepolicy.md) object.|
|[hasPayloadLinks](../api/devicecompliancepolicy-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/haspayloadlinkresultitem.md) collection||
|[getDevicesScheduledToRetire](../api/devicecompliancepolicy-getdevicesscheduledtoretire.md)|[retireScheduledManagedDevice](../resources/retirescheduledmanageddevice.md) collection||
|[setScheduledRetireState](../api/devicecompliancepolicy-setscheduledretirestate.md)|None||
|[refreshDeviceComplianceReportSummarization](../api/devicecompliancepolicy-refreshdevicecompliancereportsummarization.md)|None||
|[assign](../api/devicecompliancepolicy-assign.md)|[deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md) collection||
|[scheduleActionsForRules](../api/devicecompliancepolicy-scheduleactionsforrules.md)|None||
|[List scheduledActionsForRule](../api/devicecompliancepolicy-list-scheduledactionsforrule.md)|[deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md) collection|Get the deviceComplianceScheduledActionForRules from the scheduledActionsForRule navigation property.|
|[Add scheduledActionsForRule](../api/devicecompliancepolicy-post-scheduledactionsforrule.md)|[deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md)|Add scheduledActionsForRule by posting to the scheduledActionsForRule collection.|
|[List deviceStatuses](../api/devicecompliancepolicy-list-devicestatuses.md)|[deviceComplianceDeviceStatus](../resources/devicecompliancedevicestatus.md) collection|Get the deviceComplianceDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/devicecompliancepolicy-post-devicestatuses.md)|[deviceComplianceDeviceStatus](../resources/devicecompliancedevicestatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/devicecompliancepolicy-list-userstatuses.md)|[deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md) collection|Get the deviceComplianceUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/devicecompliancepolicy-post-userstatuses.md)|[deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceComplianceDeviceOverview](../api/devicecompliancedeviceoverview-get.md)|[deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md)|Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md) object.|
|[Get deviceComplianceUserOverview](../api/devicecomplianceuseroverview-get.md)|[deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md)|Read properties and relationships of the [deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/devicecompliancepolicy-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/devicecompliancepolicy-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|
|[List assignments](../api/devicecompliancepolicy-list-assignments.md)|[deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md) collection|Get the deviceCompliancePolicyAssignments from the assignments navigation property.|
|[Add assignments](../api/devicecompliancepolicy-post-assignments.md)|[deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset||
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|roleScopeTagIds|String collection||
|version|Int32||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md) collection||
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection||
|deviceStatuses|[deviceComplianceDeviceStatus](../resources/devicecompliancedevicestatus.md) collection||
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md)||
|scheduledActionsForRule|[deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md) collection||
|userStatuses|[deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md) collection||
|userStatusOverview|[deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md)||

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

