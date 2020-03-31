---
title: "appleVpnAlwaysOnConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# appleVpnAlwaysOnConfiguration resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|airPrintExceptionAction|Enumeration| Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|
|allowAllCaptiveNetworkPlugins|Boolean||
|allowCaptiveWebSheet|Boolean||
|allowedCaptiveNetworkPlugins|[specifiedCaptiveNetworkPlugins](../resources/specifiedcaptivenetworkplugins.md)||
|cellularExceptionAction|Enumeration| Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|
|natKeepAliveIntervalInSeconds|Int32||
|natKeepAliveOffloadEnable|Boolean||
|tunnelConfiguration|Enumeration| Possible values are: `wifiAndCellular`, `cellular`, `wifi`.|
|userToggleEnabled|Boolean||
|voicemailExceptionAction|Enumeration| Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|

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

