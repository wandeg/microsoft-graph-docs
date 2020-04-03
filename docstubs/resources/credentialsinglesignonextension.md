---
title: "credentialSingleSignOnExtension resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# credentialSingleSignOnExtension resource type


Namespace: microsoft.graph




Inherits from [singleSignOnExtension](../resources/singlesignonextension.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configurations|[keyTypedValuePair](../resources/keytypedvaluepair.md) collection||
|domains|String collection||
|extensionIdentifier|String||
|realm|String||
|teamIdentifier|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.credentialSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.credentialSingleSignOnExtension",
  "extensionIdentifier": "String",
  "teamIdentifier": "String",
  "domains": [
    "String"
  ],
  "realm": "String",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyStringValuePair",
      "key": "String",
      "value": "String"
    }
  ]
}
```

