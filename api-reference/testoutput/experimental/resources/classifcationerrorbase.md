---
title: "classifcationErrorBase resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# classifcationErrorBase resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String||
|innerError|[classificationInnerError](../resources/classificationinnererror.md)||
|message|String||
|target|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.classifcationErrorBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.classifcationErrorBase",
  "code": "String",
  "message": "String",
  "target": "String",
  "innerError": {
    "@odata.type": "microsoft.graph.classificationInnerError",
    "errorDateTime": "String (timestamp)",
    "clientRequestId": "String",
    "activityId": "String"
  }
}
```

