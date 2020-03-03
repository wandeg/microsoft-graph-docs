---
title: "classificationError resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# classificationError resource type




Inherits from [classifcationErrorBase](../resources/classifcationErrorBase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String| Inherited from [classifcationErrorBase](../resources/classifcationErrorBase.md)|
|details|[classifcationErrorBase](../resources/classifcationErrorBase.md) collection||
|innerError|[classificationInnerError](../resources/classificationInnerError.md)| Inherited from [classifcationErrorBase](../resources/classifcationErrorBase.md)|
|message|String| Inherited from [classifcationErrorBase](../resources/classifcationErrorBase.md)|
|target|String| Inherited from [classifcationErrorBase](../resources/classifcationErrorBase.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.classificationError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.classificationError",
  "code": "String",
  "message": "String",
  "target": "String",
  "innerError": {
    "@odata.type": "microsoft.graph.classificationInnerError",
    "errorDateTime": "String (timestamp)",
    "clientRequestId": "String",
    "activityId": "String"
  },
  "details": [
    {
      "@odata.type": "microsoft.graph.classifcationErrorBase"
    }
  ]
}
```

