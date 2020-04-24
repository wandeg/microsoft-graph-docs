---
title: "deviceConfiguration resource type"
description: "Device Configuration."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceConfiguration resource type


Namespace: microsoft.graph

Device Configuration.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceConfiguration](../api/deviceconfiguration-get.md)|[deviceConfiguration](../resources/deviceconfiguration.md)|Read the properties and relationships of a [deviceConfiguration](../resources/deviceconfiguration.md) object.|
|[hasPayloadLinks](../api/deviceconfiguration-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/haspayloadlinkresultitem.md) collection|**TODO: Add Description**|
|[getTargetedUsersAndDevices](../api/deviceconfiguration-gettargetedusersanddevices.md)|[deviceConfigurationTargetedUserAndDevice](../resources/deviceconfigurationtargeteduseranddevice.md) collection|**TODO: Add Description**|
|[getIosAvailableUpdateVersions](../api/deviceconfiguration-getiosavailableupdateversions.md)|[iosAvailableUpdateVersion](../resources/iosavailableupdateversion.md) collection|**TODO: Add Description**|
|[assign](../api/deviceconfiguration-assign.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|**TODO: Add Description**|
|[windowsPrivacyAccessControls](../api/deviceconfiguration-windowsprivacyaccesscontrols.md)|None|**TODO: Add Description**|
|[assignedAccessMultiModeProfiles](../api/deviceconfiguration-assignedaccessmultimodeprofiles.md)|None|**TODO: Add Description**|
|[List groupAssignments](../api/deviceconfiguration-list-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) collection|Get the deviceConfigurationGroupAssignments from the groupAssignments navigation property.|
|[Create groupAssignments](../api/deviceconfiguration-post-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md)|Create a new groupAssignments object.|
|[Delete groupAssignments](../api/deviceconfiguration-delete-groupassignments.md)|None|Delete a [deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) object.|
|[Update groupAssignments](../api/deviceconfiguration-update-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md)|Update the properties of a groupAssignments object.|
|[Get deviceConfigurationGroupAssignment](../api/deviceconfigurationgroupassignment-get.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md)|Read the properties and relationships of a [deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) object.|
|[List assignments](../api/deviceconfiguration-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Create assignments](../api/deviceconfiguration-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/deviceconfiguration-delete-assignments.md)|None|Delete an [deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) object.|
|[Update assignments](../api/deviceconfiguration-update-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Update the properties of an assignments object.|
|[Get deviceConfigurationAssignment](../api/deviceconfigurationassignment-get.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Read the properties and relationships of a [deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) object.|
|[List deviceStatuses](../api/deviceconfiguration-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Get the deviceConfigurationDeviceStatus from the deviceStatuses navigation property.|
|[Create deviceStatuses](../api/deviceconfiguration-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Create a new deviceStatuses object.|
|[Delete deviceStatuses](../api/deviceconfiguration-delete-devicestatuses.md)|None|Delete a [deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) object.|
|[Update deviceStatuses](../api/deviceconfiguration-update-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Update the properties of a deviceStatuses object.|
|[Get deviceConfigurationDeviceStatus](../api/deviceconfigurationdevicestatus-get.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Read the properties and relationships of a [deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) object.|
|[List userStatuses](../api/deviceconfiguration-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Get the deviceConfigurationUserStatus from the userStatuses navigation property.|
|[Create userStatuses](../api/deviceconfiguration-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Create a new userStatuses object.|
|[Delete userStatuses](../api/deviceconfiguration-delete-userstatuses.md)|None|Delete a [deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) object.|
|[Update userStatuses](../api/deviceconfiguration-update-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Update the properties of a userStatuses object.|
|[Get deviceConfigurationUserStatus](../api/deviceconfigurationuserstatus-get.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Read the properties and relationships of a [deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) object.|
|[List deviceStatusOverview](../api/deviceconfiguration-list-devicestatusoverview.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) collection|Get the deviceConfigurationDeviceOverviews from the deviceStatusOverview navigation property.|
|[Create deviceStatusOverview](../api/deviceconfiguration-post-devicestatusoverview.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Create a new deviceStatusOverview object.|
|[Delete deviceStatusOverview](../api/deviceconfiguration-delete-devicestatusoverview.md)|None|Delete a [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[Update deviceStatusOverview](../api/deviceconfiguration-update-devicestatusoverview.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Update the properties of a deviceStatusOverview object.|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Read the properties and relationships of a [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[List userStatusOverview](../api/deviceconfiguration-list-userstatusoverview.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) collection|Get the deviceConfigurationUserOverviews from the userStatusOverview navigation property.|
|[Create userStatusOverview](../api/deviceconfiguration-post-userstatusoverview.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Create a new userStatusOverview object.|
|[Delete userStatusOverview](../api/deviceconfiguration-delete-userstatusoverview.md)|None|Delete a [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[Update userStatusOverview](../api/deviceconfiguration-update-userstatusoverview.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Update the properties of a userStatusOverview object.|
|[Get deviceConfigurationUserOverview](../api/deviceconfigurationuseroverview-get.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Read the properties and relationships of a [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/deviceconfiguration-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Create deviceSettingStateSummaries](../api/deviceconfiguration-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Create a new deviceSettingStateSummaries object.|
|[Delete deviceSettingStateSummaries](../api/deviceconfiguration-delete-devicesettingstatesummaries.md)|None|Delete a [settingStateDeviceSummary](../resources/settingstatedevicesummary.md) object.|
|[Update deviceSettingStateSummaries](../api/deviceconfiguration-update-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Update the properties of a deviceSettingStateSummaries object.|
|[Get settingStateDeviceSummary](../api/settingstatedevicesummary-get.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Read the properties and relationships of a [settingStateDeviceSummary](../resources/settingstatedevicesummary.md) object.|
|[List deviceConfiguration](../api/deviceconfigurationgroupassignment-list-deviceconfiguration.md)|[deviceConfiguration](../resources/deviceconfiguration.md) collection|Get the deviceConfigurations from the deviceConfiguration navigation property.|
|[Add deviceConfiguration](../api/deviceconfigurationgroupassignment-post-deviceconfiguration.md)|[deviceConfiguration](../resources/deviceconfiguration.md)|Add deviceConfiguration by posting to the deviceConfiguration collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|DateTime the object was created.|
|description|String|Admin provided description of the Device Configuration.|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/devicemanagementapplicabilityruledevicemode.md)|The device mode applicability rule for this Policy.|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/devicemanagementapplicabilityruleosedition.md)|The OS edition applicability for this Policy.|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/devicemanagementapplicabilityruleosversion.md)|The OS version applicability rule for this Policy.|
|displayName|String|Admin provided name of the device configuration.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance.|
|supportsScopeTags|Boolean|Indicates whether or not the underlying Device Configuration supports the assignment of scope tags. Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users. This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal. This property is read-only.|
|version|Int32|Version of the device configuration.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|The list of assignments for the device configuration profile.|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Device Configuration Setting State Device Summary|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Device configuration installation status by device.|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Device Configuration devices status overview|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) collection|The list of group assignments for the device configuration profile.|
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
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024
}
```

