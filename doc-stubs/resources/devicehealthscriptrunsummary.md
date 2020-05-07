---
title: "deviceHealthScriptRunSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceHealthScriptRunSummary resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|detectionScriptErrorDeviceCount|Int32|**TODO: Add Description**|
|detectionScriptPendingDeviceCount|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|issueDetectedDeviceCount|Int32|**TODO: Add Description**|
|issueRemediatedCumulativeDeviceCount|Int32|**TODO: Add Description**|
|issueRemediatedDeviceCount|Int32|**TODO: Add Description**|
|issueReoccurredDeviceCount|Int32|**TODO: Add Description**|
|lastScriptRunDateTime|DateTimeOffset|**TODO: Add Description**|
|noIssueDetectedDeviceCount|Int32|**TODO: Add Description**|
|remediationScriptErrorDeviceCount|Int32|**TODO: Add Description**|
|remediationSkippedDeviceCount|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "noIssueDetectedDeviceCount": "Integer",
  "issueDetectedDeviceCount": "Integer",
  "detectionScriptErrorDeviceCount": "Integer",
  "detectionScriptPendingDeviceCount": "Integer",
  "issueRemediatedDeviceCount": "Integer",
  "remediationSkippedDeviceCount": "Integer",
  "issueReoccurredDeviceCount": "Integer",
  "remediationScriptErrorDeviceCount": "Integer",
  "lastScriptRunDateTime": "String (timestamp)",
  "issueRemediatedCumulativeDeviceCount": "Integer"
}
```

