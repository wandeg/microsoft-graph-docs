---
title: "educationIdentityDomain resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationIdentityDomain resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|appliesTo|Enumeration|. Possible values are: `student`, `teacher`, `none`, `unknownFutureValue`, `faculty`.|
|name|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationIdentityDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationIdentityDomain",
  "appliesTo": "String",
  "name": "String"
}
```

