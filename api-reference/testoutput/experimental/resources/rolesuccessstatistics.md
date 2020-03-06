---
title: "roleSuccessStatistics resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# roleSuccessStatistics resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|permanentFail|Int64||
|permanentSuccess|Int64||
|removeFail|Int64||
|removeSuccess|Int64||
|roleId|String||
|roleName|String||
|temporaryFail|Int64||
|temporarySuccess|Int64||
|unknownFail|Int64||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.roleSuccessStatistics"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleSuccessStatistics",
  "roleId": "String",
  "roleName": "String",
  "temporarySuccess": 1024,
  "temporaryFail": 1024,
  "permanentSuccess": 1024,
  "permanentFail": 1024,
  "removeSuccess": 1024,
  "removeFail": 1024,
  "unknownFail": 1024
}
```

