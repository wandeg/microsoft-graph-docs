---
title: "educationIdentityMatchingOptions resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationIdentityMatchingOptions resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|appliesTo|Enumeration| Possible values are: `student`, `teacher`, `none`, `unknownFutureValue`, `faculty`.|
|sourcePropertyName|String||
|targetDomain|String||
|targetPropertyName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationIdentityMatchingOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationIdentityMatchingOptions",
  "appliesTo": "String",
  "sourcePropertyName": "String",
  "targetPropertyName": "String",
  "targetDomain": "String"
}
```

