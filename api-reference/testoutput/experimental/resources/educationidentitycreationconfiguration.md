---
title: "educationIdentityCreationConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# educationIdentityCreationConfiguration resource type




Inherits from [educationIdentitySynchronizationConfiguration](../resources/educationIdentitySynchronizationConfiguration.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|userDomains|[educationIdentityDomain](../resources/educationIdentityDomain.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration",
  "userDomains": [
    {
      "@odata.type": "microsoft.graph.educationIdentityDomain",
      "appliesTo": "String",
      "name": "String"
    }
  ]
}
```

