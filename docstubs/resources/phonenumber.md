---
title: "PhoneNumber resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# PhoneNumber resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|extension|String||
|number|String||
|type|Enumeration| Possible values are: `WORK`, `HOME`, `MOBILE`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.PhoneNumber"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.PhoneNumber",
  "number": "String",
  "extension": "String",
  "type": "String"
}
```

