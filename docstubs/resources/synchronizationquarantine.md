---
title: "synchronizationQuarantine resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# synchronizationQuarantine resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|currentBegan|DateTimeOffset||
|error|[synchronizationError](../resources/synchronizationerror.md)||
|nextAttempt|DateTimeOffset||
|reason|Enumeration| Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`, `QuarantinedOnDemand`, `TooManyDeletes`.|
|seriesBegan|DateTimeOffset||
|seriesCount|Int64||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationQuarantine"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationQuarantine",
  "currentBegan": "String (timestamp)",
  "nextAttempt": "String (timestamp)",
  "reason": "String",
  "error": {
    "@odata.type": "microsoft.graph.synchronizationError",
    "code": "String",
    "message": "String",
    "tenantActionable": true
  },
  "seriesBegan": "String (timestamp)",
  "seriesCount": 1024
}
```

