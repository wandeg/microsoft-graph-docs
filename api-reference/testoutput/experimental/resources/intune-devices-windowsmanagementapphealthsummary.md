---
title: "windowsManagementAppHealthSummary resource type"
description: "Contains properties for the health summary of the Windows management app."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# windowsManagementAppHealthSummary resource type

Contains properties for the health summary of the Windows management app.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windowsManagementAppHealthSummaries](../api/intune-devices-windowsmanagementapphealthsummary-list.md)|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsManagementAppHealthSummary.md) collection|List properties and relationships of the [windowsManagementAppHealthSummary](../resources/windowsmanagementapphealthsummary.md) objects.|
|[Get windowsManagementAppHealthSummary](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsManagementAppHealthSummary.md)|Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/windowsmanagementapphealthsummary.md) object.|
|[Create windowsManagementAppHealthSummary](../api/intune-devices-windowsmanagementapphealthsummary-create.md)|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsManagementAppHealthSummary.md)|Create a new [windowsManagementAppHealthSummary](../resources/windowsmanagementapphealthsummary.md) object.|
|[Delete windowsManagementAppHealthSummary](../api/intune-devices-windowsmanagementapphealthsummary-delete.md)|None|Deletes a [windowsManagementAppHealthSummary](../resources/windowsmanagementapphealthsummary.md).|
|[Update windowsManagementAppHealthSummary](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsManagementAppHealthSummary.md)|Update the properties of a [windowsManagementAppHealthSummary](../resources/windowsmanagementapphealthsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|healthyDeviceCount|Int32|Healthy device count.|
|id|String| Inherited from [entity](../resources/entity.md)|
|unhealthyDeviceCount|Int32|Unhealthy device count.|
|unknownDeviceCount|Int32|Unknown device count.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "id": "String (identifier)",
  "healthyDeviceCount": 1024,
  "unhealthyDeviceCount": 1024,
  "unknownDeviceCount": 1024
}
```

