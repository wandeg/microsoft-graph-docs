---
title: "conditionalAccessGrantControls resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# conditionalAccessGrantControls resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|builtInControls|Enumeration collection||
|customAuthenticationFactors|String collection||
|operator|String||
|termsOfUse|String collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conditionalAccessGrantControls"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conditionalAccessGrantControls",
  "operator": "String",
  "builtInControls": [
    "String"
  ],
  "customAuthenticationFactors": [
    "String"
  ],
  "termsOfUse": [
    "String"
  ]
}
```

