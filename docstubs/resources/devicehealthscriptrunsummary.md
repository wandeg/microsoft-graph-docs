---
title: "deviceHealthScriptRunSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceHealthScriptRunSummary resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceHealthScriptRunSummary](../api/devicehealthscriptrunsummary-get.md)|[deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md)|Read properties and relationships of the [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md) object.|
|[Update deviceHealthScriptRunSummary](../api/devicehealthscriptrunsummary-update.md)|[deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md)|Update the properties of a [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|detectionScriptErrorDeviceCount|Int32||
|detectionScriptPendingDeviceCount|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|issueDetectedDeviceCount|Int32||
|issueRemediatedCumulativeDeviceCount|Int32||
|issueRemediatedDeviceCount|Int32||
|issueReoccurredDeviceCount|Int32||
|lastScriptRunDateTime|DateTimeOffset||
|noIssueDetectedDeviceCount|Int32||
|remediationScriptErrorDeviceCount|Int32||
|remediationSkippedDeviceCount|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "id": "String (identifier)",
  "noIssueDetectedDeviceCount": 1024,
  "issueDetectedDeviceCount": 1024,
  "detectionScriptErrorDeviceCount": 1024,
  "detectionScriptPendingDeviceCount": 1024,
  "issueRemediatedDeviceCount": 1024,
  "remediationSkippedDeviceCount": 1024,
  "issueReoccurredDeviceCount": 1024,
  "remediationScriptErrorDeviceCount": 1024,
  "lastScriptRunDateTime": "String (timestamp)",
  "issueRemediatedCumulativeDeviceCount": 1024
}
```

