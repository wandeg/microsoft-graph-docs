---
title: "windowsManagementAppHealthState resource type"
description: "Windows management app health state entity."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsManagementAppHealthState resource type


Namespace: microsoft.graph

Windows management app health state entity.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsManagementAppHealthState](../api/windowsmanagementapphealthstate-get.md)|[windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md)|Read properties and relationships of the [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) object.|
|[Update windowsManagementAppHealthState](../api/windowsmanagementapphealthstate-update.md)|[windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md)|Update the properties of a [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) object.|
|[List healthStates](../api/windowsmanagementapp-list-healthstates.md)|[windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) collection|Get the windowsManagementAppHealthStates from the healthStates navigation property.|
|[Add healthStates](../api/windowsmanagementapp-post-healthstates.md)|[windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md)|Add healthStates by posting to the healthStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceName|String|Name of the device on which Windows management app is installed.|
|deviceOSVersion|String|Windows 10 OS version of the device on which Windows management app is installed.|
|healthState|Enumeration|Windows management app health state. Possible values are: `unknown`, `healthy`, `unhealthy`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|installedVersion|String|Windows management app installed version.|
|lastCheckInDateTime|DateTimeOffset|Windows management app last check-in time.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "id": "String (identifier)",
  "healthState": "String",
  "installedVersion": "String",
  "lastCheckInDateTime": "String (timestamp)",
  "deviceName": "String",
  "deviceOSVersion": "String"
}
```

