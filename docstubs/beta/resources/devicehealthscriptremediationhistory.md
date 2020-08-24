---
title: "deviceHealthScriptRemediationHistory resource type"
description: "The number of devices remediated by a device health script on a given date with the last modified time."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# deviceHealthScriptRemediationHistory resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The number of devices remediated by a device health script on a given date with the last modified time.

## Properties

| Property             | Type                                                                                                            | Description                                                                     |
| :------------------- | :-------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| historyData          | [deviceHealthScriptRemediationHistoryData](../resources/devicehealthscriptremediationhistorydata.md) collection | The number of devices remediated by the device health script on the given date. |
| lastModifiedDateTime | DateTimeOffset                                                                                                  | The date on which the results history is calculated for the healthscript.       |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistory",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationHistory",
  "historyData": [{"@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistoryData"}],
  "lastModifiedDateTime": "DateTimeOffset"
}
```