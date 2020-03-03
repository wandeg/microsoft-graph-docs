---
title: "educationIdentityMatchingConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# educationIdentityMatchingConfiguration resource type




Inherits from [educationIdentitySynchronizationConfiguration](../resources/educationIdentitySynchronizationConfiguration.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|matchingOptions|[educationIdentityMatchingOptions](../resources/educationIdentityMatchingOptions.md) collection||

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

