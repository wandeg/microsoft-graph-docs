---
title: "synchronizationProgress resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# synchronizationProgress resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedUnits|Int64|**TODO: Add Description**|
|progressObservationDateTime|DateTimeOffset|**TODO: Add Description**|
|totalUnits|Int64|**TODO: Add Description**|
|units|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationProgress"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationProgress",
  "completedUnits": "Integer",
  "progressObservationDateTime": "String (timestamp)",
  "totalUnits": "Integer",
  "units": "String"
}
```

