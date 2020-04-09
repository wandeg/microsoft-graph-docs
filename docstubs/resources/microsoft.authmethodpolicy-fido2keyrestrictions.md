---
title: "fido2KeyRestrictions resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# fido2KeyRestrictions resource type


Namespace: microsoft.authMethodPolicy



## Properties
|Property|Type|Description|
|:---|:---|:---|
|aaGuids|String collection||
|enforcementType|Enumeration| Possible values are: `allow`, `block`, `unknownFutureValue`.|
|isEnforced|Boolean||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.authMethodPolicy.fido2KeyRestrictions"
}
-->
``` json
{
  "@odata.type": "#microsoft.authMethodPolicy.fido2KeyRestrictions",
  "isEnforced": true,
  "enforcementType": "String",
  "aaGuids": [
    "String"
  ]
}
```

