---
title: "errorDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# errorDetail resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|details|[innerErrorDetail](../resources/innerErrorDetail.md) collection||
|errorCode|String||
|message|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.errorDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.errorDetail",
  "errorCode": "String",
  "message": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.innerErrorDetail",
      "source": "String"
    }
  ]
}
```

