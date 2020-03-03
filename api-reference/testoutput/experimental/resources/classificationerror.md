---
title: "classificationError resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# classificationError resource type


Namespace: microsoft.graph




Inherits from [classifcationErrorBase](../resources/classifcationerrorbase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String| Inherited from [classifcationErrorBase](../resources/classifcationerrorbase.md)|
|details|[classifcationErrorBase](../resources/classifcationerrorbase.md) collection||
|innerError|[classificationInnerError](../resources/classificationinnererror.md)| Inherited from [classifcationErrorBase](../resources/classifcationerrorbase.md)|
|message|String| Inherited from [classifcationErrorBase](../resources/classifcationerrorbase.md)|
|target|String| Inherited from [classifcationErrorBase](../resources/classifcationerrorbase.md)|

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

