---
title: "encryptContent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# encryptContent resource type




Inherits from [labelActionBase](../resources/labelActionBase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|encryptWith|Enumeration|. Possible values are: `template`, `userDefinedRights`.|
|name|String| Inherited from [labelActionBase](../resources/labelActionBase.md)|

## Relationships
None

## JSON Representation
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

