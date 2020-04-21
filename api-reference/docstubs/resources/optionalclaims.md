---
title: "optionalClaims resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# optionalClaims resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessToken|[optionalClaim](../resources/optionalclaim.md) collection|**TODO: Add Description**|
|idToken|[optionalClaim](../resources/optionalclaim.md) collection|**TODO: Add Description**|
|saml2Token|[optionalClaim](../resources/optionalclaim.md) collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

