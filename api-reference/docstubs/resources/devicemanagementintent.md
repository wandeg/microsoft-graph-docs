---
title: "deviceManagementIntent resource type"
description: "Entity that represents an intent to apply settings to a device"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementIntent resource type


Namespace: microsoft.graph

Entity that represents an intent to apply settings to a device


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementIntent](../api/devicemanagementintent-get.md)|[deviceManagementIntent](../resources/devicemanagementintent.md)|Read the properties and relationships of a [deviceManagementIntent](../resources/devicemanagementintent.md) object.|
|[Update deviceManagementIntent](../api/devicemanagementintent-update.md)|[deviceManagementIntent](../resources/devicemanagementintent.md)|Update the properties of a [deviceManagementIntent](../resources/devicemanagementintent.md) object.|
|[updateSettings](../api/devicemanagementintent-updatesettings.md)|None|**TODO: Add Description**|
|[migrateToTemplate](../api/devicemanagementintent-migratetotemplate.md)|None|**TODO: Add Description**|
|[assign](../api/devicemanagementintent-assign.md)|None|**TODO: Add Description**|
|[compare](../api/devicemanagementintent-compare.md)|[deviceManagementSettingComparison](../resources/devicemanagementsettingcomparison.md) collection|**TODO: Add Description**|
|[List settings](../api/devicemanagementintent-list-settings.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) collection|Get the deviceManagementSettingInstances from the settings navigation property.|
|[Create settings](../api/devicemanagementintent-post-settings.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)|Create a new settings object.|
|[Delete settings](../api/devicemanagementintent-delete-settings.md)|None|Delete a [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) object.|
|[Update settings](../api/devicemanagementintent-update-settings.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)|Update the properties of a settings object.|
|[Get deviceManagementSettingInstance](../api/devicemanagementsettinginstance-get.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)|Read the properties and relationships of a [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) object.|
|[List categories](../api/devicemanagementintent-list-categories.md)|[deviceManagementIntentSettingCategory](../resources/devicemanagementintentsettingcategory.md) collection|Get the deviceManagementIntentSettingCategories from the categories navigation property.|
|[Create categories](../api/devicemanagementintent-post-categories.md)|[deviceManagementIntentSettingCategory](../resources/devicemanagementintentsettingcategory.md)|Create a new categories object.|
|[Delete categories](../api/devicemanagementintent-delete-categories.md)|None|Delete a [deviceManagementIntentSettingCategory](../resources/devicemanagementintentsettingcategory.md) object.|
|[Update categories](../api/devicemanagementintent-update-categories.md)|[deviceManagementIntentSettingCategory](../resources/devicemanagementintentsettingcategory.md)|Update the properties of a categories object.|
|[Get deviceManagementIntentSettingCategory](../api/devicemanagementintentsettingcategory-get.md)|[deviceManagementIntentSettingCategory](../resources/devicemanagementintentsettingcategory.md)|Read the properties and relationships of a [deviceManagementIntentSettingCategory](../resources/devicemanagementintentsettingcategory.md) object.|
|[List assignments](../api/devicemanagementintent-list-assignments.md)|[deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md) collection|Get the deviceManagementIntentAssignments from the assignments navigation property.|
|[Create assignments](../api/devicemanagementintent-post-assignments.md)|[deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/devicemanagementintent-delete-assignments.md)|None|Delete an [deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md) object.|
|[Update assignments](../api/devicemanagementintent-update-assignments.md)|[deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md)|Update the properties of an assignments object.|
|[Get deviceManagementIntentAssignment](../api/devicemanagementintentassignment-get.md)|[deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md)|Read the properties and relationships of a [deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md) object.|
|[List deviceSettingStateSummaries](../api/devicemanagementintent-list-devicesettingstatesummaries.md)|[deviceManagementIntentDeviceSettingStateSummary](../resources/devicemanagementintentdevicesettingstatesummary.md) collection|Get the deviceManagementIntentDeviceSettingStateSummaries from the deviceSettingStateSummaries navigation property.|
|[Create deviceSettingStateSummaries](../api/devicemanagementintent-post-devicesettingstatesummaries.md)|[deviceManagementIntentDeviceSettingStateSummary](../resources/devicemanagementintentdevicesettingstatesummary.md)|Create a new deviceSettingStateSummaries object.|
|[Delete deviceSettingStateSummaries](../api/devicemanagementintent-delete-devicesettingstatesummaries.md)|None|Delete a [deviceManagementIntentDeviceSettingStateSummary](../resources/devicemanagementintentdevicesettingstatesummary.md) object.|
|[Update deviceSettingStateSummaries](../api/devicemanagementintent-update-devicesettingstatesummaries.md)|[deviceManagementIntentDeviceSettingStateSummary](../resources/devicemanagementintentdevicesettingstatesummary.md)|Update the properties of a deviceSettingStateSummaries object.|
|[Get deviceManagementIntentDeviceSettingStateSummary](../api/devicemanagementintentdevicesettingstatesummary-get.md)|[deviceManagementIntentDeviceSettingStateSummary](../resources/devicemanagementintentdevicesettingstatesummary.md)|Read the properties and relationships of a [deviceManagementIntentDeviceSettingStateSummary](../resources/devicemanagementintentdevicesettingstatesummary.md) object.|
|[List deviceStates](../api/devicemanagementintent-list-devicestates.md)|[deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md) collection|Get the deviceManagementIntentDeviceStates from the deviceStates navigation property.|
|[Create deviceStates](../api/devicemanagementintent-post-devicestates.md)|[deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md)|Create a new deviceStates object.|
|[Delete deviceStates](../api/devicemanagementintent-delete-devicestates.md)|None|Delete a [deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md) object.|
|[Update deviceStates](../api/devicemanagementintent-update-devicestates.md)|[deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md)|Update the properties of a deviceStates object.|
|[Get deviceManagementIntentDeviceState](../api/devicemanagementintentdevicestate-get.md)|[deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md)|Read the properties and relationships of a [deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md) object.|
|[List userStates](../api/devicemanagementintent-list-userstates.md)|[deviceManagementIntentUserState](../resources/devicemanagementintentuserstate.md) collection|Get the deviceManagementIntentUserStates from the userStates navigation property.|
|[Create userStates](../api/devicemanagementintent-post-userstates.md)|[deviceManagementIntentUserState](../resources/devicemanagementintentuserstate.md)|Create a new userStates object.|
|[Delete userStates](../api/devicemanagementintent-delete-userstates.md)|None|Delete a [deviceManagementIntentUserState](../resources/devicemanagementintentuserstate.md) object.|
|[Update userStates](../api/devicemanagementintent-update-userstates.md)|[deviceManagementIntentUserState](../resources/devicemanagementintentuserstate.md)|Update the properties of a userStates object.|
|[Get deviceManagementIntentUserState](../api/devicemanagementintentuserstate-get.md)|[deviceManagementIntentUserState](../resources/devicemanagementintentuserstate.md)|Read the properties and relationships of a [deviceManagementIntentUserState](../resources/devicemanagementintentuserstate.md) object.|
|[List deviceStateSummary](../api/devicemanagementintent-list-devicestatesummary.md)|[deviceManagementIntentDeviceStateSummary](../resources/devicemanagementintentdevicestatesummary.md) collection|Get the deviceManagementIntentDeviceStateSummaries from the deviceStateSummary navigation property.|
|[Create deviceStateSummary](../api/devicemanagementintent-post-devicestatesummary.md)|[deviceManagementIntentDeviceStateSummary](../resources/devicemanagementintentdevicestatesummary.md)|Create a new deviceStateSummary object.|
|[Delete deviceStateSummary](../api/devicemanagementintent-delete-devicestatesummary.md)|None|Delete a [deviceManagementIntentDeviceStateSummary](../resources/devicemanagementintentdevicestatesummary.md) object.|
|[Update deviceStateSummary](../api/devicemanagementintent-update-devicestatesummary.md)|[deviceManagementIntentDeviceStateSummary](../resources/devicemanagementintentdevicestatesummary.md)|Update the properties of a deviceStateSummary object.|
|[Get deviceManagementIntentDeviceStateSummary](../api/devicemanagementintentdevicestatesummary-get.md)|[deviceManagementIntentDeviceStateSummary](../resources/devicemanagementintentdevicestatesummary.md)|Read the properties and relationships of a [deviceManagementIntentDeviceStateSummary](../resources/devicemanagementintentdevicestatesummary.md) object.|
|[List userStateSummary](../api/devicemanagementintent-list-userstatesummary.md)|[deviceManagementIntentUserStateSummary](../resources/devicemanagementintentuserstatesummary.md) collection|Get the deviceManagementIntentUserStateSummaries from the userStateSummary navigation property.|
|[Create userStateSummary](../api/devicemanagementintent-post-userstatesummary.md)|[deviceManagementIntentUserStateSummary](../resources/devicemanagementintentuserstatesummary.md)|Create a new userStateSummary object.|
|[Delete userStateSummary](../api/devicemanagementintent-delete-userstatesummary.md)|None|Delete a [deviceManagementIntentUserStateSummary](../resources/devicemanagementintentuserstatesummary.md) object.|
|[Update userStateSummary](../api/devicemanagementintent-update-userstatesummary.md)|[deviceManagementIntentUserStateSummary](../resources/devicemanagementintentuserstatesummary.md)|Update the properties of a userStateSummary object.|
|[Get deviceManagementIntentUserStateSummary](../api/devicemanagementintentuserstatesummary-get.md)|[deviceManagementIntentUserStateSummary](../resources/devicemanagementintentuserstatesummary.md)|Read the properties and relationships of a [deviceManagementIntentUserStateSummary](../resources/devicemanagementintentuserstatesummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|The user given description|
|displayName|String|The user given display name|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isAssigned|Boolean|Signifies whether or not the intent is assigned to users|
|lastModifiedDateTime|DateTimeOffset|When the intent was last modified|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance.|
|templateId|String|The ID of the template this intent was created from (if any)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md) collection|Collection of assignments|
|categories|[deviceManagementIntentSettingCategory](../resources/devicemanagementintentsettingcategory.md) collection|Collection of setting categories within the intent|
|deviceSettingStateSummaries|[deviceManagementIntentDeviceSettingStateSummary](../resources/devicemanagementintentdevicesettingstatesummary.md) collection|Collection of settings and their states and counts of devices that belong to corresponding state for all settings within the intent|
|deviceStates|[deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md) collection|Collection of states of all devices that the intent is applied to|
|deviceStateSummary|[deviceManagementIntentDeviceStateSummary](../resources/devicemanagementintentdevicestatesummary.md)|A summary of device states and counts of devices that belong to corresponding state for all devices that the intent is applied to|
|settings|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) collection|Collection of all settings to be applied|
|userStates|[deviceManagementIntentUserState](../resources/devicemanagementintentuserstate.md) collection|Collection of states of all users that the intent is applied to|
|userStateSummary|[deviceManagementIntentUserStateSummary](../resources/devicemanagementintentuserstatesummary.md)|A summary of user states and counts of users that belong to corresponding state for all users that the intent is applied to|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isAssigned": true,
  "lastModifiedDateTime": "String (timestamp)",
  "templateId": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```

