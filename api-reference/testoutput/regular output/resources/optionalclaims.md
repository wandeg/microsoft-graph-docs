---
title: "optionalClaims resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# optionalClaims resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessToken|[optionalClaim](../resources/optionalClaim.md) collection||
|idToken|[optionalClaim](../resources/optionalClaim.md) collection||
|saml2Token|[optionalClaim](../resources/optionalClaim.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.optionalClaims"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.optionalClaims",
  "idToken": [
    {
      "@odata.type": "microsoft.graph.optionalClaim",
      "name": "String",
      "source": "String",
      "essential": true,
      "additionalProperties": [
        "String"
      ]
    }
  ],
  "accessToken": [
    {
      "@odata.type": "microsoft.graph.optionalClaim"
    }
  ],
  "saml2Token": [
    {
      "@odata.type": "microsoft.graph.optionalClaim"
    }
  ]
}
```

