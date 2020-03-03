---
title: "synchronizationTaskExecution resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# synchronizationTaskExecution resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|activityIdentifier|String||
|countEntitled|Int64||
|countEntitledForProvisioning|Int64||
|countEscrowed|Int64||
|countEscrowedRaw|Int64||
|countExported|Int64||
|countExports|Int64||
|countImported|Int64||
|countImportedDeltas|Int64||
|countImportedReferenceDeltas|Int64||
|error|[synchronizationError](../resources/synchronizationError.md)||
|state|Enumeration|. Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.|
|timeBegan|DateTimeOffset||
|timeEnded|DateTimeOffset||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationTaskExecution"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationTaskExecution",
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
}
```

