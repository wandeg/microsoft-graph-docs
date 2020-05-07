---
title: "deviceProtectionOverview resource type"
description: "Hardware information of a given device."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceProtectionOverview resource type


Namespace: microsoft.graph

Hardware information of a given device.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|cleanDeviceCount|Int32|Clean device count.|
|criticalFailuresDeviceCount|Int32|Critical failures device count.|
|inactiveThreatAgentDeviceCount|Int32|Device with inactive threat agent count|
|pendingFullScanDeviceCount|Int32|Pending full scan device count.|
|pendingManualStepsDeviceCount|Int32|Pending manual steps device count.|
|pendingOfflineScanDeviceCount|Int32|Pending offline scan device count.|
|pendingRestartDeviceCount|Int32|Pending restart device count.|
|pendingSignatureUpdateDeviceCount|Int32|Device with old signature count.|
|totalReportedDeviceCount|Int32|Total device count.|
|unknownStateThreatAgentDeviceCount|Int32|Device with threat agent state as unknown count.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.management.services.api.deviceProtectionOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.deviceProtectionOverview",
  "totalReportedDeviceCount": "Integer",
  "inactiveThreatAgentDeviceCount": "Integer",
  "unknownStateThreatAgentDeviceCount": "Integer",
  "pendingSignatureUpdateDeviceCount": "Integer",
  "cleanDeviceCount": "Integer",
  "pendingFullScanDeviceCount": "Integer",
  "pendingRestartDeviceCount": "Integer",
  "pendingManualStepsDeviceCount": "Integer",
  "pendingOfflineScanDeviceCount": "Integer",
  "criticalFailuresDeviceCount": "Integer"
}
```

