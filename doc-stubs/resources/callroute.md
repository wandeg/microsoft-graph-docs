---
title: "callRoute resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# callRoute resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|final|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|original|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|routingType|routingType|**TODO: Add Description**. Possible values are: `forwarded`, `lookup`, `selfFork`, `unknownFutureValue`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRoute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRoute",
  "routingType": "String",
  "original": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "final": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

