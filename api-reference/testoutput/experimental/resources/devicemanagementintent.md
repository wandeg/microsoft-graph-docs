---
title: "deviceManagementIntent resource type"
description: "Entity that represents an intent to apply settings to a device"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceManagementIntent resource type

Entity that represents an intent to apply settings to a device


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementIntent](../api/devicemanagementintent-get.md)|[deviceManagementIntent](../resources/deviceManagementIntent.md)|Read properties and relationships of the [deviceManagementIntent](../resources/devicemanagementintent.md) object.|
|[Delete deviceManagementIntent](../api/devicemanagementintent-delete.md)|None|Deletes a [deviceManagementIntent](../resources/devicemanagementintent.md).|
|[Update deviceManagementIntent](../api/devicemanagementintent-update.md)|[deviceManagementIntent](../resources/deviceManagementIntent.md)|Update the properties of a [deviceManagementIntent](../resources/devicemanagementintent.md) object.|
|[updateSettings](../api/devicemanagementintent-updatesettings.md)|None||
|[migrateToTemplate](../api/devicemanagementintent-migratetotemplate.md)|None||
|[assign](../api/devicemanagementintent-assign.md)|None||
|[compare](../api/devicemanagementintent-compare.md)|[deviceManagementSettingComparison](../resources/deviceManagementSettingComparison.md) collection||
|[List settings](../api/devicemanagementintent-list-settings.md)|[deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md) collection|Get the deviceManagementSettingInstances from the settings navigation property.|
|[Add settings](../api/devicemanagementintent-post-settings.md)|[deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md)|Add settings by posting to the settings collection.|
|[List categories](../api/devicemanagementintent-list-categories.md)|[deviceManagementIntentSettingCategory](../resources/deviceManagementIntentSettingCategory.md) collection|Get the deviceManagementIntentSettingCategories from the categories navigation property.|
|[Add categories](../api/devicemanagementintent-post-categories.md)|[deviceManagementIntentSettingCategory](../resources/deviceManagementIntentSettingCategory.md)|Add categories by posting to the categories collection.|
|[List assignments](../api/devicemanagementintent-list-assignments.md)|[deviceManagementIntentAssignment](../resources/deviceManagementIntentAssignment.md) collection|Get the deviceManagementIntentAssignments from the assignments navigation property.|
|[Add assignments](../api/devicemanagementintent-post-assignments.md)|[deviceManagementIntentAssignment](../resources/deviceManagementIntentAssignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceSettingStateSummaries](../api/devicemanagementintent-list-devicesettingstatesummaries.md)|[deviceManagementIntentDeviceSettingStateSummary](../resources/deviceManagementIntentDeviceSettingStateSummary.md) collection|Get the deviceManagementIntentDeviceSettingStateSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/devicemanagementintent-post-devicesettingstatesummaries.md)|[deviceManagementIntentDeviceSettingStateSummary](../resources/deviceManagementIntentDeviceSettingStateSummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|
|[List deviceStates](../api/devicemanagementintent-list-devicestates.md)|[deviceManagementIntentDeviceState](../resources/deviceManagementIntentDeviceState.md) collection|Get the deviceManagementIntentDeviceStates from the deviceStates navigation property.|
|[Add deviceStates](../api/devicemanagementintent-post-devicestates.md)|[deviceManagementIntentDeviceState](../resources/deviceManagementIntentDeviceState.md)|Add deviceStates by posting to the deviceStates collection.|
|[List userStates](../api/devicemanagementintent-list-userstates.md)|[deviceManagementIntentUserState](../resources/deviceManagementIntentUserState.md) collection|Get the deviceManagementIntentUserStates from the userStates navigation property.|
|[Add userStates](../api/devicemanagementintent-post-userstates.md)|[deviceManagementIntentUserState](../resources/deviceManagementIntentUserState.md)|Add userStates by posting to the userStates collection.|
|[Get deviceManagementIntentDeviceStateSummary](../api/devicemanagementintentdevicestatesummary-get.md)|[deviceManagementIntentDeviceStateSummary](../resources/deviceManagementIntentDeviceStateSummary.md)|Read properties and relationships of the [deviceManagementIntentDeviceStateSummary](../resources/devicemanagementintentdevicestatesummary.md) object.|
|[Get deviceManagementIntentUserStateSummary](../api/devicemanagementintentuserstatesummary-get.md)|[deviceManagementIntentUserStateSummary](../resources/deviceManagementIntentUserStateSummary.md)|Read properties and relationships of the [deviceManagementIntentUserStateSummary](../resources/devicemanagementintentuserstatesummary.md) object.|
|[List intents](../api/intune-devices-devicemanagement-list-intents.md)|[deviceManagementIntent](../resources/deviceManagementIntent.md) collection|Get the deviceManagementIntents from the intents navigation property.|
|[Add intents](../api/intune-devices-devicemanagement-post-intents.md)|[deviceManagementIntent](../resources/deviceManagementIntent.md)|Add intents by posting to the intents collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|The user given description|
|displayName|String|The user given display name|
|id|String| Inherited from [entity](../resources/entity.md)|
|isAssigned|Boolean|Signifies whether or not the intent is assigned to users|
|lastModifiedDateTime|DateTimeOffset|When the intent was last modified|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance.|
|templateId|String|The ID of the template this intent was created from (if any)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceManagementIntentAssignment](../resources/deviceManagementIntentAssignment.md) collection|Collection of assignments|
|categories|[deviceManagementIntentSettingCategory](../resources/deviceManagementIntentSettingCategory.md) collection|Collection of setting categories within the intent|
|deviceSettingStateSummaries|[deviceManagementIntentDeviceSettingStateSummary](../resources/deviceManagementIntentDeviceSettingStateSummary.md) collection|Collection of settings and their states and counts of devices that belong to corresponding state for all settings within the intent|
|deviceStates|[deviceManagementIntentDeviceState](../resources/deviceManagementIntentDeviceState.md) collection|Collection of states of all devices that the intent is applied to|
|deviceStateSummary|[deviceManagementIntentDeviceStateSummary](../resources/deviceManagementIntentDeviceStateSummary.md)|A summary of device states and counts of devices that belong to corresponding state for all devices that the intent is applied to|
|settings|[deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md) collection|Collection of all settings to be applied|
|userStates|[deviceManagementIntentUserState](../resources/deviceManagementIntentUserState.md) collection|Collection of states of all users that the intent is applied to|
|userStateSummary|[deviceManagementIntentUserStateSummary](../resources/deviceManagementIntentUserStateSummary.md)|A summary of user states and counts of users that belong to corresponding state for all users that the intent is applied to|

## JSON Representation
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

