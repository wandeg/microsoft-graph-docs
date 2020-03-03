---
title: "persistentBrowserSessionControl resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# persistentBrowserSessionControl resource type




Inherits from [conditionalAccessSessionControl](../resources/conditionalAccessSessionControl.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|isEnabled|Boolean| Inherited from [conditionalAccessSessionControl](../resources/conditionalAccessSessionControl.md)|
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

