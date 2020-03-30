---
title: "macOSRedirectSingleSignOnExtension resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# macOSRedirectSingleSignOnExtension resource type


Namespace: microsoft.graph




Inherits from [macOSSingleSignOnExtension](../resources/macossinglesignonextension.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configurations|[keyTypedValuePair](../resources/keytypedvaluepair.md) collection||
|extensionIdentifier|String||
|teamIdentifier|String||
|urlPrefixes|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSRedirectSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSRedirectSingleSignOnExtension",
  "extensionIdentifier": "String",
  "teamIdentifier": "String",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyStringValuePair",
      "key": "String",
      "value": "String"
    }
  ],
  "urlPrefixes": [
    "String"
  ]
}
```

