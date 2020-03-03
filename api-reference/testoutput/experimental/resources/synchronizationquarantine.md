---
title: "synchronizationQuarantine resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# synchronizationQuarantine resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|currentBegan|DateTimeOffset||
|nextAttempt|DateTimeOffset||
|reason|Enumeration|. Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`, `QuarantinedOnDemand`, `TooManyDeletes`.|
|seriesBegan|DateTimeOffset||
|seriesCount|Int64||

## Relationships
None

## JSON Representation
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
  "seriesBegan": "String (timestamp)",
  "seriesCount": 1024
}
```

