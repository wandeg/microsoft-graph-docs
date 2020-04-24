---
title: "synchronizationJob resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# synchronizationJob resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get synchronizationJob](../api/synchronizationjob-get.md)|[synchronizationJob](../resources/synchronizationjob.md)|Read the properties and relationships of a [synchronizationJob](../resources/synchronizationjob.md) object.|
|[Update synchronizationJob](../api/synchronizationjob-update.md)|[synchronizationJob](../resources/synchronizationjob.md)|Update the properties of a [synchronizationJob](../resources/synchronizationjob.md) object.|
|[pause](../api/synchronizationjob-pause.md)|None|**TODO: Add Description**|
|[start](../api/synchronizationjob-start.md)|None|**TODO: Add Description**|
|[stop](../api/synchronizationjob-stop.md)|None|**TODO: Add Description**|
|[apply](../api/synchronizationjob-apply.md)|None|**TODO: Add Description**|
|[restart](../api/synchronizationjob-restart.md)|None|**TODO: Add Description**|
|[validateCredentials](../api/synchronizationjob-validatecredentials.md)|None|**TODO: Add Description**|
|[validateCredentials](../api/synchronizationjob-validatecredentials.md)|None|**TODO: Add Description**|
|[List schema](../api/synchronizationjob-list-schema.md)|[synchronizationSchema](../resources/synchronizationschema.md) collection|Get the synchronizationSchemas from the schema navigation property.|
|[Create schema](../api/synchronizationjob-post-schema.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Create a new schema object.|
|[Delete schema](../api/synchronizationjob-delete-schema.md)|None|Delete a [synchronizationSchema](../resources/synchronizationschema.md) object.|
|[Update schema](../api/synchronizationjob-update-schema.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Update the properties of a schema object.|
|[Get synchronizationSchema](../api/synchronizationschema-get.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Read the properties and relationships of a [synchronizationSchema](../resources/synchronizationschema.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|schedule|[synchronizationSchedule](../resources/synchronizationschedule.md)|**TODO: Add Description**|
|status|[synchronizationStatus](../resources/synchronizationstatus.md)|**TODO: Add Description**|
|synchronizationJobSettings|[keyValuePair](../resources/keyvaluepair.md) collection|**TODO: Add Description**|
|templateId|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|schema|[synchronizationSchema](../resources/synchronizationschema.md)|**TODO: Add Description**|

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

