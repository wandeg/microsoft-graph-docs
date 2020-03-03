---
title: "typedEmailAddress resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# typedEmailAddress resource type




Inherits from [emailAddress](../resources/emailAddress.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|String| Inherited from [emailAddress](../resources/emailAddress.md)|
|name|String| Inherited from [emailAddress](../resources/emailAddress.md)|
|otherLabel|String||
|type|Enumeration|. Possible values are: `unknown`, `work`, `personal`, `main`, `other`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.typedEmailAddress"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.typedEmailAddress",
  "name": "String",
  "address": "String",
  "type": "String",
  "otherLabel": "String"
}
```

