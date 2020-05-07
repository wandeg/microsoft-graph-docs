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
|cleanDeviceCount|Int32|**TODO: Add Description**|
|criticalFailuresDeviceCount|Int32|**TODO: Add Description**|
|inactiveThreatAgentDeviceCount|Int32|**TODO: Add Description**|
|pendingFullScanDeviceCount|Int32|**TODO: Add Description**|
|pendingManualStepsDeviceCount|Int32|**TODO: Add Description**|
|pendingOfflineScanDeviceCount|Int32|**TODO: Add Description**|
|pendingRestartDeviceCount|Int32|**TODO: Add Description**|
|pendingSignatureUpdateDeviceCount|Int32|**TODO: Add Description**|
|totalReportedDeviceCount|Int32|**TODO: Add Description**|
|unknownStateThreatAgentDeviceCount|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceProtectionOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceProtectionOverview",
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

