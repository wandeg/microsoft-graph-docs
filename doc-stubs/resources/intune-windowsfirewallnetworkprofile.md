---
title: "windowsFirewallNetworkProfile resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsFirewallNetworkProfile resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|authorizedApplicationRulesFromGroupPolicyMerged|Boolean|**TODO: Add Description**|
|connectionSecurityRulesFromGroupPolicyMerged|Boolean|**TODO: Add Description**|
|firewallEnabled|stateManagementSetting|**TODO: Add Description**. Possible values are: `notConfigured`, `blocked`, `allowed`.|
|globalPortRulesFromGroupPolicyMerged|Boolean|**TODO: Add Description**|
|inboundConnectionsBlocked|Boolean|**TODO: Add Description**|
|inboundNotificationsBlocked|Boolean|**TODO: Add Description**|
|incomingTrafficBlocked|Boolean|**TODO: Add Description**|
|outboundConnectionsBlocked|Boolean|**TODO: Add Description**|
|policyRulesFromGroupPolicyMerged|Boolean|**TODO: Add Description**|
|securedPacketExemptionAllowed|Boolean|**TODO: Add Description**|
|stealthModeBlocked|Boolean|**TODO: Add Description**|
|unicastResponsesToMulticastBroadcastsBlocked|Boolean|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallNetworkProfile",
  "firewallEnabled": "String",
  "stealthModeBlocked": "Boolean",
  "incomingTrafficBlocked": "Boolean",
  "unicastResponsesToMulticastBroadcastsBlocked": "Boolean",
  "inboundNotificationsBlocked": "Boolean",
  "authorizedApplicationRulesFromGroupPolicyMerged": "Boolean",
  "globalPortRulesFromGroupPolicyMerged": "Boolean",
  "connectionSecurityRulesFromGroupPolicyMerged": "Boolean",
  "outboundConnectionsBlocked": "Boolean",
  "inboundConnectionsBlocked": "Boolean",
  "securedPacketExemptionAllowed": "Boolean",
  "policyRulesFromGroupPolicyMerged": "Boolean"
}
```

