---
title: "synchronizationTaskExecution resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# synchronizationTaskExecution resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activityIdentifier|String|**TODO: Add Description**|
|countEntitled|Int64|**TODO: Add Description**|
|countEntitledForProvisioning|Int64|**TODO: Add Description**|
|countEscrowed|Int64|**TODO: Add Description**|
|countEscrowedRaw|Int64|**TODO: Add Description**|
|countExported|Int64|**TODO: Add Description**|
|countExports|Int64|**TODO: Add Description**|
|countImported|Int64|**TODO: Add Description**|
|countImportedDeltas|Int64|**TODO: Add Description**|
|countImportedReferenceDeltas|Int64|**TODO: Add Description**|
|error|[synchronizationError](../resources/synchronizationerror.md)|**TODO: Add Description**|
|state|synchronizationTaskExecutionResult|**TODO: Add Description**. Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.|
|timeBegan|DateTimeOffset|**TODO: Add Description**|
|timeEnded|DateTimeOffset|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationTaskExecution"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationTaskExecution",
  "activityIdentifier": "String",
  "countEntitled": "Integer",
  "countEntitledForProvisioning": "Integer",
  "countEscrowed": "Integer",
  "countEscrowedRaw": "Integer",
  "countExported": "Integer",
  "countExports": "Integer",
  "countImported": "Integer",
  "countImportedDeltas": "Integer",
  "countImportedReferenceDeltas": "Integer",
  "state": "String",
  "error": {
    "@odata.type": "microsoft.graph.synchronizationError"
  },
  "timeBegan": "String (timestamp)",
  "timeEnded": "String (timestamp)"
}
```

