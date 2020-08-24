---
title: "deviceManagementScriptAssignment resource type"
description: "Contains properties used to assign a device management script to a group."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# deviceManagementScriptAssignment resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains properties used to assign a device management script to a group.

## Methods

| Method                                                                                              | Return Type                                                                               | Description                                                                     |
| :-------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| [List deviceManagementScriptAssignment](../api/intune-devicemanagementscriptassignment-list.md)     | [deviceManagementScriptAssignment](intune-deviceManagementScriptAssignment.md) collection | List properties and relationships of a deviceManagementScriptAssignment object. |
| [Create deviceManagementScriptAssignment](../api/intune-devicemanagementscriptassignment-create.md) | [deviceManagementScriptAssignment](intune-deviceManagementScriptAssignment.md)            | Create a new deviceManagementScriptAssignment object.                           |
| [Get deviceManagementScriptAssignment](../api/intune-devicemanagementscriptassignment-get.md)       | [deviceManagementScriptAssignment](intune-deviceManagementScriptAssignment.md)            | Read properties and relationships of a deviceManagementScriptAssignment object. |
| [Update deviceManagementScriptAssignment](../api/intune-devicemanagementscriptassignment-update.md) | [deviceManagementScriptAssignment](intune-deviceManagementScriptAssignment.md)            | Update the properties of a deviceManagementScriptAssignment object.             |
| [Delete deviceManagementScriptAssignment](../api/intune-devicemanagementscriptassignment-delete.md) |                                                                                           | Delete a deviceManagementScriptAssignment object.                               |

## Properties

| Property | Type                                                                                             | Description                                                                                         |
| :------- | :----------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------- |
| id       | String                                                                                           | Key of the device management script group assignment entity. This property is read-only. Read-only. |
| target   | [deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md) | The Id of the Azure Active Directory group we are targeting the script to.                          |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "String (identifier)",
  "target": {"@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"}
}
```