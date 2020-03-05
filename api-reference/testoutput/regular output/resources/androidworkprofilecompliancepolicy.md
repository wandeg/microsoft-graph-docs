---
title: "androidWorkProfileCompliancePolicy resource type"
description: "This class contains compliance settings for Android Work Profile."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# androidWorkProfileCompliancePolicy resource type


Namespace: microsoft.graph

This class contains compliance settings for Android Work Profile.


Inherits from [deviceCompliancePolicy](../resources/devicecompliancepolicy.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List androidWorkProfileCompliancePolicies](../api/androidworkprofilecompliancepolicy-list.md)|[androidWorkProfileCompliancePolicy](../resources/androidworkprofilecompliancepolicy.md) collection|List properties and relationships of the [androidWorkProfileCompliancePolicy](../resources/androidworkprofilecompliancepolicy.md) objects.|
|[Get androidWorkProfileCompliancePolicy](../api/androidworkprofilecompliancepolicy-get.md)|[androidWorkProfileCompliancePolicy](../resources/androidworkprofilecompliancepolicy.md)|Read properties and relationships of the [androidWorkProfileCompliancePolicy](../resources/androidworkprofilecompliancepolicy.md) object.|
|[Create androidWorkProfileCompliancePolicy](../api/androidworkprofilecompliancepolicy-create.md)|[androidWorkProfileCompliancePolicy](../resources/androidworkprofilecompliancepolicy.md)|Create a new [androidWorkProfileCompliancePolicy](../resources/androidworkprofilecompliancepolicy.md) object.|
|[Delete androidWorkProfileCompliancePolicy](../api/androidworkprofilecompliancepolicy-delete.md)|None|Deletes a [androidWorkProfileCompliancePolicy](../resources/androidworkprofilecompliancepolicy.md).|
|[Update androidWorkProfileCompliancePolicy](../api/androidworkprofilecompliancepolicy-update.md)|[androidWorkProfileCompliancePolicy](../resources/androidworkprofilecompliancepolicy.md)|Update the properties of a [androidWorkProfileCompliancePolicy](../resources/androidworkprofilecompliancepolicy.md) object.|
|[assign](../api/androidworkprofilecompliancepolicy-assign.md)|[deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md) collection||
|[scheduleActionsForRules](../api/androidworkprofilecompliancepolicy-scheduleactionsforrules.md)|None||
|[List scheduledActionsForRule](../api/androidworkprofilecompliancepolicy-list-scheduledactionsforrule.md)|[deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md) collection|Get the deviceComplianceScheduledActionForRules from the scheduledActionsForRule navigation property.|
|[Add scheduledActionsForRule](../api/androidworkprofilecompliancepolicy-post-scheduledactionsforrule.md)|[deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md)|Add scheduledActionsForRule by posting to the scheduledActionsForRule collection.|
|[List deviceStatuses](../api/androidworkprofilecompliancepolicy-list-devicestatuses.md)|[deviceComplianceDeviceStatus](../resources/devicecompliancedevicestatus.md) collection|Get the deviceComplianceDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/androidworkprofilecompliancepolicy-post-devicestatuses.md)|[deviceComplianceDeviceStatus](../resources/devicecompliancedevicestatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/androidworkprofilecompliancepolicy-list-userstatuses.md)|[deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md) collection|Get the deviceComplianceUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/androidworkprofilecompliancepolicy-post-userstatuses.md)|[deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceComplianceDeviceOverview](../api/devicecompliancedeviceoverview-get.md)|[deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md)|Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md) object.|
|[Get deviceComplianceUserOverview](../api/devicecomplianceuseroverview-get.md)|[deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md)|Read properties and relationships of the [deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/androidworkprofilecompliancepolicy-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/androidworkprofilecompliancepolicy-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|
|[List assignments](../api/androidworkprofilecompliancepolicy-list-assignments.md)|[deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md) collection|Get the deviceCompliancePolicyAssignments from the assignments navigation property.|
|[Add assignments](../api/androidworkprofilecompliancepolicy-post-assignments.md)|[deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|
|deviceThreatProtectionEnabled|Boolean|Require that devices have enabled device threat protection.|
|deviceThreatProtectionRequiredSecurityLevel|Enumeration|Require Mobile Threat Protection minimum risk level to report noncompliance. Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|
|minAndroidSecurityPatchLevel|String|Minimum Android security patch level.|
|osMaximumVersion|String|Maximum Android version.|
|osMinimumVersion|String|Minimum Android version.|
|passwordExpirationDays|Int32|Number of days before the password expires. Valid values 1 to 365|
|passwordMinimumLength|Int32|Minimum password length. Valid values 4 to 16|
|passwordMinutesOfInactivityBeforeLock|Int32|Minutes of inactivity before a password is required.|
|passwordPreviousPasswordBlockCount|Int32|Number of previous passwords to block. Valid values 1 to 24|
|passwordRequired|Boolean|Require a password to unlock device.|
|passwordRequiredType|Enumeration|Type of characters in password. Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.|
|securityBlockJailbrokenDevices|Boolean|Devices must not be jailbroken or rooted.|
|securityDisableUsbDebugging|Boolean|Disable USB debugging on Android devices.|
|securityPreventInstallAppsFromUnknownSources|Boolean|Require that devices disallow installation of apps from unknown sources.|
|securityRequireCompanyPortalAppIntegrity|Boolean|Require the device to pass the Company Portal client app runtime integrity check.|
|securityRequireGooglePlayServices|Boolean|Require Google Play Services to be installed and enabled on the device.|
|securityRequireSafetyNetAttestationBasicIntegrity|Boolean|Require the device to pass the SafetyNet basic integrity check.|
|securityRequireSafetyNetAttestationCertifiedDevice|Boolean|Require the device to pass the SafetyNet certified device check.|
|securityRequireUpToDateSecurityProviders|Boolean|Require the device to have up to date security providers. The device will require Google Play Services to be enabled and up to date.|
|securityRequireVerifyApps|Boolean|Require the Android Verify apps feature is turned on.|
|storageRequireEncryption|Boolean|Require encryption on Android devices.|
|version|Int32|Version of the device configuration. Inherited from [deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md) collection|The collection of assignments for this compliance policy. Inherited from [deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Compliance Setting State Device Summary Inherited from [deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|
|deviceStatuses|[deviceComplianceDeviceStatus](../resources/devicecompliancedevicestatus.md) collection|List of DeviceComplianceDeviceStatus. Inherited from [deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md)|Device compliance devices status overview Inherited from [deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|
|scheduledActionsForRule|[deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md) collection|The list of scheduled action for this rule Inherited from [deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|
|userStatuses|[deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md) collection|List of DeviceComplianceUserStatus. Inherited from [deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|
|userStatusOverview|[deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md)|Device compliance users status overview Inherited from [deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidWorkProfileCompliancePolicy",
  "baseType": "microsoft.graph.deviceCompliancePolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordRequired": true,
  "passwordMinimumLength": 1024,
  "passwordRequiredType": "String",
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordExpirationDays": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "String",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "minAndroidSecurityPatchLevel": "String",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```

