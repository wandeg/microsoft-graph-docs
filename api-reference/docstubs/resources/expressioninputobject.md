---
title: "expressionInputObject resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# expressionInputObject resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definition|[objectDefinition](../resources/objectdefinition.md)|**TODO: Add Description**|
|properties|[stringKeyObjectValuePair](../resources/stringkeyobjectvaluepair.md) collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

