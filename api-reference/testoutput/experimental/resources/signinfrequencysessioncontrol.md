---
title: "signInFrequencySessionControl resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# signInFrequencySessionControl resource type


Namespace: microsoft.graph




Inherits from [conditionalAccessSessionControl](../resources/conditionalaccesssessioncontrol.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|isEnabled|Boolean| Inherited from [conditionalAccessSessionControl](../resources/conditionalaccesssessioncontrol.md)|
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

