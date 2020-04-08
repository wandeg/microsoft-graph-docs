---
title: "linkedInStatus resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# linkedInStatus resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|scopes|String||
|value|Enumeration| Possible values are: `Unbound`, `Bound`, `OptOut`, `DisableBound`, `LinkedInBound`, `MicrosoftBound`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.linkedInStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.linkedInStatus",
  "value": "String",
  "scopes": "String"
}
```

