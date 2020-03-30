---
title: "iosCredentialSingleSignOnExtension resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosCredentialSingleSignOnExtension resource type


Namespace: microsoft.graph




Inherits from [iosSingleSignOnExtension](../resources/iossinglesignonextension.md)

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
  "@odata.type": "microsoft.graph.iosCredentialSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosCredentialSingleSignOnExtension",
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

