---
title: "securityActionState resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# securityActionState resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|appId|String||
|status|Enumeration|. Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|updatedDateTime|DateTimeOffset||
|user|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.securityActionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityActionState",
  "appId": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

