---
title: "deviceHealthScriptAssignment resource type"
description: "Contains properties used to assign a device management script to a group."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# deviceHealthScriptAssignment resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains properties used to assign a device management script to a group.

## Methods

| Method                                                                                      | Return Type                                                                       | Description                                                                 |
| :------------------------------------------------------------------------------------------ | :-------------------------------------------------------------------------------- | :-------------------------------------------------------------------------- |
| [List deviceHealthScriptAssignment](../api/intune-devicehealthscriptassignment-list.md)     | [deviceHealthScriptAssignment](intune-deviceHealthScriptAssignment.md) collection | List properties and relationships of a deviceHealthScriptAssignment object. |
| [Create deviceHealthScriptAssignment](../api/intune-devicehealthscriptassignment-create.md) | [deviceHealthScriptAssignment](intune-deviceHealthScriptAssignment.md)            | Create a new deviceHealthScriptAssignment object.                           |
| [Get deviceHealthScriptAssignment](../api/intune-devicehealthscriptassignment-get.md)       | [deviceHealthScriptAssignment](intune-deviceHealthScriptAssignment.md)            | Read properties and relationships of a deviceHealthScriptAssignment object. |
| [Update deviceHealthScriptAssignment](../api/intune-devicehealthscriptassignment-update.md) | [deviceHealthScriptAssignment](intune-deviceHealthScriptAssignment.md)            | Update the properties of a deviceHealthScriptAssignment object.             |
| [Delete deviceHealthScriptAssignment](../api/intune-devicehealthscriptassignment-delete.md) |                                                                                   | Delete a deviceHealthScriptAssignment object.                               |

## Properties

| Property             | Type                                                                                             | Description                                                                                                |
| :------------------- | :----------------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------- |
| id                   | String                                                                                           | Key of the device health script assignment entity. This property is read-only. Read-only.                  |
| runRemediationScript | Boolean                                                                                          | Determine whether we want to run detection script only or run both detection script and remediation script |
| runSchedule          | [deviceHealthScriptRunSchedule](../resources/devicehealthscriptrunschedule.md)                   | Script run schedule for the target group                                                                   |
| target               | [deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md) | The Azure Active Directory group we are targeting the script to                                            |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
  "id": "String (identifier)",
  "runRemediationScript": "Boolean",
  "runSchedule": {"@odata.type": "microsoft.graph.deviceHealthScriptRunSchedule"},
  "target": {"@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"}
}
```