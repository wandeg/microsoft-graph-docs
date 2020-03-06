---
title: "windows81VpnProxyServer resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windows81VpnProxyServer resource type


Namespace: microsoft.graph




Inherits from [vpnProxyServer](../resources/vpnproxyserver.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|String|Address. Inherited from [vpnProxyServer](../resources/vpnproxyserver.md)|
|automaticallyDetectProxySettings|Boolean|Automatically detect proxy settings.|
|automaticConfigurationScriptUrl|String|Proxy's automatic configuration script url. Inherited from [vpnProxyServer](../resources/vpnproxyserver.md)|
|bypassProxyServerForLocalAddress|Boolean|Bypass proxy server for local address.|
|port|Int32|Port. Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/vpnproxyserver.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows81VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "automaticallyDetectProxySettings": true,
  "bypassProxyServerForLocalAddress": true
}
```

