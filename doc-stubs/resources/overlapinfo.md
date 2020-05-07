---
title: "OverlapInfo resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# OverlapInfo resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|detail|[OverlapInfoDetail](../resources/overlapinfodetail.md)|**TODO: Add Description**|
|overlapType|OverlapType|**TODO: Add Description**. Possible values are: `BOTH_CURRENT_VIEWER_STARTED_FIRST`, `BOTH_CURRENT_VIEWEE_STARTED_FIRST`, `BOTH_CURRENT_STARTED_IN_SAME_MONTH`, `NOT_BOTH_CURRENT_NO_OVERLAP_VIEWER_STARTED_FIRST`, `NOT_BOTH_CURRENT_NO_OVERLAP_VIEWEE_STARTED_FIRST`, `NOT_BOTH_CURRENT_OVERLAP`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.OverlapInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.OverlapInfo",
  "detail": {
    "@odata.type": "microsoft.graph.OverlapInfoDetail"
  },
  "overlapType": "String"
}
```

