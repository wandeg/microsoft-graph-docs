---
title: "synchronizationStatus resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# synchronizationStatus resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|Enumeration|. Possible values are: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.|
|countSuccessiveCompleteFailures|Int64||
|escrowsPruned|Boolean||
|lastExecution|[synchronizationTaskExecution](../resources/synchronizationtaskexecution.md)||
|lastSuccessfulExecution|[synchronizationTaskExecution](../resources/synchronizationtaskexecution.md)||
|lastSuccessfulExecutionWithExports|[synchronizationTaskExecution](../resources/synchronizationtaskexecution.md)||
|progress|[synchronizationProgress](../resources/synchronizationprogress.md) collection||
|quarantine|[synchronizationQuarantine](../resources/synchronizationquarantine.md)||
|steadyStateFirstAchievedTime|DateTimeOffset||
|steadyStateLastAchievedTime|DateTimeOffset||
|synchronizedEntryCountByType|[stringKeyLongValuePair](../resources/stringkeylongvaluepair.md) collection||
|troubleshootingUrl|String||

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

