---
title: "classifcationErrorBase resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# classifcationErrorBase resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String|**TODO: Add Description**|
|innerError|[classificationInnerError](../resources/classificationinnererror.md)|**TODO: Add Description**|
|message|String|**TODO: Add Description**|
|target|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

