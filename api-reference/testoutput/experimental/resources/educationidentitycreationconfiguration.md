---
title: "educationIdentityCreationConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationIdentityCreationConfiguration resource type


Namespace: microsoft.graph




Inherits from [educationIdentitySynchronizationConfiguration](../resources/educationidentitysynchronizationconfiguration.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|userDomains|[educationIdentityDomain](../resources/educationidentitydomain.md) collection||

## Relationships
None

## JSON representation
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

