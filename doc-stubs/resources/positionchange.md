---
title: "PositionChange resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# PositionChange resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|newPosition|[Position](../resources/position.md)|**TODO: Add Description**|
|oldPosition|[Position](../resources/position.md)|**TODO: Add Description**|
|positionChangeType|PositionChangeType|**TODO: Add Description**. Possible values are: `PROMOTION`, `COMPANY_CHANGE`, `POSITION_CHANGE`, `ADDITIONAL_POSITION`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.PositionChange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.PositionChange",
  "newPosition": {
    "@odata.type": "microsoft.graph.Position"
  },
  "oldPosition": {
    "@odata.type": "microsoft.graph.Position"
  },
  "positionChangeType": "String"
}
```

