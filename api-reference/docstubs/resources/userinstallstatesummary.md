---
title: "userInstallStateSummary resource type"
description: "Contains properties for the installation state summary for a user."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userInstallStateSummary resource type


Namespace: microsoft.graph

Contains properties for the installation state summary for a user.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userInstallStateSummary](../api/userinstallstatesummary-get.md)|[userInstallStateSummary](../resources/userinstallstatesummary.md)|Read the properties and relationships of a [userInstallStateSummary](../resources/userinstallstatesummary.md) object.|
|[Update userInstallStateSummary](../api/userinstallstatesummary-update.md)|[userInstallStateSummary](../resources/userinstallstatesummary.md)|Update the properties of a [userInstallStateSummary](../resources/userinstallstatesummary.md) object.|
|[List deviceStates](../api/userinstallstatesummary-list-devicestates.md)|[deviceInstallState](../resources/deviceinstallstate.md) collection|Get the deviceInstallStates from the deviceStates navigation property.|
|[Create deviceStates](../api/userinstallstatesummary-post-devicestates.md)|[deviceInstallState](../resources/deviceinstallstate.md)|Create a new deviceStates object.|
|[Delete deviceStates](../api/userinstallstatesummary-delete-devicestates.md)|None|Delete a [deviceInstallState](../resources/deviceinstallstate.md) object.|
|[Update deviceStates](../api/userinstallstatesummary-update-devicestates.md)|[deviceInstallState](../resources/deviceinstallstate.md)|Update the properties of a deviceStates object.|
|[Get deviceInstallState](../api/deviceinstallstate-get.md)|[deviceInstallState](../resources/deviceinstallstate.md)|Read the properties and relationships of a [deviceInstallState](../resources/deviceinstallstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|failedDeviceCount|Int32|Failed Device Count.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|installedDeviceCount|Int32|Installed Device Count.|
|notInstalledDeviceCount|Int32|Not installed device count.|
|userName|String|User name.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deviceStates|[deviceInstallState](../resources/deviceinstallstate.md) collection|The install state of the eBook.|

## JSON representation
Here is a JSON representation of the resource.
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
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```

