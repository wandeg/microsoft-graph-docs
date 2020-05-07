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
|authorizedApplicationRulesFromGroupPolicyNotMerged|Boolean|**TODO: Add Description**|
|connectionSecurityRulesFromGroupPolicyMerged|Boolean|**TODO: Add Description**|
|connectionSecurityRulesFromGroupPolicyNotMerged|Boolean|**TODO: Add Description**|
|firewallEnabled|stateManagementSetting|**TODO: Add Description**. Possible values are: `notConfigured`, `blocked`, `allowed`.|
|globalPortRulesFromGroupPolicyMerged|Boolean|**TODO: Add Description**|
|globalPortRulesFromGroupPolicyNotMerged|Boolean|**TODO: Add Description**|
|inboundConnectionsBlocked|Boolean|**TODO: Add Description**|
|inboundConnectionsRequired|Boolean|**TODO: Add Description**|
|inboundNotificationsBlocked|Boolean|**TODO: Add Description**|
|inboundNotificationsRequired|Boolean|**TODO: Add Description**|
|incomingTrafficBlocked|Boolean|**TODO: Add Description**|
|incomingTrafficRequired|Boolean|**TODO: Add Description**|
|outboundConnectionsBlocked|Boolean|**TODO: Add Description**|
|outboundConnectionsRequired|Boolean|**TODO: Add Description**|
|policyRulesFromGroupPolicyMerged|Boolean|**TODO: Add Description**|
|policyRulesFromGroupPolicyNotMerged|Boolean|**TODO: Add Description**|
|securedPacketExemptionAllowed|Boolean|**TODO: Add Description**|
|securedPacketExemptionBlocked|Boolean|**TODO: Add Description**|
|stealthModeBlocked|Boolean|**TODO: Add Description**|
|stealthModeRequired|Boolean|**TODO: Add Description**|
|unicastResponsesToMulticastBroadcastsBlocked|Boolean|**TODO: Add Description**|
|unicastResponsesToMulticastBroadcastsRequired|Boolean|**TODO: Add Description**|

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
  "stealthModeRequired": "Boolean",
  "stealthModeBlocked": "Boolean",
  "incomingTrafficRequired": "Boolean",
  "incomingTrafficBlocked": "Boolean",
  "unicastResponsesToMulticastBroadcastsRequired": "Boolean",
  "unicastResponsesToMulticastBroadcastsBlocked": "Boolean",
  "inboundNotificationsRequired": "Boolean",
  "inboundNotificationsBlocked": "Boolean",
  "authorizedApplicationRulesFromGroupPolicyMerged": "Boolean",
  "authorizedApplicationRulesFromGroupPolicyNotMerged": "Boolean",
  "globalPortRulesFromGroupPolicyMerged": "Boolean",
  "globalPortRulesFromGroupPolicyNotMerged": "Boolean",
  "connectionSecurityRulesFromGroupPolicyMerged": "Boolean",
  "connectionSecurityRulesFromGroupPolicyNotMerged": "Boolean",
  "outboundConnectionsRequired": "Boolean",
  "outboundConnectionsBlocked": "Boolean",
  "inboundConnectionsRequired": "Boolean",
  "inboundConnectionsBlocked": "Boolean",
  "securedPacketExemptionAllowed": "Boolean",
  "securedPacketExemptionBlocked": "Boolean",
  "policyRulesFromGroupPolicyMerged": "Boolean",
  "policyRulesFromGroupPolicyNotMerged": "Boolean"
}
```

