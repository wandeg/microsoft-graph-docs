---
title: "encryptContent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# encryptContent resource type


Namespace: microsoft.graph




Inherits from [labelActionBase](../resources/labelactionbase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|encryptWith|Enumeration| Possible values are: `template`, `userDefinedRights`.|
|name|String| Inherited from [labelActionBase](../resources/labelactionbase.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.encryptContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.encryptContent",
  "name": "String",
  "encryptWith": "String"
}
```

