---
title: "deviceHealthScriptRemediationSummary resource type"
description: "The number of device health scripts deployed and the number of devices the scripts remediated."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# deviceHealthScriptRemediationSummary resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The number of device health scripts deployed and the number of devices the scripts remediated.

## Properties

| Property              | Type  | Description                                                |
| :-------------------- | :---- | :--------------------------------------------------------- |
| remediatedDeviceCount | Int32 | The number of devices remediated by device health scripts. |
| scriptCount           | Int32 | The number of device health scripts deployed.              |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationSummary",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationSummary",
  "remediatedDeviceCount": "Int32",
  "scriptCount": "Int32"
}
```