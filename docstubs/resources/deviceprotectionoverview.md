---
title: "deviceProtectionOverview resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceProtectionOverview resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|cleanDeviceCount|Int32||
|criticalFailuresDeviceCount|Int32||
|inactiveThreatAgentDeviceCount|Int32||
|pendingFullScanDeviceCount|Int32||
|pendingManualStepsDeviceCount|Int32||
|pendingOfflineScanDeviceCount|Int32||
|pendingRestartDeviceCount|Int32||
|pendingSignatureUpdateDeviceCount|Int32||
|totalReportedDeviceCount|Int32||
|unknownStateThreatAgentDeviceCount|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceProtectionOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceProtectionOverview",
  "totalReportedDeviceCount": 1024,
  "inactiveThreatAgentDeviceCount": 1024,
  "unknownStateThreatAgentDeviceCount": 1024,
  "pendingSignatureUpdateDeviceCount": 1024,
  "cleanDeviceCount": 1024,
  "pendingFullScanDeviceCount": 1024,
  "pendingRestartDeviceCount": 1024,
  "pendingManualStepsDeviceCount": 1024,
  "pendingOfflineScanDeviceCount": 1024,
  "criticalFailuresDeviceCount": 1024
}
```

