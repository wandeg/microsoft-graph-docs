---
title: "windowsManagementApp resource type"
description: "Windows management app entity."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsManagementApp resource type


Namespace: microsoft.graph

Windows management app entity.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsManagementApp](../api/windowsmanagementapp-get.md)|[windowsManagementApp](../resources/windowsmanagementapp.md)|Read the properties and relationships of a [windowsManagementApp](../resources/windowsmanagementapp.md) object.|
|[Update windowsManagementApp](../api/windowsmanagementapp-update.md)|[windowsManagementApp](../resources/windowsmanagementapp.md)|Update the properties of a [windowsManagementApp](../resources/windowsmanagementapp.md) object.|
|[List healthStates](../api/windowsmanagementapp-list-healthstates.md)|[windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) collection|Get the windowsManagementAppHealthStates from the healthStates navigation property.|
|[Create healthStates](../api/windowsmanagementapp-post-healthstates.md)|[windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md)|Create a new healthStates object.|
|[Delete healthStates](../api/windowsmanagementapp-delete-healthstates.md)|None|Delete a [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) object.|
|[Update healthStates](../api/windowsmanagementapp-update-healthstates.md)|[windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md)|Update the properties of a healthStates object.|
|[Get windowsManagementAppHealthState](../api/windowsmanagementapphealthstate-get.md)|[windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md)|Read the properties and relationships of a [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|availableVersion|String|Windows management app available version.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|healthStates|[windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) collection|The list of health states for installed Windows management app.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementApp",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "String (identifier)",
  "availableVersion": "String"
}
```

