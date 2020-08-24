---
title: "windowsManagementAppHealthSummary resource type"
description: "Contains properties for the health summary of the Windows management app."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# windowsManagementAppHealthSummary resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains properties for the health summary of the Windows management app.

## Methods

| Method                                                                                                | Return Type                                                                                 | Description                                                                      |
| :---------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------ | :------------------------------------------------------------------------------- |
| [List windowsManagementAppHealthSummary](../api/intune-windowsmanagementapphealthsummary-list.md)     | [windowsManagementAppHealthSummary](intune-windowsManagementAppHealthSummary.md) collection | List properties and relationships of a windowsManagementAppHealthSummary object. |
| [Create windowsManagementAppHealthSummary](../api/intune-windowsmanagementapphealthsummary-create.md) | [windowsManagementAppHealthSummary](intune-windowsManagementAppHealthSummary.md)            | Create a new windowsManagementAppHealthSummary object.                           |
| [Get windowsManagementAppHealthSummary](../api/intune-windowsmanagementapphealthsummary-get.md)       | [windowsManagementAppHealthSummary](intune-windowsManagementAppHealthSummary.md)            | Read properties and relationships of a windowsManagementAppHealthSummary object. |
| [Update windowsManagementAppHealthSummary](../api/intune-windowsmanagementapphealthsummary-update.md) | [windowsManagementAppHealthSummary](intune-windowsManagementAppHealthSummary.md)            | Update the properties of a windowsManagementAppHealthSummary object.             |
| [Delete windowsManagementAppHealthSummary](../api/intune-windowsmanagementapphealthsummary-delete.md) |                                                                                             | Delete a windowsManagementAppHealthSummary object.                               |

## Properties

| Property             | Type   | Description                                                                                     |
| :------------------- | :----- | :---------------------------------------------------------------------------------------------- |
| healthyDeviceCount   | Int32  | Healthy device count.                                                                           |
| id                   | String | Key of the Windows management app health summary entity. This property is read-only. Read-only. |
| unhealthyDeviceCount | Int32  | Unhealthy device count.                                                                         |
| unknownDeviceCount   | Int32  | Unknown device count.                                                                           |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthSummary",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "healthyDeviceCount": "Int32",
  "id": "String (identifier)",
  "unhealthyDeviceCount": "Int32",
  "unknownDeviceCount": "Int32"
}
```