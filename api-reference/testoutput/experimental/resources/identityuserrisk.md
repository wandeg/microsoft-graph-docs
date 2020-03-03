---
title: "identityUserRisk resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# identityUserRisk resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|lastChangedDateTime|DateTimeOffset||
|level|Enumeration|. Possible values are: `unknown`, `none`, `low`, `medium`, `high`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityUserRisk"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.identityUserRisk",
  "level": "String",
  "lastChangedDateTime": "String (timestamp)"
}
```

