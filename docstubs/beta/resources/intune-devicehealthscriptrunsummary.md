---
title: "deviceHealthScriptRunSummary resource type"
description: "Contains properties for the run summary of a device management script."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# deviceHealthScriptRunSummary resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains properties for the run summary of a device management script.

## Methods

| Method                                                                                      | Return Type                                                                       | Description                                                                 |
| :------------------------------------------------------------------------------------------ | :-------------------------------------------------------------------------------- | :-------------------------------------------------------------------------- |
| [List deviceHealthScriptRunSummary](../api/intune-devicehealthscriptrunsummary-list.md)     | [deviceHealthScriptRunSummary](intune-deviceHealthScriptRunSummary.md) collection | List properties and relationships of a deviceHealthScriptRunSummary object. |
| [Create deviceHealthScriptRunSummary](../api/intune-devicehealthscriptrunsummary-create.md) | [deviceHealthScriptRunSummary](intune-deviceHealthScriptRunSummary.md)            | Create a new deviceHealthScriptRunSummary object.                           |
| [Get deviceHealthScriptRunSummary](../api/intune-devicehealthscriptrunsummary-get.md)       | [deviceHealthScriptRunSummary](intune-deviceHealthScriptRunSummary.md)            | Read properties and relationships of a deviceHealthScriptRunSummary object. |
| [Update deviceHealthScriptRunSummary](../api/intune-devicehealthscriptrunsummary-update.md) | [deviceHealthScriptRunSummary](intune-deviceHealthScriptRunSummary.md)            | Update the properties of a deviceHealthScriptRunSummary object.             |
| [Delete deviceHealthScriptRunSummary](../api/intune-devicehealthscriptrunsummary-delete.md) |                                                                                   | Delete a deviceHealthScriptRunSummary object.                               |

## Properties

| Property                             | Type           | Description                                                                                                       |
| :----------------------------------- | :------------- | :---------------------------------------------------------------------------------------------------------------- |
| detectionScriptErrorDeviceCount      | Int32          | Number of devices on which the detection script execution encountered an error and did not complete               |
| detectionScriptPendingDeviceCount    | Int32          | Number of devices which have not yet run the latest version of the device health script                           |
| id                                   | String         | Key of the device health script run summary entity. This property is read-only. Read-only.                        |
| issueDetectedDeviceCount             | Int32          | Number of devices for which the detection script found an issue                                                   |
| issueRemediatedCumulativeDeviceCount | Int32          | Number of devices that were remediated over the last 30 days                                                      |
| issueRemediatedDeviceCount           | Int32          | Number of devices for which the remediation script was able to resolve the detected issue                         |
| issueReoccurredDeviceCount           | Int32          | Number of devices for which the remediation script executed successfully but failed to resolve the detected issue |
| lastScriptRunDateTime                | DateTimeOffset | Last run time for the script across all devices                                                                   |
| noIssueDetectedDeviceCount           | Int32          | Number of devices for which the detection script did not find an issue and the device is healthy                  |
| remediationScriptErrorDeviceCount    | Int32          | Number of devices for which the remediation script execution encountered an error and did not complete            |
| remediationSkippedDeviceCount        | Int32          | Number of devices for which remediation was skipped                                                               |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunSummary",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "detectionScriptErrorDeviceCount": "Int32",
  "detectionScriptPendingDeviceCount": "Int32",
  "id": "String (identifier)",
  "issueDetectedDeviceCount": "Int32",
  "issueRemediatedCumulativeDeviceCount": "Int32",
  "issueRemediatedDeviceCount": "Int32",
  "issueReoccurredDeviceCount": "Int32",
  "lastScriptRunDateTime": "DateTimeOffset",
  "noIssueDetectedDeviceCount": "Int32",
  "remediationScriptErrorDeviceCount": "Int32",
  "remediationSkippedDeviceCount": "Int32"
}
```