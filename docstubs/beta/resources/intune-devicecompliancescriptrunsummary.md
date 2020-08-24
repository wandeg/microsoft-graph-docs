---
title: "deviceComplianceScriptRunSummary resource type"
description: "Contains properties for the run summary of a device management script."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# deviceComplianceScriptRunSummary resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains properties for the run summary of a device management script.

## Methods

| Method                                                                                              | Return Type                                                                               | Description                                                                     |
| :-------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| [List deviceComplianceScriptRunSummary](../api/intune-devicecompliancescriptrunsummary-list.md)     | [deviceComplianceScriptRunSummary](intune-deviceComplianceScriptRunSummary.md) collection | List properties and relationships of a deviceComplianceScriptRunSummary object. |
| [Create deviceComplianceScriptRunSummary](../api/intune-devicecompliancescriptrunsummary-create.md) | [deviceComplianceScriptRunSummary](intune-deviceComplianceScriptRunSummary.md)            | Create a new deviceComplianceScriptRunSummary object.                           |
| [Get deviceComplianceScriptRunSummary](../api/intune-devicecompliancescriptrunsummary-get.md)       | [deviceComplianceScriptRunSummary](intune-deviceComplianceScriptRunSummary.md)            | Read properties and relationships of a deviceComplianceScriptRunSummary object. |
| [Update deviceComplianceScriptRunSummary](../api/intune-devicecompliancescriptrunsummary-update.md) | [deviceComplianceScriptRunSummary](intune-deviceComplianceScriptRunSummary.md)            | Update the properties of a deviceComplianceScriptRunSummary object.             |
| [Delete deviceComplianceScriptRunSummary](../api/intune-devicecompliancescriptrunsummary-delete.md) |                                                                                           | Delete a deviceComplianceScriptRunSummary object.                               |

## Properties

| Property                          | Type           | Description                                                                                                                                 |
| :-------------------------------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------ |
| detectionScriptErrorDeviceCount   | Int32          | Number of devices on which the detection script execution encountered an error and did not complete. Valid values -2147483648 to 2147483647 |
| detectionScriptPendingDeviceCount | Int32          | Number of devices which have not yet run the latest version of the device compliance script. Valid values -2147483648 to 2147483647         |
| id                                | String         | Key of the device compliance script run summary entity. This property is read-only. Read-only.                                              |
| issueDetectedDeviceCount          | Int32          | Number of devices for which the detection script found an issue. Valid values -2147483648 to 2147483647                                     |
| lastScriptRunDateTime             | DateTimeOffset | Last run time for the script across all devices                                                                                             |
| noIssueDetectedDeviceCount        | Int32          | Number of devices for which the detection script did not find an issue and the device is healthy. Valid values -2147483648 to 2147483647    |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScriptRunSummary",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "detectionScriptErrorDeviceCount": "Int32",
  "detectionScriptPendingDeviceCount": "Int32",
  "id": "String (identifier)",
  "issueDetectedDeviceCount": "Int32",
  "lastScriptRunDateTime": "DateTimeOffset",
  "noIssueDetectedDeviceCount": "Int32"
}
```