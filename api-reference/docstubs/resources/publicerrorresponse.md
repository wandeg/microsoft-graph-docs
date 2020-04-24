---
title: "publicErrorResponse resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# publicErrorResponse resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|error|[publicError](../resources/publicerror.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicErrorResponse"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicErrorResponse",
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
  }
}
```

