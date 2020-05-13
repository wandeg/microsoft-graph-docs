---
title: "userInstallStateSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userInstallStateSummary resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List userStateSummary](../api/intune-managedebook-list-userstatesummary.md)|[userInstallStateSummary](../resources/intune-userinstallstatesummary.md) collection|Get the userInstallStateSummaries from the userStateSummary navigation property.|
|[Create userStateSummary](../api/intune-managedebook-post-userstatesummary.md)|[userInstallStateSummary](../resources/intune-userinstallstatesummary.md)|Create a new userStateSummary object.|
|[Delete userStateSummary](../api/intune-managedebook-delete-userstatesummary.md)|None|Delete a [userInstallStateSummary](../resources/intune-userinstallstatesummary.md) object.|
|[Update userStateSummary](../api/intune-managedebook-update-userstatesummary.md)|[userInstallStateSummary](../resources/intune-userinstallstatesummary.md)|Update the properties of a userStateSummary object.|
|[Get userStateSummary](../api/intune-managedebook-get-userinstallstatesummary.md)|[userInstallStateSummary](../resources/intune-userinstallstatesummary.md)|Read the properties and relationships of a [userInstallStateSummary](../resources/intune-userinstallstatesummary.md) object.|
|[List deviceStates](../api/intune-userinstallstatesummary-list-devicestates.md)|[deviceInstallState](../resources/intune-deviceinstallstate.md) collection|Get the deviceInstallStates from the deviceStates navigation property.|
|[Create deviceStates](../api/intune-userinstallstatesummary-post-devicestates.md)|[deviceInstallState](../resources/intune-deviceinstallstate.md)|Create a new deviceStates object.|
|[Delete deviceStates](../api/intune-userinstallstatesummary-delete-devicestates.md)|None|Delete a [deviceInstallState](../resources/intune-deviceinstallstate.md) object.|
|[Update deviceStates](../api/intune-userinstallstatesummary-update-devicestates.md)|[deviceInstallState](../resources/intune-deviceinstallstate.md)|Update the properties of a deviceStates object.|
|[Get deviceStates](../api/intune-userinstallstatesummary-get-deviceinstallstate.md)|[deviceInstallState](../resources/intune-deviceinstallstate.md)|Read the properties and relationships of a [deviceInstallState](../resources/intune-deviceinstallstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|failedDeviceCount|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|installedDeviceCount|Int32|**TODO: Add Description**|
|notInstalledDeviceCount|Int32|**TODO: Add Description**|
|userName|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deviceStates|[deviceInstallState](../resources/intune-deviceinstallstate.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userInstallStateSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "String (identifier)",
  "userName": "String",
  "installedDeviceCount": "Integer",
  "failedDeviceCount": "Integer",
  "notInstalledDeviceCount": "Integer"
}
```

