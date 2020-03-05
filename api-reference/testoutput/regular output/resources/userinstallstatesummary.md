---
title: "userInstallStateSummary resource type"
description: "Contains properties for the installation state summary for a user."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userInstallStateSummary resource type


Namespace: microsoft.graph

Contains properties for the installation state summary for a user.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List userInstallStateSummaries](../api/userinstallstatesummary-list.md)|[userInstallStateSummary](../resources/userinstallstatesummary.md) collection|List properties and relationships of the [userInstallStateSummary](../resources/userinstallstatesummary.md) objects.|
|[Get userInstallStateSummary](../api/userinstallstatesummary-get.md)|[userInstallStateSummary](../resources/userinstallstatesummary.md)|Read properties and relationships of the [userInstallStateSummary](../resources/userinstallstatesummary.md) object.|
|[Create userInstallStateSummary](../api/userinstallstatesummary-create.md)|[userInstallStateSummary](../resources/userinstallstatesummary.md)|Create a new [userInstallStateSummary](../resources/userinstallstatesummary.md) object.|
|[Delete userInstallStateSummary](../api/userinstallstatesummary-delete.md)|None|Deletes a [userInstallStateSummary](../resources/userinstallstatesummary.md).|
|[Update userInstallStateSummary](../api/userinstallstatesummary-update.md)|[userInstallStateSummary](../resources/userinstallstatesummary.md)|Update the properties of a [userInstallStateSummary](../resources/userinstallstatesummary.md) object.|
|[List deviceStates](../api/userinstallstatesummary-list-devicestates.md)|[deviceInstallState](../resources/deviceinstallstate.md) collection|Get the deviceInstallStates from the deviceStates navigation property.|
|[Add deviceStates](../api/userinstallstatesummary-post-devicestates.md)|[deviceInstallState](../resources/deviceinstallstate.md)|Add deviceStates by posting to the deviceStates collection.|

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

