---
title: "objectIdentity resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# objectIdentity resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|issuer|String||
|issuerAssignedId|String||
|signInType|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.objectIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.objectIdentity",
  "signInType": "String",
  "issuer": "String",
  "issuerAssignedId": "String"
}
```

