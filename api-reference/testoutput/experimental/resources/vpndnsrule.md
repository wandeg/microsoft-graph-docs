---
title: "vpnDnsRule resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# vpnDnsRule resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|autoTrigger|Boolean|Automatically connect to the VPN when the device connects to this domain: Default False.|
|name|String|Name.|
|persistent|Boolean|Keep this rule active even when the VPN is not connected: Default False|
|proxyServerUri|String|Proxy Server Uri.|
|servers|String collection|Servers.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnDnsRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnDnsRule",
  "name": "String",
  "servers": [
    "String"
  ],
  "proxyServerUri": "String",
  "autoTrigger": true,
  "persistent": true
}
```

