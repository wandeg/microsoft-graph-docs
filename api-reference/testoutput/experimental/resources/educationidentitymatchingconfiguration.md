---
title: "educationIdentityMatchingConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationIdentityMatchingConfiguration resource type


Namespace: microsoft.graph




Inherits from [educationIdentitySynchronizationConfiguration](../resources/educationidentitysynchronizationconfiguration.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|matchingOptions|[educationIdentityMatchingOptions](../resources/educationidentitymatchingoptions.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationIdentityMatchingConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationIdentityMatchingConfiguration",
  "matchingOptions": [
    {
      "@odata.type": "microsoft.graph.educationIdentityMatchingOptions",
      "appliesTo": "String",
      "sourcePropertyName": "String",
      "targetPropertyName": "String",
      "targetDomain": "String"
    }
  ]
}
```

