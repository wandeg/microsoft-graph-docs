---
title: "protectGroup resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# protectGroup resource type


Namespace: microsoft.graph




Inherits from [labelActionBase](../resources/labelactionbase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowEmailFromGuestUsers|Boolean||
|allowGuestUsers|Boolean||
|name|String| Inherited from [labelActionBase](../resources/labelactionbase.md)|
|privacy|Enumeration|. Possible values are: `public`, `private`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.protectGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.protectGroup",
  "name": "String",
  "allowEmailFromGuestUsers": true,
  "allowGuestUsers": true,
  "privacy": "String"
}
```

