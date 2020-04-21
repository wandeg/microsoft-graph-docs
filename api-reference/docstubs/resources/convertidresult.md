---
title: "convertIdResult resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# convertIdResult resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|errorDetails|[genericError](../resources/genericerror.md)|**TODO: Add Description**|
|sourceId|String|**TODO: Add Description**|
|targetId|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.convertIdResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.convertIdResult",
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError",
    "message": "String",
    "code": "String"
  }
}
```

