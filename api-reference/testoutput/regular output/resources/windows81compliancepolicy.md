---
title: "windows81CompliancePolicy resource type"
description: "This class contains compliance settings for Windows 8.1."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# windows81CompliancePolicy resource type

This class contains compliance settings for Windows 8.1.


Inherits from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windows81CompliancePolicies](../api/windows81compliancepolicy-list.md)|[windows81CompliancePolicy](../resources/windows81CompliancePolicy.md) collection|List properties and relationships of the [windows81CompliancePolicy](../resources/windows81compliancepolicy.md) objects.|
|[Get windows81CompliancePolicy](../api/windows81compliancepolicy-get.md)|[windows81CompliancePolicy](../resources/windows81CompliancePolicy.md)|Read properties and relationships of the [windows81CompliancePolicy](../resources/windows81compliancepolicy.md) object.|
|[Create windows81CompliancePolicy](../api/windows81compliancepolicy-create.md)|[windows81CompliancePolicy](../resources/windows81CompliancePolicy.md)|Create a new [windows81CompliancePolicy](../resources/windows81compliancepolicy.md) object.|
|[Delete windows81CompliancePolicy](../api/windows81compliancepolicy-delete.md)|None|Deletes a [windows81CompliancePolicy](../resources/windows81compliancepolicy.md).|
|[Update windows81CompliancePolicy](../api/windows81compliancepolicy-update.md)|[windows81CompliancePolicy](../resources/windows81CompliancePolicy.md)|Update the properties of a [windows81CompliancePolicy](../resources/windows81compliancepolicy.md) object.|
|[assign](../api/windows81compliancepolicy-assign.md)|[deviceCompliancePolicyAssignment](../resources/deviceCompliancePolicyAssignment.md) collection||
|[scheduleActionsForRules](../api/windows81compliancepolicy-scheduleactionsforrules.md)|None||
|[List scheduledActionsForRule](../api/windows81compliancepolicy-list-scheduledactionsforrule.md)|[deviceComplianceScheduledActionForRule](../resources/deviceComplianceScheduledActionForRule.md) collection|Get the deviceComplianceScheduledActionForRules from the scheduledActionsForRule navigation property.|
|[Add scheduledActionsForRule](../api/windows81compliancepolicy-post-scheduledactionsforrule.md)|[deviceComplianceScheduledActionForRule](../resources/deviceComplianceScheduledActionForRule.md)|Add scheduledActionsForRule by posting to the scheduledActionsForRule collection.|
|[List deviceStatuses](../api/windows81compliancepolicy-list-devicestatuses.md)|[deviceComplianceDeviceStatus](../resources/deviceComplianceDeviceStatus.md) collection|Get the deviceComplianceDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/windows81compliancepolicy-post-devicestatuses.md)|[deviceComplianceDeviceStatus](../resources/deviceComplianceDeviceStatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/windows81compliancepolicy-list-userstatuses.md)|[deviceComplianceUserStatus](../resources/deviceComplianceUserStatus.md) collection|Get the deviceComplianceUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/windows81compliancepolicy-post-userstatuses.md)|[deviceComplianceUserStatus](../resources/deviceComplianceUserStatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceComplianceDeviceOverview](../api/devicecompliancedeviceoverview-get.md)|[deviceComplianceDeviceOverview](../resources/deviceComplianceDeviceOverview.md)|Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md) object.|
|[Get deviceComplianceUserOverview](../api/devicecomplianceuseroverview-get.md)|[deviceComplianceUserOverview](../resources/deviceComplianceUserOverview.md)|Read properties and relationships of the [deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/windows81compliancepolicy-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/windows81compliancepolicy-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|
|[List assignments](../api/windows81compliancepolicy-list-assignments.md)|[deviceCompliancePolicyAssignment](../resources/deviceCompliancePolicyAssignment.md) collection|Get the deviceCompliancePolicyAssignments from the assignments navigation property.|
|[Add assignments](../api/windows81compliancepolicy-post-assignments.md)|[deviceCompliancePolicyAssignment](../resources/deviceCompliancePolicyAssignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|
|osMaximumVersion|String|Maximum Windows 8.1 version.|
|osMinimumVersion|String|Minimum Windows 8.1 version.|
|passwordBlockSimple|Boolean|Indicates whether or not to block simple password.|
|passwordExpirationDays|Int32|Password expiration in days.|
|passwordMinimumCharacterSetCount|Int32|The number of character sets required in the password.|
|passwordMinimumLength|Int32|The minimum password length.|
|passwordMinutesOfInactivityBeforeLock|Int32|Minutes of inactivity before a password is required.|
|passwordPreviousPasswordBlockCount|Int32|The number of previous passwords to prevent re-use of. Valid values 0 to 24|
|passwordRequired|Boolean|Require a password to unlock Windows device.|
|passwordRequiredType|Enumeration|The required password type. Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.|
|storageRequireEncryption|Boolean|Indicates whether or not to require encryption on a windows 8.1 device.|
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
  "@odata.type": "microsoft.graph.windows81CompliancePolicy",
  "baseType": "microsoft.graph.deviceCompliancePolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordRequiredType": "String",
  "passwordPreviousPasswordBlockCount": 1024,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "storageRequireEncryption": true
}
```

