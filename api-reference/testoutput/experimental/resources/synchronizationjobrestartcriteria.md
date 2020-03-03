---
title: "synchronizationJobRestartCriteria resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# synchronizationJobRestartCriteria resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|resetScope|Enumeration|. Possible values are: `ForceDeletes`, `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`, `None`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationJobRestartCriteria",
  "resetScope": "String"
}
```

