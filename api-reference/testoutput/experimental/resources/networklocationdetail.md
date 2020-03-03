---
title: "networkLocationDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# networkLocationDetail resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|networkNames|String collection||
|networkType|Enumeration|. Possible values are: `intranet`, `extranet`, `namedNetwork`, `trusted`, `unknownFutureValue`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.networkLocationDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkLocationDetail",
  "networkType": "String",
  "networkNames": [
    "String"
  ]
}
```

