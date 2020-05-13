---
title: "networkConnection resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# networkConnection resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationName|String|**TODO: Add Description**|
|destinationAddress|String|**TODO: Add Description**|
|destinationDomain|String|**TODO: Add Description**|
|destinationPort|String|**TODO: Add Description**|
|destinationUrl|String|**TODO: Add Description**|
|direction|connectionDirection|**TODO: Add Description**. Possible values are: `unknown`, `inbound`, `outbound`, `unknownFutureValue`.|
|domainRegisteredDateTime|DateTimeOffset|**TODO: Add Description**|
|localDnsName|String|**TODO: Add Description**|
|natDestinationAddress|String|**TODO: Add Description**|
|natDestinationPort|String|**TODO: Add Description**|
|natSourceAddress|String|**TODO: Add Description**|
|natSourcePort|String|**TODO: Add Description**|
|protocol|securityNetworkProtocol|**TODO: Add Description**. Possible values are: `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`, `unknownFutureValue`, `unknown`.|
|riskScore|String|**TODO: Add Description**|
|sourceAddress|String|**TODO: Add Description**|
|sourcePort|String|**TODO: Add Description**|
|status|connectionStatus|**TODO: Add Description**. Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`, `unknownFutureValue`.|
|urlParameters|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.networkConnection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkConnection",
  "applicationName": "String",
  "destinationAddress": "String",
  "destinationDomain": "String",
  "destinationPort": "String",
  "destinationUrl": "String",
  "direction": "String",
  "domainRegisteredDateTime": "String (timestamp)",
  "localDnsName": "String",
  "natDestinationAddress": "String",
  "natDestinationPort": "String",
  "natSourceAddress": "String",
  "natSourcePort": "String",
  "protocol": "String",
  "riskScore": "String",
  "sourceAddress": "String",
  "sourcePort": "String",
  "status": "String",
  "urlParameters": "String"
}
```

