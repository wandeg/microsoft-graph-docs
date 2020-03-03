---
title: "androidForWorkEasEmailProfileBase resource type"
description: "Base for Android For Work EAS Email profiles"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# androidForWorkEasEmailProfileBase resource type

Base for Android For Work EAS Email profiles


Inherits from [deviceConfiguration](../resources/deviceConfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List androidForWorkEasEmailProfileBases](../api/androidforworkeasemailprofilebase-list.md)|[androidForWorkEasEmailProfileBase](../resources/androidForWorkEasEmailProfileBase.md) collection|List properties and relationships of the [androidForWorkEasEmailProfileBase](../resources/androidforworkeasemailprofilebase.md) objects.|
|[Get androidForWorkEasEmailProfileBase](../api/androidforworkeasemailprofilebase-get.md)|[androidForWorkEasEmailProfileBase](../resources/androidForWorkEasEmailProfileBase.md)|Read properties and relationships of the [androidForWorkEasEmailProfileBase](../resources/androidforworkeasemailprofilebase.md) object.|
|[assign](../api/androidforworkeasemailprofilebase-assign.md)|[deviceConfigurationAssignment](../resources/deviceConfigurationAssignment.md) collection||
|[windowsPrivacyAccessControls](../api/androidforworkeasemailprofilebase-windowsprivacyaccesscontrols.md)|None||
|[assignedAccessMultiModeProfiles](../api/androidforworkeasemailprofilebase-assignedaccessmultimodeprofiles.md)|None||
|[List groupAssignments](../api/androidforworkeasemailprofilebase-list-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceConfigurationGroupAssignment.md) collection|Get the deviceConfigurationGroupAssignments from the groupAssignments navigation property.|
|[Add groupAssignments](../api/androidforworkeasemailprofilebase-post-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceConfigurationGroupAssignment.md)|Add groupAssignments by posting to the groupAssignments collection.|
|[List assignments](../api/androidforworkeasemailprofilebase-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceConfigurationAssignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/androidforworkeasemailprofilebase-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceConfigurationAssignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/androidforworkeasemailprofilebase-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceConfigurationDeviceStatus.md) collection|Get the deviceConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/androidforworkeasemailprofilebase-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceConfigurationDeviceStatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/androidforworkeasemailprofilebase-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceConfigurationUserStatus.md) collection|Get the deviceConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/androidforworkeasemailprofilebase-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceConfigurationUserStatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceConfigurationDeviceOverview.md)|Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[Get deviceConfigurationUserOverview](../api/deviceconfigurationuseroverview-get.md)|[deviceConfigurationUserOverview](../resources/deviceConfigurationUserOverview.md)|Read properties and relationships of the [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/androidforworkeasemailprofilebase-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/androidforworkeasemailprofilebase-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|
|[Get androidForWorkCertificateProfileBase](../api/androidforworkcertificateprofilebase-get.md)|[androidForWorkCertificateProfileBase](../resources/androidForWorkCertificateProfileBase.md)|Read properties and relationships of the [androidForWorkCertificateProfileBase](../resources/androidforworkcertificateprofilebase.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|authenticationMethod|Enumeration|Authentication method for Exchange ActiveSync. Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/deviceManagementApplicabilityRuleDeviceMode.md)|The device mode applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/deviceManagementApplicabilityRuleOsEdition.md)|The OS edition applicability for this Policy. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/deviceManagementApplicabilityRuleOsVersion.md)|The OS version applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|durationOfEmailToSync|Enumeration|Duration of time email should be synced to. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.|
|emailAddressSource|Enumeration|Email attribute that is picked from AAD and injected into this profile before installing on the device. Possible values are: `userPrincipalName`, `primarySmtpAddress`.|
|hostName|String|Exchange location (URL) that the mail app connects to.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|requireSsl|Boolean|Indicates whether or not to use SSL.|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|supportsScopeTags|Boolean|Indicates whether or not the underlying Device Configuration supports the assignment of scope tags. Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users. This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal. This property is read-only. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|usernameSource|Enumeration|Username attribute that is picked from AAD and injected into this profile before installing on the device. Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/deviceConfigurationAssignment.md) collection|The list of assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md) collection|Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/deviceConfigurationDeviceStatus.md) collection|Device configuration installation status by device. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/deviceConfigurationDeviceOverview.md)|Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/deviceConfigurationGroupAssignment.md) collection|The list of group assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|identityCertificate|[androidForWorkCertificateProfileBase](../resources/androidForWorkCertificateProfileBase.md)|Identity certificate.|
|userStatuses|[deviceConfigurationUserStatus](../resources/deviceConfigurationUserStatus.md) collection|Device configuration installation status by user. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/deviceConfigurationUserOverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkEasEmailProfileBase",
  "baseType": "microsoft.graph.deviceConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkEasEmailProfileBase",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "authenticationMethod": "String",
  "durationOfEmailToSync": "String",
  "emailAddressSource": "String",
  "hostName": "String",
  "requireSsl": true,
  "usernameSource": "String"
}
```

