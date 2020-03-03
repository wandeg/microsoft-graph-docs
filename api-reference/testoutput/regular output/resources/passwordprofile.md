---
title: "passwordProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# passwordProfile resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|forceChangePasswordNextSignIn|Boolean||
|forceChangePasswordNextSignInWithMfa|Boolean||
|password|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.passwordProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordProfile",
  "password": "String",
  "forceChangePasswordNextSignIn": true,
  "forceChangePasswordNextSignInWithMfa": true
}
```

