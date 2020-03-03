---
title: "attributeDefinition resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# attributeDefinition resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|anchor|Boolean||
|apiExpressions|[stringKeyStringValuePair](../resources/stringKeyStringValuePair.md) collection||
|caseExact|Boolean||
|defaultValue|String||
|metadata|[metadataEntry](../resources/metadataEntry.md) collection||
|multivalued|Boolean||
|mutability|Enumeration|. Possible values are: `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.|
|name|String||
|referencedObjects|[referencedObject](../resources/referencedObject.md) collection||
|required|Boolean||
|type|Enumeration|. Possible values are: `DateTime`, `Boolean`, `Binary`, `Reference`, `Integer`, `String`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attributeDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attributeDefinition",
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
```

