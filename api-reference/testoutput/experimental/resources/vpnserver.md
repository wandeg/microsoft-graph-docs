---
title: "vpnServer resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# vpnServer resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|String|Address (IP address, FQDN or URL)|
|description|String|Description.|
|isDefaultServer|Boolean|Default server.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnServer",
  "description": "String",
  "address": "String",
  "isDefaultServer": true
}
```

