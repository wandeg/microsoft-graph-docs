---
title: "optionalClaims resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# optionalClaims resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessToken|[optionalClaim](../resources/microsoft.directoryservices-optionalclaim.md) collection|**TODO: Add Description**|
|idToken|[optionalClaim](../resources/microsoft.directoryservices-optionalclaim.md) collection|**TODO: Add Description**|
|saml2Token|[optionalClaim](../resources/microsoft.directoryservices-optionalclaim.md) collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.DirectoryServices.optionalClaims"
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.optionalClaims",
  "idToken": [
    {
      "@odata.type": "Microsoft.DirectoryServices.optionalClaim",
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
      "@odata.type": "Microsoft.DirectoryServices.optionalClaim"
    }
  ],
  "saml2Token": [
    {
      "@odata.type": "Microsoft.DirectoryServices.optionalClaim"
    }
  ]
}
```

