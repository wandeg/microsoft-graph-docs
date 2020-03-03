---
title: "logonUser resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# logonUser resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountDomain|String||
|accountName|String||
|accountType|Enumeration|. Possible values are: `unknown`, `standard`, `power`, `administrator`, `unknownFutureValue`.|
|firstSeenDateTime|DateTimeOffset||
|lastSeenDateTime|DateTimeOffset||
|logonId|String||
|logonTypes|Enumeration collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.logonUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.logonUser",
  "accountDomain": "String",
  "accountName": "String",
  "accountType": "String",
  "firstSeenDateTime": "String (timestamp)",
  "lastSeenDateTime": "String (timestamp)",
  "logonId": "String",
  "logonTypes": [
    "String"
  ]
}
```

