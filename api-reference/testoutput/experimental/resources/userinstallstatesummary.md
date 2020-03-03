---
title: "userInstallStateSummary resource type"
description: "Contains properties for the installation state summary for a user."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# userInstallStateSummary resource type

Contains properties for the installation state summary for a user.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userInstallStateSummary](../api/userinstallstatesummary-get.md)|[userInstallStateSummary](../resources/userInstallStateSummary.md)|Read properties and relationships of the [userInstallStateSummary](../resources/userinstallstatesummary.md) object.|
|[Delete userInstallStateSummary](../api/userinstallstatesummary-delete.md)|None|Deletes a [userInstallStateSummary](../resources/userinstallstatesummary.md).|
|[Update userInstallStateSummary](../api/userinstallstatesummary-update.md)|[userInstallStateSummary](../resources/userInstallStateSummary.md)|Update the properties of a [userInstallStateSummary](../resources/userinstallstatesummary.md) object.|
|[List deviceStates](../api/userinstallstatesummary-list-devicestates.md)|[deviceInstallState](../resources/deviceInstallState.md) collection|Get the deviceInstallStates from the deviceStates navigation property.|
|[Add deviceStates](../api/userinstallstatesummary-post-devicestates.md)|[deviceInstallState](../resources/deviceInstallState.md)|Add deviceStates by posting to the deviceStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|failedDeviceCount|Int32|Failed Device Count.|
|id|String| Inherited from [entity](../resources/entity.md)|
|installedDeviceCount|Int32|Installed Device Count.|
|notInstalledDeviceCount|Int32|Not installed device count.|
|userName|String|User name.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deviceStates|[deviceInstallState](../resources/deviceInstallState.md) collection|The install state of the eBook.|

## JSON Representation
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

