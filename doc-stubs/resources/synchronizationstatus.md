---
title: "synchronizationStatus resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# synchronizationStatus resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|synchronizationStatusCode|**TODO: Add Description**. Possible values are: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.|
|countSuccessiveCompleteFailures|Int64|**TODO: Add Description**|
|escrowsPruned|Boolean|**TODO: Add Description**|
|lastExecution|[synchronizationTaskExecution](../resources/synchronizationtaskexecution.md)|**TODO: Add Description**|
|lastSuccessfulExecution|[synchronizationTaskExecution](../resources/synchronizationtaskexecution.md)|**TODO: Add Description**|
|lastSuccessfulExecutionWithExports|[synchronizationTaskExecution](../resources/synchronizationtaskexecution.md)|**TODO: Add Description**|
|progress|[synchronizationProgress](../resources/synchronizationprogress.md) collection|**TODO: Add Description**|
|quarantine|[synchronizationQuarantine](../resources/synchronizationquarantine.md)|**TODO: Add Description**|
|steadyStateFirstAchievedTime|DateTimeOffset|**TODO: Add Description**|
|steadyStateLastAchievedTime|DateTimeOffset|**TODO: Add Description**|
|synchronizedEntryCountByType|[stringKeyLongValuePair](../resources/stringkeylongvaluepair.md) collection|**TODO: Add Description**|
|troubleshootingUrl|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationStatus",
  "countSuccessiveCompleteFailures": "Integer",
  "escrowsPruned": "Boolean",
  "code": "String",
  "lastExecution": {
    "@odata.type": "microsoft.graph.synchronizationTaskExecution"
  },
  "lastSuccessfulExecution": {
    "@odata.type": "microsoft.graph.synchronizationTaskExecution"
  },
  "lastSuccessfulExecutionWithExports": {
    "@odata.type": "microsoft.graph.synchronizationTaskExecution"
  },
  "progress": [
    {
      "@odata.type": "microsoft.graph.synchronizationProgress"
    }
  ],
  "quarantine": {
    "@odata.type": "microsoft.graph.synchronizationQuarantine"
  },
  "steadyStateFirstAchievedTime": "String (timestamp)",
  "steadyStateLastAchievedTime": "String (timestamp)",
  "synchronizedEntryCountByType": [
    {
      "@odata.type": "microsoft.graph.stringKeyLongValuePair"
    }
  ],
  "troubleshootingUrl": "String"
}
```

