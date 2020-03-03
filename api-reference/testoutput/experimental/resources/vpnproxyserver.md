---
title: "vpnProxyServer resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# vpnProxyServer resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|String|Address.|
|automaticConfigurationScriptUrl|String|Proxy's automatic configuration script url.|
|port|Int32|Port. Valid values 0 to 65535|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024
}
```

