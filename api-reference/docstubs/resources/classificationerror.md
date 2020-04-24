---
title: "classificationError resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# classificationError resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [classifcationErrorBase](../resources/classifcationerrorbase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String|**TODO: Add Description** Inherited from [classifcationErrorBase](../resources/classifcationerrorbase.md)|
|details|[classifcationErrorBase](../resources/classifcationerrorbase.md) collection|**TODO: Add Description**|
|innerError|[classificationInnerError](../resources/classificationinnererror.md)|**TODO: Add Description** Inherited from [classifcationErrorBase](../resources/classifcationerrorbase.md)|
|message|String|**TODO: Add Description** Inherited from [classifcationErrorBase](../resources/classifcationerrorbase.md)|
|target|String|**TODO: Add Description** Inherited from [classifcationErrorBase](../resources/classifcationerrorbase.md)|

## Relationships
None

## JSON representation
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

