---
title: "responseStatus resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# responseStatus resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|response|responseType|**TODO: Add Description**. Possible values are: `none`, `organizer`, `tentativelyAccepted`, `accepted`, `declined`, `notResponded`.|
|time|DateTimeOffset|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.responseStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.responseStatus",
  "response": "String",
  "time": "String (timestamp)"
}
```

