---
title: "acl resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# acl resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessType|Enumeration|. Possible values are: `grant`, `deny`.|
|identitySource|String||
|type|Enumeration|. Possible values are: `user`, `group`, `everyone`, `everyoneExceptGuests`.|
|value|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.acl"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.acl",
  "type": "String",
  "value": "String",
  "accessType": "String",
  "identitySource": "String"
}
```

