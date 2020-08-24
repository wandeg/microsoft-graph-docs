---
title: "deviceManagementScriptGroupAssignment resource type"
description: "Contains properties used to assign a device management script to a group."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# deviceManagementScriptGroupAssignment resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains properties used to assign a device management script to a group.

## Methods

| Method                                                                                                        | Return Type                                                                                         | Description                                                                          |
| :------------------------------------------------------------------------------------------------------------ | :-------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------- |
| [List deviceManagementScriptGroupAssignment](../api/intune-devicemanagementscriptgroupassignment-list.md)     | [deviceManagementScriptGroupAssignment](intune-deviceManagementScriptGroupAssignment.md) collection | List properties and relationships of a deviceManagementScriptGroupAssignment object. |
| [Create deviceManagementScriptGroupAssignment](../api/intune-devicemanagementscriptgroupassignment-create.md) | [deviceManagementScriptGroupAssignment](intune-deviceManagementScriptGroupAssignment.md)            | Create a new deviceManagementScriptGroupAssignment object.                           |
| [Get deviceManagementScriptGroupAssignment](../api/intune-devicemanagementscriptgroupassignment-get.md)       | [deviceManagementScriptGroupAssignment](intune-deviceManagementScriptGroupAssignment.md)            | Read properties and relationships of a deviceManagementScriptGroupAssignment object. |
| [Update deviceManagementScriptGroupAssignment](../api/intune-devicemanagementscriptgroupassignment-update.md) | [deviceManagementScriptGroupAssignment](intune-deviceManagementScriptGroupAssignment.md)            | Update the properties of a deviceManagementScriptGroupAssignment object.             |
| [Delete deviceManagementScriptGroupAssignment](../api/intune-devicemanagementscriptgroupassignment-delete.md) |                                                                                                     | Delete a deviceManagementScriptGroupAssignment object.                               |

## Properties

| Property      | Type   | Description                                                                                         |
| :------------ | :----- | :-------------------------------------------------------------------------------------------------- |
| id            | String | Key of the device management script group assignment entity. This property is read-only. Read-only. |
| targetGroupId | String | The Id of the Azure Active Directory group we are targeting the script to.                          |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptGroupAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```