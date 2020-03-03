---
title: "objectDefinition resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# objectDefinition resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|attributes|[attributeDefinition](../resources/attributeDefinition.md) collection||
|metadata|[metadataEntry](../resources/metadataEntry.md) collection||
|name|String||
|supportedApis|String collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.objectDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.objectDefinition",
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
  "metadata": [
    {
      "@odata.type": "microsoft.graph.metadataEntry"
    }
  ],
  "name": "String",
  "supportedApis": [
    "String"
  ]
}
```

