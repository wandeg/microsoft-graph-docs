---
title: "DecoratedProfileBatchGetResult resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# DecoratedProfileBatchGetResult resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|errors|[ErrorMapElement](../resources/errormapelement.md) collection|**TODO: Add Description**|
|results|[DecoratedProfileMapElement](../resources/decoratedprofilemapelement.md) collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.DecoratedProfileBatchGetResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.DecoratedProfileBatchGetResult",
  "errors": [
    {
      "@odata.type": "microsoft.graph.ErrorMapElement"
    }
  ],
  "results": [
    {
      "@odata.type": "microsoft.graph.DecoratedProfileMapElement"
    }
  ]
}
```

