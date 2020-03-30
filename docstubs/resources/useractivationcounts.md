---
title: "userActivationCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userActivationCounts resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|activatedOnSharedComputer|Boolean||
|android|Int64||
|ios|Int64||
|lastActivatedDate|Date||
|mac|Int64||
|productType|String||
|windows|Int64||
|windows10Mobile|Int64||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userActivationCounts"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userActivationCounts",
  "productType": "String",
  "lastActivatedDate": "Date",
  "windows": 1024,
  "mac": 1024,
  "windows10Mobile": 1024,
  "ios": 1024,
  "android": 1024,
  "activatedOnSharedComputer": true
}
```

