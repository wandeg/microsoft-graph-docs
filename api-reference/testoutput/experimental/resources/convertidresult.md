---
title: "convertIdResult resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# convertIdResult resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|errorDetails|[genericError](../resources/genericError.md)||
|sourceId|String||
|targetId|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.convertIdResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.convertIdResult",
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError",
    "message": "String",
    "code": "String"
  }
}
```

