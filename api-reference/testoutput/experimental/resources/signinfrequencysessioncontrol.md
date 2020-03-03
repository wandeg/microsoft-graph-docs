---
title: "signInFrequencySessionControl resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# signInFrequencySessionControl resource type




Inherits from [conditionalAccessSessionControl](../resources/conditionalAccessSessionControl.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|isEnabled|Boolean| Inherited from [conditionalAccessSessionControl](../resources/conditionalAccessSessionControl.md)|
|type|Enumeration|. Possible values are: `days`, `hours`.|
|value|Int32||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.signInFrequencySessionControl"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.signInFrequencySessionControl",
  "isEnabled": true,
  "value": 1024,
  "type": "String"
}
```

