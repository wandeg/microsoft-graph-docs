---
title: "windowsManagementAppHealthState resource type"
description: "Windows management app health state entity."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsManagementAppHealthState resource type


Namespace: microsoft.graph

Windows management app health state entity.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsManagementAppHealthState](../api/windowsmanagementapphealthstate-get.md)|[windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md)|Read the properties and relationships of a [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) object.|
|[Update windowsManagementAppHealthState](../api/windowsmanagementapphealthstate-update.md)|[windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md)|Update the properties of a [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceName|String|Name of the device on which Windows management app is installed.|
|deviceOSVersion|String|Windows 10 OS version of the device on which Windows management app is installed.|
|healthState|healthState|Windows management app health state. Possible values are: `unknown`, `healthy`, `unhealthy`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
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

