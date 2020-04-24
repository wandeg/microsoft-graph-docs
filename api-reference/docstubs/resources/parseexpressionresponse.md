---
title: "parseExpressionResponse resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# parseExpressionResponse resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|error|[publicError](../resources/publicerror.md)|**TODO: Add Description**|
|evaluationResult|String collection|**TODO: Add Description**|
|evaluationSucceeded|Boolean|**TODO: Add Description**|
|parsedExpression|[attributeMappingSource](../resources/attributemappingsource.md)|**TODO: Add Description**|
|parsingSucceeded|Boolean|**TODO: Add Description**|

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

