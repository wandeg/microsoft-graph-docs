---
title: "macOSCompliancePolicy resource type"
description: "This class contains compliance settings for Mac OS."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# macOSCompliancePolicy resource type

This class contains compliance settings for Mac OS.


Inherits from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List macOSCompliancePolicies](../api/macoscompliancepolicy-list.md)|[macOSCompliancePolicy](../resources/macOSCompliancePolicy.md) collection|List properties and relationships of the [macOSCompliancePolicy](../resources/macoscompliancepolicy.md) objects.|
|[Get macOSCompliancePolicy](../api/macoscompliancepolicy-get.md)|[macOSCompliancePolicy](../resources/macOSCompliancePolicy.md)|Read properties and relationships of the [macOSCompliancePolicy](../resources/macoscompliancepolicy.md) object.|
|[Create macOSCompliancePolicy](../api/macoscompliancepolicy-create.md)|[macOSCompliancePolicy](../resources/macOSCompliancePolicy.md)|Create a new [macOSCompliancePolicy](../resources/macoscompliancepolicy.md) object.|
|[Delete macOSCompliancePolicy](../api/macoscompliancepolicy-delete.md)|None|Deletes a [macOSCompliancePolicy](../resources/macoscompliancepolicy.md).|
|[Update macOSCompliancePolicy](../api/macoscompliancepolicy-update.md)|[macOSCompliancePolicy](../resources/macOSCompliancePolicy.md)|Update the properties of a [macOSCompliancePolicy](../resources/macoscompliancepolicy.md) object.|
|[assign](../api/macoscompliancepolicy-assign.md)|[deviceCompliancePolicyAssignment](../resources/deviceCompliancePolicyAssignment.md) collection||
|[scheduleActionsForRules](../api/macoscompliancepolicy-scheduleactionsforrules.md)|None||
|[List scheduledActionsForRule](../api/macoscompliancepolicy-list-scheduledactionsforrule.md)|[deviceComplianceScheduledActionForRule](../resources/deviceComplianceScheduledActionForRule.md) collection|Get the deviceComplianceScheduledActionForRules from the scheduledActionsForRule navigation property.|
|[Add scheduledActionsForRule](../api/macoscompliancepolicy-post-scheduledactionsforrule.md)|[deviceComplianceScheduledActionForRule](../resources/deviceComplianceScheduledActionForRule.md)|Add scheduledActionsForRule by posting to the scheduledActionsForRule collection.|
|[List deviceStatuses](../api/macoscompliancepolicy-list-devicestatuses.md)|[deviceComplianceDeviceStatus](../resources/deviceComplianceDeviceStatus.md) collection|Get the deviceComplianceDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/macoscompliancepolicy-post-devicestatuses.md)|[deviceComplianceDeviceStatus](../resources/deviceComplianceDeviceStatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/macoscompliancepolicy-list-userstatuses.md)|[deviceComplianceUserStatus](../resources/deviceComplianceUserStatus.md) collection|Get the deviceComplianceUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/macoscompliancepolicy-post-userstatuses.md)|[deviceComplianceUserStatus](../resources/deviceComplianceUserStatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceComplianceDeviceOverview](../api/devicecompliancedeviceoverview-get.md)|[deviceComplianceDeviceOverview](../resources/deviceComplianceDeviceOverview.md)|Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md) object.|
|[Get deviceComplianceUserOverview](../api/devicecomplianceuseroverview-get.md)|[deviceComplianceUserOverview](../resources/deviceComplianceUserOverview.md)|Read properties and relationships of the [deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/macoscompliancepolicy-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/macoscompliancepolicy-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|
|[List assignments](../api/macoscompliancepolicy-list-assignments.md)|[deviceCompliancePolicyAssignment](../resources/deviceCompliancePolicyAssignment.md) collection|Get the deviceCompliancePolicyAssignments from the assignments navigation property.|
|[Add assignments](../api/macoscompliancepolicy-post-assignments.md)|[deviceCompliancePolicyAssignment](../resources/deviceCompliancePolicyAssignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|
|deviceThreatProtectionEnabled|Boolean|Require that devices have enabled device threat protection.|
|deviceThreatProtectionRequiredSecurityLevel|Enumeration|Require Mobile Threat Protection minimum risk level to report noncompliance. Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|
|firewallBlockAllIncoming|Boolean|Corresponds to the “Block all incoming connections” option.|
|firewallEnabled|Boolean|Whether the firewall should be enabled or not.|
|firewallEnableStealthMode|Boolean|Corresponds to “Enable stealth mode.”|
|gatekeeperAllowedAppSource|Enumeration|System and Privacy setting that determines which download locations apps can be run from on a macOS device. Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|
|osMaximumBuildVersion|String|Maximum MacOS build version.|
|osMaximumVersion|String|Maximum MacOS version.|
|osMinimumBuildVersion|String|Minimum MacOS build version.|
|osMinimumVersion|String|Minimum MacOS version.|
|passwordBlockSimple|Boolean|Indicates whether or not to block simple passwords.|
|passwordExpirationDays|Int32|Number of days before the password expires. Valid values 1 to 65535|
|passwordMinimumCharacterSetCount|Int32|The number of character sets required in the password.|
|passwordMinimumLength|Int32|Minimum length of password. Valid values 4 to 14|
|passwordMinutesOfInactivityBeforeLock|Int32|Minutes of inactivity before a password is required.|
|passwordPreviousPasswordBlockCount|Int32|Number of previous passwords to block. Valid values 1 to 24|
|passwordRequired|Boolean|Whether or not to require a password.|
|passwordRequiredType|Enumeration|The required password type. Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [deviceCompliancePolicy](../resources/deviceCompliancePolicy.md)|
|storageRequireEncryption|Boolean|Require encryption on Mac OS devices.|
|systemIntegrityProtectionEnabled|Boolean|Require that devices have enabled system integrity protection.|
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
  "@odata.type": "microsoft.graph.macOSCompliancePolicy",
  "baseType": "microsoft.graph.deviceCompliancePolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "id": "String (identifier)",
  "roleScopeTagIds": [
    "String"
  ],
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
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordRequiredType": "String",
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "osMinimumBuildVersion": "String",
  "osMaximumBuildVersion": "String",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "String",
  "storageRequireEncryption": true,
  "gatekeeperAllowedAppSource": "String",
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```

