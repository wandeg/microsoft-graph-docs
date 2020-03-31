---
title: "windowsFirewallNetworkProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsFirewallNetworkProfile resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|authorizedApplicationRulesFromGroupPolicyMerged|Boolean||
|authorizedApplicationRulesFromGroupPolicyNotMerged|Boolean||
|connectionSecurityRulesFromGroupPolicyMerged|Boolean||
|connectionSecurityRulesFromGroupPolicyNotMerged|Boolean||
|firewallEnabled|Enumeration| Possible values are: `notConfigured`, `blocked`, `allowed`.|
|globalPortRulesFromGroupPolicyMerged|Boolean||
|globalPortRulesFromGroupPolicyNotMerged|Boolean||
|inboundConnectionsBlocked|Boolean||
|inboundConnectionsRequired|Boolean||
|inboundNotificationsBlocked|Boolean||
|inboundNotificationsRequired|Boolean||
|incomingTrafficBlocked|Boolean||
|incomingTrafficRequired|Boolean||
|outboundConnectionsBlocked|Boolean||
|outboundConnectionsRequired|Boolean||
|policyRulesFromGroupPolicyMerged|Boolean||
|policyRulesFromGroupPolicyNotMerged|Boolean||
|securedPacketExemptionAllowed|Boolean||
|securedPacketExemptionBlocked|Boolean||
|stealthModeBlocked|Boolean||
|stealthModeRequired|Boolean||
|unicastResponsesToMulticastBroadcastsBlocked|Boolean||
|unicastResponsesToMulticastBroadcastsRequired|Boolean||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallNetworkProfile",
  "firewallEnabled": "String",
  "stealthModeRequired": true,
  "stealthModeBlocked": true,
  "incomingTrafficRequired": true,
  "incomingTrafficBlocked": true,
  "unicastResponsesToMulticastBroadcastsRequired": true,
  "unicastResponsesToMulticastBroadcastsBlocked": true,
  "inboundNotificationsRequired": true,
  "inboundNotificationsBlocked": true,
  "authorizedApplicationRulesFromGroupPolicyMerged": true,
  "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
  "globalPortRulesFromGroupPolicyMerged": true,
  "globalPortRulesFromGroupPolicyNotMerged": true,
  "connectionSecurityRulesFromGroupPolicyMerged": true,
  "connectionSecurityRulesFromGroupPolicyNotMerged": true,
  "outboundConnectionsRequired": true,
  "outboundConnectionsBlocked": true,
  "inboundConnectionsRequired": true,
  "inboundConnectionsBlocked": true,
  "securedPacketExemptionAllowed": true,
  "securedPacketExemptionBlocked": true,
  "policyRulesFromGroupPolicyMerged": true,
  "policyRulesFromGroupPolicyNotMerged": true
}
```

