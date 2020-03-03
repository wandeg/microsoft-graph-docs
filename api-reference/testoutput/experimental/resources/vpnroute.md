---
title: "vpnRoute resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# vpnRoute resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|destinationPrefix|String|Destination prefix (IPv4/v6 address).|
|prefixSize|Int32|Prefix size. (1-32). Valid values 1 to 32|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnRoute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnRoute",
  "destinationPrefix": "String",
  "prefixSize": 1024
}
```

