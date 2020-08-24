---
title: "deviceManagementScriptRunSummary resource type"
description: "Contains properties for the run summary of a device management script."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# deviceManagementScriptRunSummary resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains properties for the run summary of a device management script.

## Methods

| Method                                                                                              | Return Type                                                                               | Description                                                                     |
| :-------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| [List deviceManagementScriptRunSummary](../api/intune-devicemanagementscriptrunsummary-list.md)     | [deviceManagementScriptRunSummary](intune-deviceManagementScriptRunSummary.md) collection | List properties and relationships of a deviceManagementScriptRunSummary object. |
| [Create deviceManagementScriptRunSummary](../api/intune-devicemanagementscriptrunsummary-create.md) | [deviceManagementScriptRunSummary](intune-deviceManagementScriptRunSummary.md)            | Create a new deviceManagementScriptRunSummary object.                           |
| [Get deviceManagementScriptRunSummary](../api/intune-devicemanagementscriptrunsummary-get.md)       | [deviceManagementScriptRunSummary](intune-deviceManagementScriptRunSummary.md)            | Read properties and relationships of a deviceManagementScriptRunSummary object. |
| [Update deviceManagementScriptRunSummary](../api/intune-devicemanagementscriptrunsummary-update.md) | [deviceManagementScriptRunSummary](intune-deviceManagementScriptRunSummary.md)            | Update the properties of a deviceManagementScriptRunSummary object.             |
| [Delete deviceManagementScriptRunSummary](../api/intune-devicemanagementscriptrunsummary-delete.md) |                                                                                           | Delete a deviceManagementScriptRunSummary object.                               |

## Properties

| Property           | Type   | Description                                                                                    |
| :----------------- | :----- | :--------------------------------------------------------------------------------------------- |
| errorDeviceCount   | Int32  | Error device count.                                                                            |
| errorUserCount     | Int32  | Error user count.                                                                              |
| id                 | String | Key of the device management script run summary entity. This property is read-only. Read-only. |
| successDeviceCount | Int32  | Success device count.                                                                          |
| successUserCount   | Int32  | Success user count.                                                                            |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptRunSummary",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "errorDeviceCount": "Int32",
  "errorUserCount": "Int32",
  "id": "String (identifier)",
  "successDeviceCount": "Int32",
  "successUserCount": "Int32"
}
```