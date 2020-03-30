---
title: "parseExpressionResponse resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# parseExpressionResponse resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|error|[publicError](../resources/publicerror.md)||
|evaluationResult|String collection||
|evaluationSucceeded|Boolean||
|parsedExpression|[attributeMappingSource](../resources/attributemappingsource.md)||
|parsingSucceeded|Boolean||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.parseExpressionResponse"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.parseExpressionResponse",
  "error": {
    "@odata.type": "microsoft.graph.publicError",
    "code": "String",
    "message": "String",
    "target": "String",
    "details": [
      {
        "@odata.type": "microsoft.graph.publicErrorDetail"
      }
    ],
    "innerError": {
      "@odata.type": "microsoft.graph.publicInnerError"
    }
  },
  "evaluationSucceeded": true,
  "evaluationResult": [
    "String"
  ],
  "parsedExpression": {
    "@odata.type": "microsoft.graph.attributeMappingSource",
    "expression": "String",
    "name": "String",
    "parameters": [
      {
        "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair",
        "key": "String",
        "value": {
          "@odata.type": "microsoft.graph.attributeMappingSource",
          "type": "String"
        }
      }
    ]
  },
  "parsingSucceeded": true
}
```

