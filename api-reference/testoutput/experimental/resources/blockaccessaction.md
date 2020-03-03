---
title: "blockAccessAction resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# blockAccessAction resource type


Namespace: microsoft.graph




Inherits from [dlpActionInfo](../resources/dlpactioninfo.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|Enumeration| Inherited from [dlpActionInfo](../resources/dlpactioninfo.md). Possible values are: `notifyUser`, `blockAccess`, `deviceRestriction`.|

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

