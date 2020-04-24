---
title: "windows10VpnProxyServer resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windows10VpnProxyServer resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [vpnProxyServer](../resources/vpnproxyserver.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|String|Address. Inherited from [vpnProxyServer](../resources/vpnproxyserver.md)|
|automaticConfigurationScriptUrl|String|Proxy's automatic configuration script url. Inherited from [vpnProxyServer](../resources/vpnproxyserver.md)|
|bypassProxyServerForLocalAddress|Boolean|Bypass proxy server for local address.|
|port|Int32|Port. Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/vpnproxyserver.md)|

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

