---
title: "persistentBrowserSessionControl resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# persistentBrowserSessionControl resource type


Namespace: microsoft.graph




Inherits from [conditionalAccessSessionControl](../resources/conditionalaccesssessioncontrol.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|isEnabled|Boolean| Inherited from [conditionalAccessSessionControl](../resources/conditionalaccesssessioncontrol.md)|
|mode|Enumeration|. Possible values are: `always`, `never`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.persistentBrowserSessionControl"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.persistentBrowserSessionControl",
  "isEnabled": true,
  "mode": "String"
}
```

