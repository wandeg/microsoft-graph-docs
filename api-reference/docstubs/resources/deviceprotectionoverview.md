---
title: "deviceProtectionOverview resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceProtectionOverview resource type


Namespace: microsoft.graph

**TODO: Add Description**

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

