---
title: "windowsManagementApp resource type"
description: "Windows management app entity."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsManagementApp resource type


Namespace: microsoft.graph

Windows management app entity.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsManagementApp](../api/windowsmanagementapp-get.md)|[windowsManagementApp](../resources/windowsmanagementapp.md)|Read properties and relationships of the [windowsManagementApp](../resources/windowsmanagementapp.md) object.|
|[Update windowsManagementApp](../api/windowsmanagementapp-update.md)|[windowsManagementApp](../resources/windowsmanagementapp.md)|Update the properties of a [windowsManagementApp](../resources/windowsmanagementapp.md) object.|
|[List healthStates](../api/windowsmanagementapp-list-healthstates.md)|[windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) collection|Get the windowsManagementAppHealthStates from the healthStates navigation property.|
|[Add healthStates](../api/windowsmanagementapp-post-healthstates.md)|[windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md)|Add healthStates by posting to the healthStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|availableVersion|String|Windows management app available version.|
|id|String| Inherited from [entity](../resources/entity.md)|

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

