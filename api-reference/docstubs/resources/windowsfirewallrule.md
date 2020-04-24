---
title: "windowsFirewallRule resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsFirewallRule resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|stateManagementSetting|The action the rule enforces. If not specified, the default is Allowed. Possible values are: `notConfigured`, `blocked`, `allowed`.|
|description|String|The description of the rule.|
|displayName|String|The display name of the rule. Does not need to be unique.|
|edgeTraversal|stateManagementSetting|Indicates whether edge traversal is enabled or disabled for this rule. The EdgeTraversal setting indicates that specific inbound traffic is allowed to tunnel through NATs and other edge devices using the Teredo tunneling technology. In order for this setting to work correctly, the application or service with the inbound firewall rule needs to support IPv6. The primary application of this setting allows listeners on the host to be globally addressable through a Teredo IPv6 address. New rules have the EdgeTraversal property disabled by default. Possible values are: `notConfigured`, `blocked`, `allowed`.|
|filePath|String|The full file path of an app that's affected by the firewall rule.|
|interfaceTypes|windowsFirewallRuleInterfaceTypes|The interface types of the rule. Possible values are: `notConfigured`, `remoteAccess`, `wireless`, `lan`.|
|localAddressRanges|String collection|List of local addresses covered by the rule. Default is any address. Valid tokens include:<ul><li>"*" indicates any local address. If present, this must be the only token included.</li><li>A subnet can be specified using either the subnet mask or network prefix notation. If neither a subnet mask nor a network prefix is specified, the subnet mask defaults to 255.255.255.255.</li><li>A valid IPv6 address.</li><li>An IPv4 address range in the format of "start address - end address" with no spaces included.</li><li>An IPv6 address range in the format of "start address - end address" with no spaces included.</li></ul>|
|localPortRanges|String collection|List of local port ranges. For example, "100-120", "200", "300-320". If not specified, the default is All.|
|localUserAuthorizations|String|Specifies the list of authorized local users for the app container. This is a string in Security Descriptor Definition Language (SDDL) format.|
|packageFamilyName|String|The package family name of a Microsoft Store application that's affected by the firewall rule.|
|profileTypes|windowsFirewallRuleNetworkProfileTypes|Specifies the profiles to which the rule belongs. If not specified, the default is All. Possible values are: `notConfigured`, `domain`, `private`, `public`.|
|protocol|Int32|0-255 number representing the IP protocol (TCP = 6, UDP = 17). If not specified, the default is All. Valid values 0 to 255|
|remoteAddressRanges|String collection|List of tokens specifying the remote addresses covered by the rule. Tokens are case insensitive. Default is any address. Valid tokens include:<ul><li>"*" indicates any remote address. If present, this must be the only token included.</li><li>"Defaultgateway"</li><li>"DHCP"</li><li>"DNS"</li><li>"WINS"</li><li>"Intranet" (supported on Windows versions 1809+)</li><li>"RmtIntranet" (supported on Windows versions 1809+)</li><li>"Internet" (supported on Windows versions 1809+)</li><li>"Ply2Renders" (supported on Windows versions 1809+)</li><li>"LocalSubnet" indicates any local address on the local subnet.</li><li>A subnet can be specified using either the subnet mask or network prefix notation. If neither a subnet mask nor a network prefix is specified, the subnet mask defaults to 255.255.255.255.</li><li>A valid IPv6 address.</li><li>An IPv4 address range in the format of "start address - end address" with no spaces included.</li><li>An IPv6 address range in the format of "start address - end address" with no spaces included.</li></ul>|
|remotePortRanges|String collection|List of remote port ranges. For example, "100-120", "200", "300-320". If not specified, the default is All.|
|serviceName|String|The name used in cases when a service, not an application, is sending or receiving traffic.|
|trafficDirection|windowsFirewallRuleTrafficDirectionType|The traffic direction that the rule is enabled for. If not specified, the default is Out. Possible values are: `notConfigured`, `out`, `in`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallRule",
  "displayName": "String",
  "description": "String",
  "packageFamilyName": "String",
  "filePath": "String",
  "serviceName": "String",
  "protocol": 1024,
  "localPortRanges": [
    "String"
  ],
  "remotePortRanges": [
    "String"
  ],
  "localAddressRanges": [
    "String"
  ],
  "remoteAddressRanges": [
    "String"
  ],
  "profileTypes": "String",
  "action": "String",
  "trafficDirection": "String",
  "interfaceTypes": "String",
  "edgeTraversal": "String",
  "localUserAuthorizations": "String"
}
```

