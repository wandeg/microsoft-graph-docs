---
title: "windowsNetworkIsolationPolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsNetworkIsolationPolicy resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|enterpriseCloudResources|[proxiedDomain](../resources/proxieddomain.md) collection|**TODO: Add Description**|
|enterpriseInternalProxyServers|String collection|**TODO: Add Description**|
|enterpriseIPRanges|[ipRange](../resources/iprange.md) collection|**TODO: Add Description**|
|enterpriseIPRangesAreAuthoritative|Boolean|**TODO: Add Description**|
|enterpriseNetworkDomainNames|String collection|**TODO: Add Description**|
|enterpriseProxyServers|String collection|**TODO: Add Description**|
|enterpriseProxyServersAreAuthoritative|Boolean|**TODO: Add Description**|
|neutralDomainResources|String collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
      "@odata.type": "microsoft.graph.proxiedDomain"
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4CidrRange"
    }
  ],
  "enterpriseInternalProxyServers": [
    "String"
  ],
  "enterpriseIPRangesAreAuthoritative": "Boolean",
  "enterpriseProxyServers": [
    "String"
  ],
  "enterpriseProxyServersAreAuthoritative": "Boolean",
  "neutralDomainResources": [
    "String"
  ]
}
```

