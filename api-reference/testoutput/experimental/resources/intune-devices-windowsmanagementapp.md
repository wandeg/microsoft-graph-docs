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
|[List windowsManagementApps](../api/intune-devices-windowsmanagementapp-list.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) collection|List properties and relationships of the [windowsManagementApp](../resources/windowsmanagementapp.md) objects.|
|[Get windowsManagementApp](../api/intune-devices-windowsmanagementapp-get.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.|
|[Create windowsManagementApp](../api/intune-devices-windowsmanagementapp-create.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Create a new [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.|
|[Delete windowsManagementApp](../api/intune-devices-windowsmanagementapp-delete.md)|None|Deletes a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).|
|[Update windowsManagementApp](../api/intune-devices-windowsmanagementapp-update.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.|
|[List healthStates](../api/intune-devices-windowsmanagementapp-list-healthstates.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection|Get the windowsManagementAppHealthStates from the healthStates navigation property.|
|[Add healthStates](../api/intune-devices-windowsmanagementapp-post-healthstates.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Add healthStates by posting to the healthStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|availableVersion|String|Windows management app available version.|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|healthStates|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection|The list of health states for installed Windows management app.|

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

