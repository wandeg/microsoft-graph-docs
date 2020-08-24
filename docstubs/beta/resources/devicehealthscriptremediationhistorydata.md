---
title: "deviceHealthScriptRemediationHistoryData resource type"
description: "The number of devices remediated by a device health script on a given date."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# deviceHealthScriptRemediationHistoryData resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The number of devices remediated by a device health script on a given date.

## Properties

| Property              | Type  | Description                                                                         |
| :-------------------- | :---- | :---------------------------------------------------------------------------------- |
| date                  | Date  | The date on which devices were remediated by the device health script.              |
| noIssueDeviceCount    | Int32 | The number of devices that were found to have no issue by the device health script. |
| remediatedDeviceCount | Int32 | The number of devices remediated by the device health script.                       |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistoryData",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationHistoryData",
  "date": "Date",
  "noIssueDeviceCount": "Int32",
  "remediatedDeviceCount": "Int32"
}
```