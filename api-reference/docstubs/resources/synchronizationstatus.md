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
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationStatus",
  "countSuccessiveCompleteFailures": 1024,
  "escrowsPruned": true,
  "code": "String",
  "lastExecution": {
    "@odata.type": "microsoft.graph.synchronizationTaskExecution",
    "activityIdentifier": "String",
    "countEntitled": 1024,
    "countEntitledForProvisioning": 1024,
    "countEscrowed": 1024,
    "countEscrowedRaw": 1024,
    "countExported": 1024,
    "countExports": 1024,
    "countImported": 1024,
    "countImportedDeltas": 1024,
    "countImportedReferenceDeltas": 1024,
    "state": "String",
    "error": {
      "@odata.type": "microsoft.graph.synchronizationError",
      "code": "String",
      "message": "String",
      "tenantActionable": true
    },
    "timeBegan": "String (timestamp)",
    "timeEnded": "String (timestamp)"
  },
  "lastSuccessfulExecution": {
    "@odata.type": "microsoft.graph.synchronizationTaskExecution"
  },
  "lastSuccessfulExecutionWithExports": {
    "@odata.type": "microsoft.graph.synchronizationTaskExecution"
  },
  "progress": [
    {
      "@odata.type": "microsoft.graph.synchronizationProgress",
      "completedUnits": 1024,
      "progressObservationDateTime": "String (timestamp)",
      "totalUnits": 1024,
      "units": "String"
    }
  ],
  "quarantine": {
    "@odata.type": "microsoft.graph.synchronizationQuarantine",
    "currentBegan": "String (timestamp)",
    "nextAttempt": "String (timestamp)",
    "reason": "String",
    "seriesBegan": "String (timestamp)",
    "seriesCount": 1024
  },
  "steadyStateFirstAchievedTime": "String (timestamp)",
  "steadyStateLastAchievedTime": "String (timestamp)",
  "synchronizedEntryCountByType": [
    {
      "@odata.type": "microsoft.graph.stringKeyLongValuePair",
      "key": "String",
      "value": 1024
    }
  ],
  "troubleshootingUrl": "String"
}
```

