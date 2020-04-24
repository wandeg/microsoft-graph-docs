---
title: "vpnTrafficRule resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# vpnTrafficRule resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appId|String|App identifier, if this traffic rule is triggered by an app.|
|appType|vpnTrafficRuleAppType|App type, if this traffic rule is triggered by an app. Possible values are: `none`, `desktop`, `universal`.|
|claims|String|Claims associated with this traffic rule.|
|localAddressRanges|[iPv4Range](../resources/ipv4range.md) collection|Local address range. This collection can contain a maximum of 500 elements.|
|localPortRanges|[numberRange](../resources/numberrange.md) collection|Local port range can be set only when protocol is either TCP or UDP (6 or 17). This collection can contain a maximum of 500 elements.|
|name|String|Name.|
|protocols|Int32|Protocols (0-255). Valid values 0 to 255|
|remoteAddressRanges|[iPv4Range](../resources/ipv4range.md) collection|Remote address range. This collection can contain a maximum of 500 elements.|
|remotePortRanges|[numberRange](../resources/numberrange.md) collection|Remote port range can be set only when protocol is either TCP or UDP (6 or 17). This collection can contain a maximum of 500 elements.|
|routingPolicyType|vpnTrafficRuleRoutingPolicyType|When app triggered, indicates whether to enable split tunneling along this route. Possible values are: `none`, `splitTunnel`, `forceTunnel`.|

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

