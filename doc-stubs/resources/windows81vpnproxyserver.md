---
title: "windows81VpnProxyServer resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windows81VpnProxyServer resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [vpnProxyServer](../resources/vpnproxyserver.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|String|**TODO: Add Description** Inherited from [vpnProxyServer](../resources/vpnproxyserver.md)|
|automaticallyDetectProxySettings|Boolean|**TODO: Add Description**|
|automaticConfigurationScriptUrl|String|**TODO: Add Description** Inherited from [vpnProxyServer](../resources/vpnproxyserver.md)|
|bypassProxyServerForLocalAddress|Boolean|**TODO: Add Description**|
|port|Int32|**TODO: Add Description** Inherited from [vpnProxyServer](../resources/vpnproxyserver.md)|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "port": "Integer",
  "automaticallyDetectProxySettings": "Boolean",
  "bypassProxyServerForLocalAddress": "Boolean"
}
```

