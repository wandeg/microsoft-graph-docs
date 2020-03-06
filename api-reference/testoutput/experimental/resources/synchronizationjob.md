---
title: "synchronizationJob resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# synchronizationJob resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get synchronizationJob](../api/synchronizationjob-get.md)|[synchronizationJob](../resources/synchronizationjob.md)|Read properties and relationships of the [synchronizationJob](../resources/synchronizationjob.md) object.|
|[Update synchronizationJob](../api/synchronizationjob-update.md)|[synchronizationJob](../resources/synchronizationjob.md)|Update the properties of a [synchronizationJob](../resources/synchronizationjob.md) object.|
|[pause](../api/synchronizationjob-pause.md)|None||
|[start](../api/synchronizationjob-start.md)|None||
|[stop](../api/synchronizationjob-stop.md)|None||
|[apply](../api/synchronizationjob-apply.md)|None||
|[restart](../api/synchronizationjob-restart.md)|None||
|[validateCredentials](../api/synchronizationjob-validatecredentials.md)|None||
|[validateCredentials](../api/synchronizationjob-validatecredentials.md)|None||
|[Get synchronizationSchema](../api/synchronizationschema-get.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Read properties and relationships of the [synchronizationSchema](../resources/synchronizationschema.md) object.|
|[List jobs](../api/synchronization-list-jobs.md)|[synchronizationJob](../resources/synchronizationjob.md) collection|Get the synchronizationJobs from the jobs navigation property.|
|[Add jobs](../api/synchronization-post-jobs.md)|[synchronizationJob](../resources/synchronizationjob.md)|Add jobs by posting to the jobs collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|schedule|[synchronizationSchedule](../resources/synchronizationschedule.md)||
|status|[synchronizationStatus](../resources/synchronizationstatus.md)||
|synchronizationJobSettings|[keyValuePair](../resources/keyvaluepair.md) collection||
|templateId|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|schema|[synchronizationSchema](../resources/synchronizationschema.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationJob",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationJob",
  "id": "String (identifier)",
  "templateId": "String",
  "schedule": {
    "@odata.type": "microsoft.graph.synchronizationSchedule",
    "expiration": "String (timestamp)",
    "interval": "String (duration)",
    "state": "String"
  },
  "status": {
    "@odata.type": "microsoft.graph.synchronizationStatus",
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
        "value": 1024
      }
    ],
    "troubleshootingUrl": "String"
  },
  "synchronizationJobSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
}
```

