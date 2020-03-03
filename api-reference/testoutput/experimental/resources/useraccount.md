---
title: "userAccount resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# userAccount resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|lastSeenDateTime|DateTimeOffset||
|riskScore|String||
|service|String||
|signinName|String||
|status|Enumeration|. Possible values are: `unknown`, `staged`, `active`, `suspended`, `deleted`, `unknownFutureValue`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userAccount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAccount",
  "displayName": "String",
  "lastSeenDateTime": "String (timestamp)",
  "riskScore": "String",
  "service": "String",
  "signinName": "String",
  "status": "String"
}
```

