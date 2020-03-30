---
title: "windows10VpnProxyServer resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windows10VpnProxyServer resource type


Namespace: microsoft.graph




Inherits from [vpnProxyServer](../resources/vpnproxyserver.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|String| Inherited from [vpnProxyServer](../resources/vpnproxyserver.md)|
|automaticConfigurationScriptUrl|String| Inherited from [vpnProxyServer](../resources/vpnproxyserver.md)|
|bypassProxyServerForLocalAddress|Boolean||
|port|Int32| Inherited from [vpnProxyServer](../resources/vpnproxyserver.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "bypassProxyServerForLocalAddress": true
}
```

