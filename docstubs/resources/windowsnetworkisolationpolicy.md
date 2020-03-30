---
title: "windowsNetworkIsolationPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsNetworkIsolationPolicy resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|enterpriseCloudResources|[proxiedDomain](../resources/proxieddomain.md) collection||
|enterpriseInternalProxyServers|String collection||
|enterpriseIPRanges|[ipRange](../resources/iprange.md) collection||
|enterpriseIPRangesAreAuthoritative|Boolean||
|enterpriseNetworkDomainNames|String collection||
|enterpriseProxyServers|String collection||
|enterpriseProxyServersAreAuthoritative|Boolean||
|neutralDomainResources|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsNetworkIsolationPolicy",
  "enterpriseNetworkDomainNames": [
    "String"
  ],
  "enterpriseCloudResources": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4CidrRange",
      "cidrAddress": "String"
    }
  ],
  "enterpriseInternalProxyServers": [
    "String"
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    "String"
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    "String"
  ]
}
```

