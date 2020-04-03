---
title: "vpnTrafficRule resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# vpnTrafficRule resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|appId|String||
|appType|Enumeration| Possible values are: `none`, `desktop`, `universal`.|
|claims|String||
|localAddressRanges|[iPv4Range](../resources/ipv4range.md) collection||
|localPortRanges|[numberRange](../resources/numberrange.md) collection||
|name|String||
|protocols|Int32||
|remoteAddressRanges|[iPv4Range](../resources/ipv4range.md) collection||
|remotePortRanges|[numberRange](../resources/numberrange.md) collection||
|routingPolicyType|Enumeration| Possible values are: `none`, `splitTunnel`, `forceTunnel`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnTrafficRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnTrafficRule",
  "name": "String",
  "protocols": 1024,
  "localPortRanges": [
    {
      "@odata.type": "microsoft.graph.numberRange",
      "lowerNumber": 1024,
      "upperNumber": 1024
    }
  ],
  "remotePortRanges": [
    {
      "@odata.type": "microsoft.graph.numberRange"
    }
  ],
  "localAddressRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "remoteAddressRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4Range"
    }
  ],
  "appId": "String",
  "appType": "String",
  "routingPolicyType": "String",
  "claims": "String"
}
```

