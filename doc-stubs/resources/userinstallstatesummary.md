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
|[List deviceStates](../api/userinstallstatesummary-list-devicestates.md)|[deviceInstallState](../resources/deviceinstallstate.md) collection|Get the deviceInstallStates from the deviceStates navigation property.|
|[Create deviceStates](../api/userinstallstatesummary-post-devicestates.md)|[deviceInstallState](../resources/deviceinstallstate.md)|Create a new deviceStates object.|
|[Delete deviceStates](../api/userinstallstatesummary-delete-devicestates.md)|None|Delete a [deviceInstallState](../resources/deviceinstallstate.md) object.|
|[Update deviceStates](../api/userinstallstatesummary-update-devicestates.md)|[deviceInstallState](../resources/deviceinstallstate.md)|Update the properties of a deviceStates object.|
|[Get deviceInstallState](../api/deviceinstallstate-get.md)|[deviceInstallState](../resources/deviceinstallstate.md)|Read the properties and relationships of a [deviceInstallState](../resources/deviceinstallstate.md) object.|
|[List userStateSummary](../api/managedebook-list-userstatesummary.md)|[userInstallStateSummary](../resources/userinstallstatesummary.md) collection|Get the userInstallStateSummaries from the userStateSummary navigation property.|
|[Create userStateSummary](../api/managedebook-post-userstatesummary.md)|[userInstallStateSummary](../resources/userinstallstatesummary.md)|Create a new userStateSummary object.|

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
|deviceStates|[deviceInstallState](../resources/deviceinstallstate.md) collection|**TODO: Add Description**|

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

