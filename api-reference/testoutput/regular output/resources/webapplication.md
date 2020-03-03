---
title: "webApplication resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# webApplication resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|homePageUrl|String||
|implicitGrantSettings|[implicitGrantSettings](../resources/implicitGrantSettings.md)||
|logoutUrl|String||
|redirectUris|String collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.webApplication"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.webApplication",
  "homePageUrl": "String",
  "redirectUris": [
    "String"
  ],
  "logoutUrl": "String",
  "implicitGrantSettings": {
    "@odata.type": "microsoft.graph.implicitGrantSettings",
    "enableIdTokenIssuance": true,
    "enableAccessTokenIssuance": true
  }
}
```

