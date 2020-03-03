---
title: "blockAccessAction resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# blockAccessAction resource type




Inherits from [dlpActionInfo](../resources/dlpActionInfo.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|Enumeration| Inherited from [dlpActionInfo](../resources/dlpActionInfo.md). Possible values are: `notifyUser`, `blockAccess`, `deviceRestriction`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.blockAccessAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.blockAccessAction",
  "action": "String"
}
```

