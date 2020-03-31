---
title: "ErrorMapElement resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# ErrorMapElement resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|key|String||
|value|[Error](../resources/error.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ErrorMapElement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ErrorMapElement",
  "key": "String",
  "value": {
    "@odata.type": "microsoft.graph.Error",
    "status": 1024,
    "message": "String"
  }
}
```

