---
title: "initiator resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# initiator resource type


Namespace: Microsoft.AAD.Reporting



## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String||
|initiatorType|Enumeration| Possible values are: `user`, `app`, `system`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.AAD.Reporting.initiator"
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.initiator",
  "id": "String (identifier)",
  "displayName": "String",
  "initiatorType": "String"
}
```

