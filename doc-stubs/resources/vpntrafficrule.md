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
|appId|String|**TODO: Add Description**|
|appType|vpnTrafficRuleAppType|**TODO: Add Description**. Possible values are: `none`, `desktop`, `universal`.|
|claims|String|**TODO: Add Description**|
|localAddressRanges|[iPv4Range](../resources/ipv4range.md) collection|**TODO: Add Description**|
|localPortRanges|[numberRange](../resources/numberrange.md) collection|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|protocols|Int32|**TODO: Add Description**|
|remoteAddressRanges|[iPv4Range](../resources/ipv4range.md) collection|**TODO: Add Description**|
|remotePortRanges|[numberRange](../resources/numberrange.md) collection|**TODO: Add Description**|
|routingPolicyType|vpnTrafficRuleRoutingPolicyType|**TODO: Add Description**. Possible values are: `none`, `splitTunnel`, `forceTunnel`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnTrafficRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnTrafficRule",
  "name": "String",
  "protocols": "Integer",
  "localPortRanges": [
    {
      "@odata.type": "microsoft.graph.numberRange"
    }
  ],
  "remotePortRanges": [
    {
      "@odata.type": "microsoft.graph.numberRange"
    }
  ],
  "localAddressRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4Range"
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

