---
title: "deviceManagementReports resource type"
description: "Singleton entity that acts as a container for all reports functionality."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# deviceManagementReports resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Singleton entity that acts as a container for all reports functionality.

## Methods

| Method                                                                             | Return Type                                                      | Description                                                            |
| :--------------------------------------------------------------------------------- | :--------------------------------------------------------------- | :--------------------------------------------------------------------- |
| [List deviceManagementReports](../api/devicemanagementreports-list.md)             | [deviceManagementReports](deviceManagementReports.md) collection | List properties and relationships of a deviceManagementReports object. |
| [Create deviceManagementReports](../api/devicemanagementreports-create.md)         | [deviceManagementReports](deviceManagementReports.md)            | Create a new deviceManagementReports object.                           |
| [Get deviceManagementReports](../api/devicemanagementreports-get.md)               | [deviceManagementReports](deviceManagementReports.md)            | Read properties and relationships of a deviceManagementReports object. |
| [Update deviceManagementReports](../api/devicemanagementreports-update.md)         | [deviceManagementReports](deviceManagementReports.md)            | Update the properties of a deviceManagementReports object.             |
| [Delete deviceManagementReports](../api/devicemanagementreports-delete.md)         |                                                                  | Delete a deviceManagementReports object.                               |
| [getActiveMalwareReport](../api/devicemanagementreports-getActiveMalwareReport.md) | Stream                                                           |                                                                        |

## Properties

| Property | Type   | Description                                  |
| :------- | :----- | :------------------------------------------- |
| id       | String | Unique identifier for this entity Read-only. |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementReports",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "String (identifier)"
}
```