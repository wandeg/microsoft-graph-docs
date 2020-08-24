---
title: "windowsManagementApp resource type"
description: "Windows management app entity."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# windowsManagementApp resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Windows management app entity.

## Methods

| Method                                                                           | Return Type                                                       | Description                                                                        |
| :------------------------------------------------------------------------------- | :---------------------------------------------------------------- | :--------------------------------------------------------------------------------- |
| [List windowsManagementApp](../api/intune-windowsmanagementapp-list.md)          | [windowsManagementApp](intune-windowsManagementApp.md) collection | List properties and relationships of a windowsManagementApp object.                |
| [Create windowsManagementApp](../api/intune-windowsmanagementapp-create.md)      | [windowsManagementApp](intune-windowsManagementApp.md)            | Create a new windowsManagementApp object.                                          |
| [Get windowsManagementApp](../api/intune-windowsmanagementapp-get.md)            | [windowsManagementApp](intune-windowsManagementApp.md)            | Read properties and relationships of a windowsManagementApp object.                |
| [Update windowsManagementApp](../api/intune-windowsmanagementapp-update.md)      | [windowsManagementApp](intune-windowsManagementApp.md)            | Update the properties of a windowsManagementApp object.                            |
| [Delete windowsManagementApp](../api/intune-windowsmanagementapp-delete.md)      |                                                                   | Delete a windowsManagementApp object.                                              |
| [List healthStates](../api/intune-windowsmanagementapp-list-healthstates.md)     | windowsManagementAppHealthState                                   | Get the windowsManagementAppHealthState from a healthStates navigation property.   |
| [Create healthStates](../api/intune-windowsmanagementapp-post-healthstates.md)   | windowsManagementAppHealthState                                   | Create a new healthStates object.                                                  |
| [Get healthStates](../api/intune-windowsmanagementapp-get-healthstates.md)       | windowsManagementAppHealthState                                   | Read the properties and relationships of a windowsManagementAppHealthState object. |
| [Update healthStates](../api/intune-windowsmanagementapp-update-healthstates.md) | windowsManagementAppHealthState                                   | Update the properties of a healthStates object.                                    |
| [Delete healthStates](../api/intune-windowsmanagementapp-delete-healthstates.md) |                                                                   | Delete a windowsManagementAppHealthState object.                                   |

## Properties

| Property         | Type   | Description                                                 |
| :--------------- | :----- | :---------------------------------------------------------- |
| availableVersion | String | Windows management app available version.                   |
| id               | String | Unique Identifier for the Windows management app Read-only. |

## Relationships

| Relationship | Type                                                                                          | Description                                                     |
| :----------- | :-------------------------------------------------------------------------------------------- | :-------------------------------------------------------------- |
| healthStates | [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) collection | The list of health states for installed Windows management app. |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementApp",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "availableVersion": "String",
  "id": "String (identifier)"
}
```