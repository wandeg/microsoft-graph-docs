---
title: "passwordProfile resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# passwordProfile resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|forceChangePasswordNextSignIn|Boolean|**TODO: Add Description**|
|forceChangePasswordNextSignInWithMfa|Boolean|**TODO: Add Description**|
|password|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.DirectoryServices.passwordProfile"
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.passwordProfile",
  "password": "String",
  "forceChangePasswordNextSignIn": true,
  "forceChangePasswordNextSignInWithMfa": true
}
```

