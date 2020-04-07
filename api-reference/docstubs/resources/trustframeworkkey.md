---
title: "trustFrameworkKey resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# trustFrameworkKey resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|d|String||
|dp|String||
|dq|String||
|e|String||
|exp|Int64||
|k|String||
|kid|String||
|kty|String||
|n|String||
|nbf|Int64||
|p|String||
|q|String||
|qi|String||
|use|String||
|x5c|String collection||
|x5t|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.trustFrameworkKey"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.trustFrameworkKey",
  "k": "String",
  "x5c": [
    "String"
  ],
  "x5t": "String",
  "kty": "String",
  "use": "String",
  "exp": 1024,
  "nbf": 1024,
  "kid": "String",
  "e": "String",
  "n": "String",
  "d": "String",
  "p": "String",
  "q": "String",
  "dp": "String",
  "dq": "String",
  "qi": "String"
}
```

