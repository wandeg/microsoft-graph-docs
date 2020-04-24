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
|airPrintExceptionAction|vpnServiceExceptionAction|Determine whether AirPrint service will be exempt from the always-on VPN connection. Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|
|allowAllCaptiveNetworkPlugins|Boolean|Specifies whether traffic from all captive network plugins should be allowed outside the vpn|
|allowCaptiveWebSheet|Boolean|Determines whether traffic from the Websheet app is allowed outside of the VPN|
|allowedCaptiveNetworkPlugins|[specifiedCaptiveNetworkPlugins](../resources/specifiedcaptivenetworkplugins.md)|Determines whether all, some, or no non-native captive networking apps are allowed|
|cellularExceptionAction|vpnServiceExceptionAction|Determine whether Cellular service will be exempt from the always-on VPN connection. Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|
|natKeepAliveIntervalInSeconds|Int32|Specifies how often in seconds to send a network address translation keepalive package through the VPN|
|natKeepAliveOffloadEnable|Boolean|Enable hardware offloading of NAT keepalive signals when the device is asleep|
|tunnelConfiguration|vpnTunnelConfigurationType|Determines what connections the specific tunnel configuration applies to. Possible values are: `wifiAndCellular`, `cellular`, `wifi`.|
|userToggleEnabled|Boolean|Allow the user to toggle the VPN configuration using the UI|
|voicemailExceptionAction|vpnServiceExceptionAction|Determine whether voicemail service will be exempt from the always-on VPN connection. Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleVpnAlwaysOnConfiguration",
  "tunnelConfiguration": "String",
  "userToggleEnabled": true,
  "voicemailExceptionAction": "String",
  "airPrintExceptionAction": "String",
  "cellularExceptionAction": "String",
  "allowAllCaptiveNetworkPlugins": true,
  "allowedCaptiveNetworkPlugins": {
    "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
    "allowedBundleIdentifiers": [
      "String"
    ]
  },
  "allowCaptiveWebSheet": true,
  "natKeepAliveIntervalInSeconds": 1024,
  "natKeepAliveOffloadEnable": true
}
```

