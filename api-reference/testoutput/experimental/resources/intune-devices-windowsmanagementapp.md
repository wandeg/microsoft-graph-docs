---
title: "windowsManagementApp resource type"
description: "Windows management app entity."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# windowsManagementApp resource type

Windows management app entity.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windowsManagementApps](../api/intune-devices-windowsmanagementapp-list.md)|[windowsManagementApp](../resources/intune-devices-windowsManagementApp.md) collection|List properties and relationships of the [windowsManagementApp](../resources/windowsmanagementapp.md) objects.|
|[Get windowsManagementApp](../api/intune-devices-windowsmanagementapp-get.md)|[windowsManagementApp](../resources/intune-devices-windowsManagementApp.md)|Read properties and relationships of the [windowsManagementApp](../resources/windowsmanagementapp.md) object.|
|[Create windowsManagementApp](../api/intune-devices-windowsmanagementapp-create.md)|[windowsManagementApp](../resources/intune-devices-windowsManagementApp.md)|Create a new [windowsManagementApp](../resources/windowsmanagementapp.md) object.|
|[Delete windowsManagementApp](../api/intune-devices-windowsmanagementapp-delete.md)|None|Deletes a [windowsManagementApp](../resources/windowsmanagementapp.md).|
|[Update windowsManagementApp](../api/intune-devices-windowsmanagementapp-update.md)|[windowsManagementApp](../resources/intune-devices-windowsManagementApp.md)|Update the properties of a [windowsManagementApp](../resources/windowsmanagementapp.md) object.|
|[List healthStates](../api/intune-devices-windowsmanagementapp-list-healthstates.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsManagementAppHealthState.md) collection|Get the windowsManagementAppHealthStates from the healthStates navigation property.|
|[Add healthStates](../api/intune-devices-windowsmanagementapp-post-healthstates.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsManagementAppHealthState.md)|Add healthStates by posting to the healthStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|availableVersion|String|Windows management app available version.|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|healthStates|[windowsManagementAppHealthState](../resources/intune-devices-windowsManagementAppHealthState.md) collection|The list of health states for installed Windows management app.|

## JSON Representation
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

