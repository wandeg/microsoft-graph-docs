---
title: "typedEmailAddress resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# typedEmailAddress resource type


Namespace: microsoft.graph




Inherits from [emailAddress](../resources/emailaddress.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|String| Inherited from [emailAddress](../resources/emailaddress.md)|
|name|String| Inherited from [emailAddress](../resources/emailaddress.md)|
|otherLabel|String||
|type|Enumeration|. Possible values are: `unknown`, `work`, `personal`, `main`, `other`.|

## Relationships
None

## JSON representation
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

