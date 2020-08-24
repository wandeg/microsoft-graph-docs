---
title: "deviceProtectionOverview resource type"
description: "Hardware information of a given device."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# deviceProtectionOverview resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Hardware information of a given device.

## Properties

| Property                           | Type  | Description                                                             |
| :--------------------------------- | :---- | :---------------------------------------------------------------------- |
| cleanDeviceCount                   | Int32 | Clean device count.                                                     |
| criticalFailuresDeviceCount        | Int32 | Critical failures device count.                                         |
| inactiveThreatAgentDeviceCount     | Int32 | Device with inactive threat agent count                                 |
| pendingFullScanDeviceCount         | Int32 | Pending full scan device count.                                         |
| pendingManualStepsDeviceCount      | Int32 | Pending manual steps device count.                                      |
| pendingOfflineScanDeviceCount      | Int32 | Pending offline scan device count.                                      |
| pendingQuickScanDeviceCount        | Int32 | Pending quick scan device count. Valid values -2147483648 to 2147483647 |
| pendingRestartDeviceCount          | Int32 | Pending restart device count.                                           |
| pendingSignatureUpdateDeviceCount  | Int32 | Device with old signature count.                                        |
| totalReportedDeviceCount           | Int32 | Total device count.                                                     |
| unknownStateThreatAgentDeviceCount | Int32 | Device with threat agent state as unknown count.                        |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceProtectionOverview",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceProtectionOverview",
  "cleanDeviceCount": "Int32",
  "criticalFailuresDeviceCount": "Int32",
  "inactiveThreatAgentDeviceCount": "Int32",
  "pendingFullScanDeviceCount": "Int32",
  "pendingManualStepsDeviceCount": "Int32",
  "pendingOfflineScanDeviceCount": "Int32",
  "pendingQuickScanDeviceCount": "Int32",
  "pendingRestartDeviceCount": "Int32",
  "pendingSignatureUpdateDeviceCount": "Int32",
  "totalReportedDeviceCount": "Int32",
  "unknownStateThreatAgentDeviceCount": "Int32"
}
```