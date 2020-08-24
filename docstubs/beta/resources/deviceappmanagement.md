---
title: "deviceAppManagement resource type"
description: "Singleton entity that acts as a container for all device app management functionality."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# deviceAppManagement resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Singleton entity that acts as a container for all device app management functionality.

## Methods

| Method                                                                                   | Return Type                                              | Description                                                                   |
| :--------------------------------------------------------------------------------------- | :------------------------------------------------------- | :---------------------------------------------------------------------------- |
| [List deviceAppManagement](../api/deviceappmanagement-list.md)                           | [deviceAppManagement](deviceAppManagement.md) collection | List properties and relationships of a deviceAppManagement object.            |
| [Create deviceAppManagement](../api/deviceappmanagement-create.md)                       | [deviceAppManagement](deviceAppManagement.md)            | Create a new deviceAppManagement object.                                      |
| [Get deviceAppManagement](../api/deviceappmanagement-get.md)                             | [deviceAppManagement](deviceAppManagement.md)            | Read properties and relationships of a deviceAppManagement object.            |
| [Update deviceAppManagement](../api/deviceappmanagement-update.md)                       | [deviceAppManagement](deviceAppManagement.md)            | Update the properties of a deviceAppManagement object.                        |
| [Delete deviceAppManagement](../api/deviceappmanagement-delete.md)                       |                                                          | Delete a deviceAppManagement object.                                          |
| [List windowsManagementApp](../api/deviceappmanagement-list-windowsmanagementapp.md)     | windowsManagementApp                                     | Get the windowsManagementApp from a windowsManagementApp navigation property. |
| [Add windowsManagementApp](../api/deviceappmanagement-post-windowsmanagementapp.md)      | windowsManagementApp                                     | Add windowsManagementApp by posting to the windowsManagementApp collection.   |
| [Get windowsManagementApp](../api/deviceappmanagement-get-windowsmanagementapp.md)       | windowsManagementApp                                     | Read the properties and relationships of a windowsManagementApp object.       |
| [Update windowsManagementApp](../api/deviceappmanagement-update-windowsmanagementapp.md) | windowsManagementApp                                     | Update the properties of a windowsManagementApp object.                       |
| [Remove windowsManagementApp](../api/deviceappmanagement-delete-windowsmanagementapp.md) |                                                          | Remove a windowsManagementApp object.                                         |

## Properties

| Property | Type   | Description                   |
| :------- | :----- | :---------------------------- |
| id       | String | Key of the entity. Read-only. |

## Relationships

| Relationship         | Type                                                         | Description             |
| :------------------- | :----------------------------------------------------------- | :---------------------- |
| windowsManagementApp | [windowsManagementApp](../resources/windowsmanagementapp.md) | Windows management app. |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```