---
title: "hostSecurityState resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# hostSecurityState resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|fqdn|String|**TODO: Add Description**|
|isAzureAdJoined|Boolean|**TODO: Add Description**|
|isAzureAdRegistered|Boolean|**TODO: Add Description**|
|isHybridAzureDomainJoined|Boolean|**TODO: Add Description**|
|netBiosName|String|**TODO: Add Description**|
|os|String|**TODO: Add Description**|
|privateIpAddress|String|**TODO: Add Description**|
|publicIpAddress|String|**TODO: Add Description**|
|riskScore|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hostSecurityState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hostSecurityState",
  "fqdn": "String",
  "isAzureAdJoined": true,
  "isAzureAdRegistered": true,
  "isHybridAzureDomainJoined": true,
  "netBiosName": "String",
  "os": "String",
  "privateIpAddress": "String",
  "publicIpAddress": "String",
  "riskScore": "String"
}
```

