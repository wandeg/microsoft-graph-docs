---
title: "appliedConditionalAccessPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# appliedConditionalAccessPolicy resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|enforcedGrantControls|String collection||
|enforcedSessionControls|String collection||
|id|String||
|result|Enumeration|. Possible values are: `success`, `failure`, `notApplied`, `notEnabled`, `unknown`, `unknownFutureValue`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appliedConditionalAccessPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "enforcedGrantControls": [
    "String"
  ],
  "enforcedSessionControls": [
    "String"
  ],
  "result": "String"
}
```

