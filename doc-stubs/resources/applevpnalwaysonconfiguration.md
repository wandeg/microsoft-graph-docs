---
title: "appleVpnAlwaysOnConfiguration resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# appleVpnAlwaysOnConfiguration resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|airPrintExceptionAction|vpnServiceExceptionAction|**TODO: Add Description**. Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|
|allowAllCaptiveNetworkPlugins|Boolean|**TODO: Add Description**|
|allowCaptiveWebSheet|Boolean|**TODO: Add Description**|
|allowedCaptiveNetworkPlugins|[specifiedCaptiveNetworkPlugins](../resources/specifiedcaptivenetworkplugins.md)|**TODO: Add Description**|
|cellularExceptionAction|vpnServiceExceptionAction|**TODO: Add Description**. Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|
|natKeepAliveIntervalInSeconds|Int32|**TODO: Add Description**|
|natKeepAliveOffloadEnable|Boolean|**TODO: Add Description**|
|tunnelConfiguration|vpnTunnelConfigurationType|**TODO: Add Description**. Possible values are: `wifiAndCellular`, `cellular`, `wifi`.|
|userToggleEnabled|Boolean|**TODO: Add Description**|
|voicemailExceptionAction|vpnServiceExceptionAction|**TODO: Add Description**. Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleVpnAlwaysOnConfiguration",
  "tunnelConfiguration": "String",
  "userToggleEnabled": "Boolean",
  "voicemailExceptionAction": "String",
  "airPrintExceptionAction": "String",
  "cellularExceptionAction": "String",
  "allowAllCaptiveNetworkPlugins": "Boolean",
  "allowedCaptiveNetworkPlugins": {
    "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins"
  },
  "allowCaptiveWebSheet": "Boolean",
  "natKeepAliveIntervalInSeconds": "Integer",
  "natKeepAliveOffloadEnable": "Boolean"
}
```

