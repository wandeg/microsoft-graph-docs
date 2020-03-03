---
title: "responseStatus resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# responseStatus resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|response|Enumeration|. Possible values are: `none`, `organizer`, `tentativelyAccepted`, `accepted`, `declined`, `notResponded`.|
|time|DateTimeOffset||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
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

