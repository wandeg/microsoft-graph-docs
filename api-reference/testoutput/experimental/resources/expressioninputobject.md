---
title: "expressionInputObject resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# expressionInputObject resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|definition|[objectDefinition](../resources/objectdefinition.md)||
|properties|[stringKeyObjectValuePair](../resources/stringkeyobjectvaluepair.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.expressionInputObject"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.expressionInputObject",
  "definition": {
    "@odata.type": "microsoft.graph.objectDefinition",
    "attributes": [
      {
        "@odata.type": "microsoft.graph.attributeDefinition",
        "anchor": true,
        "apiExpressions": [
          {
            "@odata.type": "microsoft.graph.stringKeyStringValuePair",
            "key": "String",
            "value": "String"
          }
        ],
        "caseExact": true,
        "defaultValue": "String",
        "metadata": [
          {
            "@odata.type": "microsoft.graph.metadataEntry"
          }
        ],
        "multivalued": true,
        "mutability": "String",
        "name": "String",
        "required": true,
        "referencedObjects": [
          {
            "@odata.type": "microsoft.graph.referencedObject",
            "referencedObjectName": "String",
            "referencedProperty": "String"
          }
        ],
        "type": "String"
      }
    ],
    "supportedApis": [
      "String"
    ]
  },
  "properties": [
    {
      "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
    }
  ]
}
```

